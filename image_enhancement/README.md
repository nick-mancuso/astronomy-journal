# Image Enhancement

## Gradient Correction

 - top: mean = 1501.936
 - bottom: mean = 1434.895
 - left: mean = 1444.896
 - right: mean = 1386.658

## Brightness Scaling

 - min: 929.666
 - max: 22406.6
 - mean: 1485.102
 - sd: 139.8919

### Initial values

 - black point: 0.01
 - white point: 0.999
 - low pixel value: 1417.836
 - high pixel value: 2992.52

### Experiment

> Start by setting
> the Black Point to 0.01 and the White Point to 0.98. Record the new
> Black Point, White Point, and Low and High Pixel values.

They did not change at all, this was nearly the default settings.

> When you have an image you like, Record the Black Point, White Point,
> and the Low and High Pixel values for this image.

 - black point: 0.0
 - white point: 1.0
 - low pixel value: 0
 - high pixel value: 65535.0

> Record the information and compare it to your original image.
>  How have the Min and Max pixel values changed?

 - min: 0.0
 - max: 65535.0
 - mean: 2480.79
 - sd: 3918.8

> How does your scaled image differ from your original?

It's like a completely different image; I can see the arms and outer areas of
M31 with much greater definition and clarity. I can also see many more stars and differentiate between them readily.

## Gamma Scaling

> What does the transfer function for Gamma=1.0 look like?

It is linear.

> What does the transfer function for Gamma < 1 look like?

It increases very slowly until we approach the maximum p.

> What does the transfer function for Gamma > l look like?

It increases quickly and approaches y = 65535.

> Do you have to increase or decrease Gamma to emphasize the fainter background?

Increase

> What does the transfer function for Gamma=2.3 look like?

It looks like a sqrt function. (It is very close to this)

> What pixel values does it emphasize?

The medium and low values.

> What does the transfer function for Gamma=0.9 look like?

Nearly linear, slight upwards curve.

> What pixel values does it emphasize?

Medium and high values.

## Gamma Log Scaling

> What is the overall effect of logarithmic scaling?

It makes fainter objects more visible, and it is easier to discern between
different pixel values.

> Compare the gammalog function with γ=0.9 to the gamma function with the same value of γ (from step 3).

The gammalog function looks more like a sqrt function at this value, and emphasizes more of the fainter regions of the image.

> Use a gammalog value of 0.1 to scale your image. Subtract this
> gammalog image from the gamma=0.9 image (from step 3).

>  What does the subtracted image look like? 

Like an nearly exact opposite of the original gamma(0.9) image (things that are dark are light, and vice versa).

> Where is the pixel value zero?

In the center of M31.

> Where is it not zero?

In the arms and disk of M31, and the outer areas of stars.

> Can you determine what the major difference is between Gamma and Gammalog scaling?

How the medium and medium low pixel values are treated.

## Sawtooth and Quantized Scaling

> What does the sawtooth function look like?

A zigzag pattern.

> What does the quantize function look like?

Steps.

> Can you think of any situation where you might want to use sawtooth function?

To accentuate certain elements that are similar; i.e. if we only want to see a certain type/size/proximity (apparent magnitude) of a star.

> A quantize function?

To produce more marked transitions in pixel values for large objects (galaxies, etc.).

> Experiment with the sawtooth function on your first image. Describe what it does to the image.

The sawtooth function makes M31 appear to have "bands" or "divisions".

> Experiment with the quantize function. What values do you find that best brings out the faint stars?

Higher values bring out the fainter stars, due to higher function values at
lower pixel values (from increased number of steps).

> Describe this quantize function. Which technique is best for bringing out the faint stars?

See above, same answer.

## Histogram shaping

> Describe the shape of the histogram of your image.

It increases quickly to ~1400, then slowly decreases.


> What count value has the most pixels in each?

As stated above, about 1479.


> What feature in your images do you think is responsible for these pixels?

The disk of M31.

> What is the highest count value you found in each image?

22340.4

> What feature do you think is responsible for these pixels?

The center of M31.

## Exponential Histogram Shaping

> Slide the peak skew button all the way to the left. Describe the
> blue curve and what image features you think the new image with
> emphasize. Click “apply”. How does the new image compare to
> the original?

The blue curve is nearly constant, except at the endpoints. So, this peak skew
will emphasize all light sources/ pixel values. The new image is very "busy"
with lots of what I can only surmise is space dust.

> Slide the peak skew button to a mid point position. Describe the
> blue curve and what image features you think the new image will
> emphasize. Click “apply”. How does the new image compare to
> the original?

The blue curve is linear, and steadily decreasing. You can see many more stars, and much greater definition in the M31's disk and surrounding area.

> Slide the peak skew button to the right. Describe the blue curve
> and what features you think the new image will emphasize. Click
> “apply”. How does the new image compare with the original?

The blue curve is linearly decreasing, similar to the middle peak skew.
I think that the result will be similar to above, but perhaps the middle
range pixel values will be muted. This was an accurate estimate.

> Set the Peak Skew slider to a point around 40 (a little box with a...
> What features does the new image emphasize? 

The new image emphasizes the space dust and disk around M31 (middle range pixel values).

> Repeat for a Peak Skew value of 160.

The new image emphasizes many of the same, but focuses more on the lower-middle and middle range pixel values.

## Gaussian Histogram Shaping

> Set the Peak Skew slider to a point around 40 (a little box with a...
> What features does the new image emphasize? 

It is much higher for the lower pixel values, and makes the image almost entirely
grey/white.

> Repeat for a Peak Skew value of 160.

Basically the same as above, but it does not obfuscate the surrounding stars and galaxy
features as much.
