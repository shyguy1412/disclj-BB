<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [bitburner](./bitburner.md) &gt; [GoCheat](./bitburner.gocheat.md) &gt; [removeRouter](./bitburner.gocheat.removerouter.md)

## GoCheat.removeRouter() method

Attempts to remove an existing router, leaving an empty node behind.

Success chance can be seen via ns.go.getCheatSuccessChance()

Warning: if you fail to play a cheat move, your turn will be skipped. After your first cheat attempt, if you fail, there is a small (\~10%) chance you will instantly be ejected from the subnet.

**Signature:**

```typescript
removeRouter(
    x: number,
    y: number,
    playAsWhite?: boolean,
  ): Promise<{
    type: "move" | "pass" | "gameOver";
    x: number | null;
    y: number | null;
  }>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  x | number | x coordinate of router to remove |
|  y | number | y coordinate of router to remove |
|  playAsWhite | boolean | _(Optional)_ Optional override for playing as white. Can only be used when playing on a 'No AI' board. |

**Returns:**

Promise&lt;{ type: "move" \| "pass" \| "gameOver"; x: number \| null; y: number \| null; }&gt;

a promise that contains the opponent move's x and y coordinates (or pass) in response, or an indication if the game has ended

## Remarks

RAM cost: 8 GB Requires BitNode 14.2 to use

