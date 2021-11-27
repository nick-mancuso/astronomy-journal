# Color Image Lab

Object: M31

### Create a Color Image

I think that the automatic image generator did a pretty good job with the
initial image; it is not too dark. I think that the colors are realistic.
The image produced with the automatic settings is consistent with other
images that I have seen of M31.

All of the specifed adjustments had the intended effect on the image, such
as increasing the brightness, histogram hipoint, etc.

> Experiment on your own, and record the values you find for your image

I found that a subjectively "better" image was produced by:
gamma: 1.8
highlight saturation: 70%
shadow saturation: 60%
brightness 0.9977
histogram hipoint: 0.9977

> How does changing the Image Brightness affect color balance?

Colors appear more intense when increasing the brightness.

> How does the Histogram HiPoint affect the color balance?

It seems to affect the "warmth" of the image.

### Color Effect

> Click “Apply Color Effect”. What changes in the image? 

Nothing that I can tell.

> What is chromatic aberration?

It is an effect that is caused by different wavelengths of light traveling at
different speeds when passing through a lens.

> What is saturation?

The intensity of color in an image.

> How do the Rolloffs and Cutoffs affect the color balance?

They cut off certain wavelengths of light, effectively changing the saturation
of the image.

> Experiment with the input values. Can you make the saturated stars look “unsaturated”?

Yes. This can be achieved by increasing the "Low Rolloff" value.

### Manual Settings in Join Colrs Tool

> What happens if you set the various Sky colors to a high value (lets say 1000)?

The entire image appears like a blue-green filter has been applied to it.

> What happens if you set the values to 100?

The entire image looks like a blue-violet filter has been placed over it.

> What happens when you double the various Bright settings?

The entire image has a yellow tint.

> What happens when you set them to 0.05?

The entire image has a red tint.

##

Star | X coord | Y coord | Blue | Green | Red | Clear |
-----|---------|---------|------|-------|-----|-------|
1 | 70.555 | 419.830 | 62363.0 | 148345.5 | 280908 |  |
2 | 293.483 | 662.801 | 198708.7 | 659735 | 1466009 |  |
3 | 356.578 | 664.404 | 65441.7 | 152663.3 | 285853.0 |  |
4 | 379.306 | 620.888 | 12109.19 | 30038.3 | 59396.7 |  |
5 | 345.173 | 568.364 | 17026.7 | 44201.6 | 88879.7 |  |
6 | 305.348 | 530.432 | 58959.9 | 132190.6 | 245335.0 |  |
7 | 253.137 | 419.909 | 6493.63 | 21448.3 | 50967.4 |  |
8 | 788.374 | 585.895 | 206181.0 | 666085 | 1470033.0 |  |
9 | 690.970 | 512.532 | 48883.4 | 104841.0 | 192082.0 |  |
10 | 469.581 | 374.927 | 5703.1 | 16109.45 | 34115.4 |  |


Graph created from above dataset: https://docs.google.com/spreadsheets/d/e/2PACX-1vTIXcC1rpPx0X8hbgHm-owvCWIqioUfGaR3_suqdyYKKWxx-ez2MK9OPNj5fBKZac8273rW4zvwr7Wn/pubhtml

I found that the two values are very close; I had to use an absolute value function inside of the logarithm since the difference of some of the values
were negative.