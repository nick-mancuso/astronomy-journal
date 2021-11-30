# Advanced Image Enhancement

## moon.fts

> Compare this image with the original. How has the contrast and detail changed?

There is less contrast overall in the "crisp" image, but the image also
appears less blurry (I suppose this is the "crispening"). You can notice
a much greater definition in the craters and other terrain.

> Compare the “hot” pixels in the original image with those in the enhanced image.

The "hot" pixels are much more noticable now, and have a thick, distinct
black border.

## mars images

>  View the fits headers of two of the images and record the exposure time.

mars.00000017.NA.fts:

```

SIMPLE  =                    T / CONFORMS TO FITS                               
BITPIX  =                   16 / 16-BIT TWOS COMP INTEGER                       
NAXIS   =                    2 / CONFORMS TO FITS                               
NAXIS1  =                  150 / NUMBER OF PIXELS PER ROW                       
NAXIS2  =                  150 / NUMBER OF ROWS                                 
BSCALE  =                  1.0 / REAL = FITS_VALUE * BSCALE + BZERO             
BZERO   =                  0.0 /                                                
OBJECT  = '                    '                                                
DATE-OBS= '2003-10-03          '                                                
TIME-OBS= '02:56:05            '                                                
TELESCOP= '80.0 35.0           '                                                
INSTRUME= 'Apogee AM and AP Series'                                             
OBSERVER= 'Observer            '                                                
OBSERVAT=                                                                       
EXPOSURE= +1.000000000000e-002                                                  
HISTORY    

```

mars.00000016.NA.fts:

```

SIMPLE  =                    T / CONFORMS TO FITS                               
BITPIX  =                   16 / 16-BIT TWOS COMP INTEGER                       
NAXIS   =                    2 / CONFORMS TO FITS                               
NAXIS1  =                  150 / NUMBER OF PIXELS PER ROW                       
NAXIS2  =                  150 / NUMBER OF ROWS                                 
BSCALE  =                  1.0 / REAL = FITS_VALUE * BSCALE + BZERO             
BZERO   =                  0.0 /                                                
OBJECT  = '                    '                                                
DATE-OBS= '2003-10-03          '                                                
TIME-OBS= '02:55:55            '                                                
TELESCOP= '80.0 35.0           '                                                
INSTRUME= 'Apogee AM and AP Series'                                             
OBSERVER= 'Observer            '                                                
OBSERVAT=                                                                       
EXPOSURE= +1.000000000000e-002                                                  
HISTORY                                                                         
COMMENT                                                                         
ORIGIN  = 'Origin              '                                                
FOCALLEN= +8.000000000000e+001                                                  
APERTURE= +3.500000000000e+001                                                  
OBJCTRA = '00 00 00.000        '                                                
OBJCTDEC= '+00 00 00.00        '                                                
ORCHCOMM= '                    '                                                
TEMPERAT= -4.000000000000e+001                                                  
CBLACK  =                 5004                                                  
CWHITE  =                 5834                                                  
HISTORY   Original image: mars.00000016.NA.FIT                                  
HISTORY   Auto-processed: Planetary                                             
HISTORY   Calibrated                                                            
HISTORY   Planet Centered                                                       
HISTORY   Cropped to 150 x 150                                                  
COMMENT Processed using Aip32 version 1.4.15, SN:00000119 on 10/03/03           
END  

```

> Are they the same exposure time?

Yes.

> Do the images all look the same?

Mostly, yes.

> How can you explain the differences?

The sumdges, which I can surmise are the Martian terrain, appear a bit to
be a bit different in each image. I would guess that this is due to the rotation of Mars, and the movement of Earth.

Also, the sunlight is reflected at a different angle in each.

> Record which Mars images are clearer than the others.

00000005.NA.fts
00000016.NA.fts
00000006.NA.fts
00000012.NA.fts
00000001.NA.fts

> Pick one of the images that is fairly sharp and another that is of medium quality.
> Start with the fairly sharp image. Click EnhanceÆConvolution Filters Æ Crispen. A
> new image will appear. Compare this image with the original. How has the contrast and
> detail changed? 

It is tough to tell; I would say that the "medium" quality image got worse,
while the fairly sharp image did improve.

> How does “sharpen” compare with “crispen”?

Sharpen seems to add a greater depth and defintion, but also make reflected
light from Mars look like part of the planet.

> Which filter (crispen or sharpen) do you feel is stronger?

I think that sharpen is definitely stronger.

> Open one of the calibrated images of an object we’ve observed in class. Make
> sure it is an image that contains stars. Try “EnhanceÆ Convolution FiltersÆSharpen” on this image.

> What happens to the stars?

They look like nerds (the candy); they are misshapen blobs with dark borders.

> Looking at the crispening operators given above, why do you think this happens to stars?

Since they are smaller objects (point source), the center of the star's pixel
value is getting increased while the outside edges (border) is decreasing.

>Return to the original Moon image. Apply “EnhanceÆConvolution FiltersÆ
> Smooth” and “EnhanceÆConvolution FiltersÆ Blur” to the original images. The crispen
> and sharpen filters are called “high pass” filters. They are designed to bring out details.
> The Smooth filter is an example of a “low pass” filter.

> Compare the smoothed image with the original. What are the differences?

Most notable is the removal of the "hot" pixels. There is also a slight loss
of defintion in the terrain of the moon.

> What do you think “low pass” filters are designed to do?

Reduce/ remove pixels with a high value.

> Sometimes giving objects in an image a three dimensional feel helps to isolate
> faint objects. The bas relief filter makes a copy of the images, shifts it by one pixel, and
> subtracts that from the original image. Try the “Enhance -> Convolution Filters -> Bas
> Relief on the original moon and Mars images. What happens to each?

They both appear to look like a plaster cast of the respective object;
textured, three dimensional, and mostly white and grey.

> Experiment with the Gradient, 3x3, and 5x5 Emboss filters.
> What do you think these filters are designed to detect?

To me, it seems like these filters are designed to make terrain and 
geological features more prominent.

> Experiment with the Sobel, Kirsch, and Prewitt Operators on the moon images.
> What do you think these filters are designed to enhance?

These filters seem to enhance valleys and channels the most.

## Convolution by Unsharp Masking

TODO: complete this section
