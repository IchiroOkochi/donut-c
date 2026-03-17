# Donut C

This folder contains the legendary spinning ASCII donut in C, but with one important extra joke: the source code itself has been arranged into the shape of a donut.

Important credit where it belongs: the original `donut.c` logic was created by Andy Sloane. The point of this version is not to pretend the algorithm is new. The point is to present that iconic code as a little code-art object where the donut program is also visually shaped like a donut.

## What This Is

`donut.c` prints an animated torus directly in the terminal using ASCII characters and a surprisingly small amount of code.

This version keeps the classic donut animation, but reformats the source so the file itself looks like a donut when you open it. That is the twist.

It is:

- computer graphics
- terminal art
- math cosplay
- one of the great snacks in programming history
- a tribute remix, not a claim of invention

## Why People Love It

Because it feels impossible the first time you see it.

Because it is clever without being huge.

Because a spinning donut made of punctuation is simply good for morale.

## Credit

The original donut animation and source are by Andy Sloane.

- Original post: [Donut math: how donut.c works](https://www.a1k0n.net/2006/09/15/obfuscated-c-donut.html)
- Original source: [donut.c](https://www.a1k0n.net/2006/09/15/obfuscated-c-donut.html#donut)

## Files

- `donut.c` - Andy Sloane's classic donut logic, reformatted into a donut-shaped source layout
- `assets/donut.png` - a preview image of the donut-shaped source itself
- `README.md` - the official pastry label

## What Makes This Version Different

If this were just a plain repost of the original code, there would not be much point.

The fun here is that the source has been arranged into the shape of the thing it renders. It is still executable C, but it also works as visual code art. The program draws a donut, and the code is a donut, which is exactly the kind of unnecessary commitment that makes projects memorable.

## How The Code Works

At a high level, the program:

1. Loops over points on a mathematical torus.
2. Rotates that shape in 3D space.
3. Projects the 3D points onto a 2D terminal grid.
4. Chooses ASCII characters based on brightness so the donut looks shaded.
5. Repeats fast enough to create animation.

Even if the formatting is playful, the underlying idea is still a smart little graphics demo:

- `z[1760]` stores depth values so nearer points win
- `b[1760]` stores the character buffer printed to the terminal
- the nested loops walk around the donut surface
- the trig handles rotation and projection
- the ASCII ramp `".,-~:;=!*#$@"` acts like a tiny lighting system

## How To Run It

Compile with `gcc`:

```bash
gcc donut.c -o donut -lm
./donut
```

On systems where `unistd.h` or `usleep` behaves differently, you may need a small platform-specific adjustment, but the idea stays the same: compile, run, admire pastry.

## Why Keep It Like This

Because the source layout is the whole point.

This is part homage, part formatting stunt, part tiny gallery piece for one of the internet's most beloved C programs.

## In One Sentence

An iconic ASCII donut in C by Andy Sloane, presented here as executable code art where the program renders a donut and the source is shaped like one too.
