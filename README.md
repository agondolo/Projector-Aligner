# Space Engineers Projector Aligner

All configuration is done through Custom Data. Simply create a heading
in the custom data of any block that you wish to use with this script:

```ini
[projector]
```

You may add cockpits, flight seats, remote controls and projectors.
By default all blocks will be in the "default" projector group. You can
change this by specifying a group name. For example:

```ini
[projector]
group=Ship Printer
```

To make use of a display, specify a display number and (optionally) a
scale and a color. For example:

```ini
[projector]
display=0
scale=0.5
color=00CED1
```

Change the number to the screen that you wish to use; numbers start at 0, so a
five-screen cockpit has screens 0, 1, 2, 3 and 4.
Color should be entered as six hexadecimal digits representing red, green and blue.

Arguments
---------

- `up`             Move up one line on screen
- `down`           Move down one line on screen
- `apply`          Enter Menu / Select current projector from Menu
- `select`           "
- `build`          Re-read the Custom Data of blocks, and reconfigure
- `rebuild`          "

If you wish to control a group other than "default", append its name to the
argument, using quotes if the group name has spaces in it.
