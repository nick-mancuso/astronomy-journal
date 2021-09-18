### Astronomical Image Processing for Windows V6

#### Basic Use of the Program


Images are from the `20200113rm` archive.

-------------------------

##### Bias Frames
removed bias images 1-4, 8, 10-13 (much lighter than others)


Bias file stats:
```
Image Statistics for [14] sarm20200113bias-014.fits:
  Image Type: Greyscale
  Image Width: 2048
  Image Height: 2048
  Data Bytes: 16777216
  Minimum: 268.0
  Maximum: 868.0
  Mean:    301.28
  Median:  301.0
  Std Dev: 6.31531
  Skew:    0.226059
  Ignore:  10.0%
  Camera Type: STL-4020M/CM 1x1         
  Pixel Width: 7.4
  Pixel Height: 7.4
```

Master bias:

```
Image Statistics for [21] Averaged: [5] & [6]:
  Image Type: Greyscale
  Image Width: 2048
  Image Height: 2048
  Data Bytes: 16777216
  Minimum: 279.0
  Maximum: 707.0
  Mean:    301.216
  Median:  300.999
  Std Dev: 4.47434
  Skew:    0.380077
  Ignore:  10.0%
  Camera Type: STL-4020M/CM 1x1         
  Pixel Width: 7.4
  Pixel Height: 7.4
  Original image: Z:\home\nick\Astronomy\20200113rm\sarm20200113bias-005.fits
  Averaged with Z:\home\nick\Astronomy\20200113rm\sarm20200113bias-006.fits
```

Average of Two Images

> 1) How does the standard deviation compare to your measurement for a single image?

The standard deviation(SD) is significantly lower (6.31 vs. 4.47).

> 2) How would you expect the standard deviation to behave when averaging multiple
images?

I would expect it to be further reduced, since our proportion of consistent data is
increasing.

Average Combine

> 1) How does the appearance of this image compare with your single images?

This image is very consistent, and a bit darker than some of the images. I
do not notice any "noise".

> 2) Click "Measure", "Statistics" and "Image". Record min, max, mean and standard
deviation for this image in your journal. How does the standard deviation
compare to your measurement for a single image?

```
Image Statistics for [22] Average of 11 images:
  Image Type: Greyscale
  Image Width: 2048
  Image Height: 2048
  Data Bytes: 16777216
  Minimum: 291.273
  Maximum: 889.818
  Mean:    300.803
  Median:  300.814
  Std Dev: 1.983586
  Skew:    14.12044
  Ignore:  10.0%
  ```
  The average of 11 images SD is MUCH lower than the single image SD (6.31 vs. 1.98).

  > 3) How does the standard deviation compare to your measurement for your average
of two images?

  The average of 11 images SD is lower than the two image average SD (4.47 vs. 1.98).

  > 4) Why?

  This is because the number of consistent data points (close to the mean) has
  now greatly increased.


##### Dark Frames
Dark file stats:

```
Image Statistics for [28] sarm20200113dark-006.fits:
  Image Type: Greyscale
  Image Width: 2048
  Image Height: 2048
  Data Bytes: 16777216
  Minimum: 267.0
  Maximum: 6179.0
  Mean:    301.109
  Median:  300.994
  Std Dev: 7.07562
  Skew:    142.7397
  Ignore:  10.0%
  Camera Type: STL-4020M/CM 1x1         
  Pixel Width: 7.4
  Pixel Height: 7.4

```

Average of Two Images

> 1) How does the standard deviation compare to your measurement for a single
image? 

```
Image Statistics for [33] Averaged: [23] & [24]:
  Image Type: Greyscale
  Image Width: 2048
  Image Height: 2048
  Data Bytes: 16777216
  Minimum: 277.0
  Maximum: 6204.0
  Mean:    300.223
  Median:  299.997
  Std Dev: 5.794
  Skew:    278.916
  Ignore:  10.0%
  Camera Type: STL-4020M/CM 1x1         
  Pixel Width: 7.4
  Pixel Height: 7.4
  Original image: Z:\home\nick\Astronomy\20200113rm\sarm20200113dark-001.fits
  Averaged with Z:\home\nick\Astronomy\20200113rm\sarm20200113dark-002.fits

```

The standard deviation(SD) is significantly lower (7.07 vs. 5.79).


> 2) How would you expect the standard deviation to behave when averaging multiple
images?

I would expect it to be further reduced, since our proportion of consistent data is
increasing.

Average Combine

> 1) How does the appearance of this image compare with your single images?

This image is very consistent, it just looks like a solid black image.

> 2) Click "Measure", "Statistics" and "Image". Record min, max, mean and standard
deviation for this image in your journal. How does the standard deviation
compare to your measurement for a single image?

