# Fredoka One: Adding The Hebrew Script

The Fredoka One is originally designed by Milena Brandao and is licensed under the SIL Open Font License (v1.1)

## Design Process

Design #5 - 18.10.15:

![Design #5](documentation/10.png)

Design #4 - 30.9.15 (plus [test.pdf](documentation/test.pdf))

![Design #4](documentation/7.png)
       
Design #3 - 20.9.15

![Design #3a](documentation/6.png)

![Design #3b](documentation/5.png)

Design #2 - 16.9.15

![Design #2](documentation/4.png)

Design #1 - 15.9.15

![Design #1](documentation/1.png)

## Build Process

OTF exported from `Fredoka.glyphs` with Glyphs 2.3 with Remove Overlap and Autohinting enabled.

TTF exported from `Fredoka.glyphs` with Glyphs 2.3 with Remove Overlap but without autohinting, then hinted with ttfautohint using this command:

    ttfautohint  \
      --composites  \
      --default-script=latn  \
      --fallback-script=hebr  \
      --detailed-info  \
      --verbose  \
      --strong-stem-width=G  \
      --windows-compatibility  \
      --increase-x-height=0 \
      FredokaOne-Regular.ttf \
      FredokaOne-Regular-ta.ttf;

Note that the `increase-x-height` feature is de-activated to make hand-hinting in the future easier to do without creating visible changes.
