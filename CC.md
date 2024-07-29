<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/Playtronica">
    <img src="static/logo.png" alt="Logo" width="100">
  </a>

<h3 align="center">TouchMe Continuous Controllers</h3>

  <p align="center">
    BODY IS AN INSTRUMENT
    <br />
    <a href="https://github.com/Playtronica/Biotron"><strong>Explore the docs »</strong></a>
    <br />
    <br />
  </p>
</div>

<!-- TABLE OF CONTENTS -->

<details >

  <summary>Table of Continuous Controllers</summary>

  <ol>

1)[Commands](#commands)
1) [Sensitivity (fib)](#sensitivity--fib-)
2) [Smoothness](#smoothness)
3) [Scale](#scale)
4) [Max Velocity](#max-velocity)
5) [Min Velocity](#min-velocity)
6) [Humanize](#humanize)
7) [Ultra sensitivity](#ultra-sensitivity)
8) [Same Note](#same-note)
9) [Note Off Percent](#note-off-percent)
10) [Light Notes Range](#light-notes-range)
11) [Light Pitch Bend](#light-pitch-bend)
12) [Performance Mode](#performance-mode)

  </ol>

</details>

# Description

It is list of Continuous Controllers.

# Commands

## Scale

### Description

Scale played from the device

### Input
- Num: CC 24


| Range Value | Scale      |
|-------------|------------|
| 0 - 10      | MAJOR      |
| 10 - 21     | MINOR      |
| 21 - 31     | CHROM      |
| 31 - 42     | DORIAN     |
| 42 - 52     | MIXOLYDIAN |
| 52 - 63     | LYDIAN     |
| 63 - 73     | WHOLETONE  |
| 73 - 84     | MINBLUES   |
| 84 - 95     | MAJBLUES   |
| 95 - 105    | MINPEN     |
| 105 - 116   | MAJPEN     |
| 116 - 127   | DIMINISHED |


## Change key

### Description

Start Note in default range (Disabled when custom range is active)

### Input
- Num: CC 23

| Range Value | Scale |
|-------------|-------|
| 0 - 10      | +1    |
| 10 - 21     | +2    |
| 21 - 31     | +3    |
| 31 - 42     | +4    |
| 42 - 52     | +5    |
| 52 - 63     | +6    |
| 63 - 73     | +7    |
| 73 - 84     | +8    |
| 84 - 95     | +9    |
| 95 - 105    | +10   |
| 105 - 116   | +11   |
| 116 - 127   | +12   |


## Mute

### Description

Disable note generation from the channel

### Input
Num: CC 3

Turn off mute if value < 63, else turn it on

## Humanize

### Description

Velocity randomization at a controlled interval for each channel.

### Input
Num: CC 9

Turn off humanize if value < 63, else turn it on


## Max Velocity

### Description

Max pressing force for each channel. (From plant and from light sensor)

### Input
Num: CC 15

Change max velocity of channel


## Min Velocity

### Description

Min pressing force for each channel. (From plant and from light sensor)

### Input
Num: CC 14

Change min velocity of channel

## Custom Range

### Description

Range of playable notes

### Input
Num: CC 20

Turn off Custom Range if value < 63, else turn it on


## Lowest Note

### Description

Lowest note of custom range

### Input
Num: CC 21

Change lowest note of custom range


## Highest Note

### Description

Highest note of custom range

### Input
Num: CC 22

Change highest note of custom range