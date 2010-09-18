# NAME

  colorcoke - modify the extended, non-ANSI terminal colorset

# DESCRIPTION

![screenshot](http://github.com/trapd00r/colorcoke/raw/master/extra/c256-red.png)

  colorcoke lets one modify the extended colorset (88-16 or 256-16 colors,
  respectively) for a running terminal session. The change takes effect
  immediately - no need to restart the terminal, like when using xrdb.

  Shades and tints can be generated for an arbitary number of ranges.

  The ANSI colors can be left untouched, be included in a shade or set
  separately. One can also exclude everything but the ANSI colors.
  The ANSI colors is untouched by default.

  The grey scale ramp (extended color index 232-255) is left untouched by
  default. To include them, set the end point to 255.

  Additional colors can be left untouched by specifying their index with the
  --no flag. This can also be configured in the configuration file.

  The base color to use is specified with the -c flag, and the stepping
  is controlled with the -r, -g and -b flag - red, green and blue channel.

  Red, blue and green amount is specified with -rr, -rg and -rb when the
  randomizing option is used.

# OPTIONS

    -c,   --color       the base color
    -r,   --red         red channel stepping
    -g,   --green       green channel stepping
    -b,   --blue        blue channel stepping
    -s,   --start       first color index to operate on (default: 17)
    -e,   --end         last  color index to operate on (default: 231)
    -a,   --ansi        modify the ANSI color range only
    -1,   --single      set a single color (HEX, index)
          --random      randomize the colors
    -rr,  --rand-red    control amount of red
    -rg,  --rand-green  control amount of green
    -rb,  --rand-blue   control amount of blue
    -N,   --no          do not modify color index n

    -h,   --help        show the help and exit
    -m,   --man         show the manpage and exit

# AUTHOR

Written by Magnus Woldrich

# COPYRIGHT

Copyright (C) 2010 Magnus Woldrich

Licence GPLv2