```
Image Statistics for [34] Average of 10 images:
  Image Type: Greyscale
  Image Width: 2048
  Image Height: 2048
  Data Bytes: 16777216
  Minimum: 289.5
  Maximum: 6138.6
  Mean:    300.153
  Median:  300.087
  Std Dev: 3.83272
  Skew:    863.868
  Ignore:  10.0%

  ```
  The average of 11 images SD is MUCH lower than the single image SD (7.07 vs. 3.83).

  > 3) How does the standard deviation compare to your measurement for your average
of two images?

  The average of 11 images SD is lower than the two image average SD (5.79 vs. 3.83).

  > 4) Why?

  This is because the number of consistent data points (close to the mean) has
  now greatly increased.


-----------------------

> 1) How does the mean value for the "master" dark compare with the mean value for
the "master" bias? Consider what you know about bias and dark images, and
present a theory to explain the differences.

Master bias mean: 300.803
Master dark mean: 300.153

The means of these two master images are very close in value. The "dark" frames
have a lower mean, which is not what I would expect from our discussion last week.
I would have expected the "dark" frames to have picked up additional electrons 
from the heat generated by the CCD.

### Master Thermal

 > 1) Click "Measure", "Statistics" and "Image". Record the information about this
image in your journal.

```
Image Statistics for [69] Subtracted: [34] - [68]:
  Image Type: Greyscale
  Image Width: 2048
  Image Height: 2048
  Data Bytes: 16777216
  Minimum: -590.318
  Maximum: 5838.6
  Mean:    -0.650108
  Median:  -0.722126
  Std Dev: 4.30313
  Skew:    609.213
  Ignore:  10.0%
  Average of 10 images
  Subtracted Z:\home\nick\Astronomy\20200113rm\sarm20200113bias-012.fits

```



> 2) How does the mean value for this image compare with the mean value for the
master bias and the master dark?

The mean is negative, which is not what I would expect.


> 3) What is thermal noise? How does this agree with your theory presented above?

The thermal noise should be the heat generated by the operation of the CCD.
My theory above... TODO: Complete

### Flat Image

> 1) Click "Measure", "Statistics" and "Image". Record the information about this
image in your journal.

```
Image Statistics for [70] sarm20200113flatb-001.fits:
  Image Type: Greyscale
  Image Width: 2048
  Image Height: 2048
  Data Bytes: 16777216
  Minimum: 2354.0
  Maximum: 39890.0
  Mean:    32948.6
  Median:  32987.9
  Std Dev: 647.082
  Skew:    -0.564015
  Ignore:  10.0%
  Camera Type: STL-4020M/CM 1x1         
  Pixel Width: 7.4
  Pixel Height: 7.4

```



> 2) How does the appearance of this image compare with the biases and the darks?

This image is much brighter, and there are a few noticable objects.

> 3) How does the mean value compare the mean of the biases and the darks?

It is many orders of magnitude greater than the biases and darks.

> 4) Create a "master" flat by averaging all of the individual images for the same filter.
(should be 15-20 individual images). It is very important that you use only those
flats taking with the SAME FILTER.

I used the blue filter flats.


> 5) Click "Measure", "Statistics" and "Image". Record the information about this
average flat in your journal.

```
Image Statistics for [86] Average of 16 images:
  Image Type: Greyscale
  Image Width: 2048
  Image Height: 2048
  Data Bytes: 16777216
  Minimum: 2197.06
  Maximum: 30153.6
  Mean:    28296.8
  Median:  28335.9
  Std Dev: 533.851
  Skew:    -0.647432
  Ignore:  10.0%

```


> 6) What is the mean for your flat image?

  Mean:    28296.8


> 7) The CCD has 16 bit electronics, which means the voltages from each pixel can be
converted to maximum value of 65536 (216). The CCD is not sensitive to
increased brightness beyond that limit. Flat images should be exposed long
enough to have a signal about half this value. Does the mean for your single flat
meet this requirement?

Yes.


8) How do the master flat’s statistics compare with the statistics for the master dark
and master bias images?

Even the minimums in the flat are much higher than the max of the dark and bias images.
The SD is also much higher than the bias and dark images.

9) Now, subtract the master bias and the thermal frame from the master flat.

Done.

10) Click "Measure", "Statistics" and "Image". Record the information about this
image in your journal. How do the statistics compare with the statistics of the
original master flat?

```
Image Statistics for [88] Subtracted: [87] - [68]:
  Image Type: Greyscale
  Image Width: 2048
  Image Height: 2048
  Data Bytes: 16777216
  Minimum: 1895.463
  Maximum: 29855.7
  Mean:    27996.6
  Median:  28035.8
  Std Dev: 533.899
  Skew:    -0.648711
  Ignore:  10.0%
  Average of 16 images
  Subtracted Z:\home\nick\Astronomy\20200113rm\sarm20200113bias-013.fits
  Subtracted Z:\home\nick\Astronomy\20200113rm\sarm20200113bias-012.fits

```
