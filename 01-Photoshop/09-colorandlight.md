# Adjustment
- tools to control lights and color.
- access via layer panel, adjustment panel, image > adjustment.
- an adjustment layer impacts EVERY layer beneath it. or use clipping mask.
- on raster image adjustment layer via layer/adjustment panel should be used with a mask. (which is auto added). and via image menu permanently changes the image.
- on smart object the image menu option adds a smart filter (kind of mask) that doesn't permanently effect the image.
- divided sections:
    - background = solid color, gradient, pattern
    - lights = brightness/contrast, levels, curves, exposure
    - colors = vibrance, hue/saturation, etc.
    - extra = invert, gradient map, etc.

# Hue ('about color')
- Adjust the color shift across different colors. (red to green, x to y)
- use when you want to literally change the color of something.

# Saturation ('about color')
- How colorfull a color is. (dull vs bright)
- red: 0% = grey and 100% = pure bright red
- use when you want to make a certain color pop more.

# Midtone, higlight and shadow ('about light')
- the darkest parts of an image is the shadow.
- now the least shadow part is highlight and a lil bit shadow is midtone.
- can adjust using levels/curves. changing one thing will impact the other but that thing being changed will be impacted the most.

# Contrast ('about light')
- dark gets more darker and bright gets more brighter, the higher the contrast is.
- low contrast is called 'flat' meaning not much defination or seperation b/w colors of an image.
- increase contrast to add more detail/defination/seperation.
- to acces use 'brightness/contrast' adjustment layer.

---

# Levels
- if the graph is empty towards shadow or hightlight then simple bring the slider to wher graph starts from (don't leave empty graph)
- the graph (called histogram) shows where are most of the pixels in image are concentrated, towards shadows or highlight.
- there's two sliders:
    - the top is for input with histogram shown. meaning if you slide say dark slider where more of the histogram is covered then that means more pixels on image will be of darker light.
    - the bottom slider is for output. meaning you set 'how many' pixels will be dark/light with above slider and then with this one you set the light value of those said pixels. (ex: making dark pixels even darker or lighter.)
- you can sample pick the shadow or highlight part (atleast the part which is supposed to be that).
    - chose only 1 sample, if the image is very dark overall then go for selecting on white sample.

# Curves (most important light control)
- histogram shows, where are most of the pixels in image are concentrated, towards shadows or highlight.
- upper triangle increases highlights and lower triangle increases shadows.
- theory:
    - say an image is made of 100 pixels.
    - each pixel has its own color BUT also has its own light level (b/w dark [0] or bright [225]).
    - the vertical and horizontal axis sliders are like 'Levels' input slider, where you set how many of the pixels of image will be dark or light.
        - the concentration of pixels in any image can't be changed. the histogram will be fixed. if 20% pixel are light and rest are dark then you can't make 30% light. best you can do is make those 20% more lighter or more darker.
    - there is a linear line of graph which is by defualt at 45deg angle and goes from bottom left (value 0) to top right (value 225). works as output slider of 'Levels'.
        - any point on this line (added by clicking) means we are selecting all the pixels in the image of that particular light value. (show as input value)
            - ex: you add a point no. of 170 on that line, now every pixel in image who's light level is 170 is selected.
        - now when you move this point on line up and down (vertically) on the graph, then those pixel's light level is changed to that shown in output value.
- you can add multiple points, have a light value picker tool, different modes (rgb, red (opposite cyan), green (opposite magenta), blue (opposite yellow))

# Exposer
- exposer slider = controls highlights
- offset slider = controls shadows
- gamma corerction slider = controls midtones

# Vibrance
- similar to saturation but only difference is that it is more advanced auto detects different areas that need different levels of saturation.
- it knows which pixels needs to be tweaked or not. like vibrance doesn't touch skin tone much but saturation slider treats skin tone like any other pixel.

# Hue and Saturation
- you can select individual color to alter thier saturation (master(all), red, green, blue, cyan, magenta, yellow).
    - in the bottom slider select the range of chosen color and add feather using slider to smooth out.
- check 'colorize' to flatten the image into one hue and then adjust its hue/saturation across the image for 1 color only.

# Color balance
- manipulating color only BUT by selecting shadow, highlight or midtone. only on that the color change will occur.
- 'preserve luminosity' checked ensures that lights aren't affected much when you change color and keep them in control.

# Black and white
- convert colorful image into b&w.
- change the vlaues of 'black' and 'white' by adjusting RGBCMY sliders.

# Photo filter
- something to be applied after all the correction, like a camera effect.
- one base color applied to entire image.

# Channel mixer
- select a color from 'output channel' and then this color will be added to R,G or B colors if you move their slider to right and removed from them if you move slider to left.

# Lookup Table (LUTs)
- you can create presets for any color or light adjustment by clicking on top right hamburger icon and saving as preset. saved in default PS folder on pc.
    - this only saves preset for that particular adjustment. ex: preset saved for curves will be only useable on curves adjustment only and obviously only adjusts light.
- LUT or color lookup basically is also a preset but instead of being preset for only 1 type of color adjustment or 1 type of light adjustment, it can be ANY number of color PLUS light adjustments.
    - can be downloaded online and be used to achieve some specific look of a movie on normal footage.
- LUTs are hyper specific usecase. they vary image to image. if you think downloading a LUT will make your image look exactly like something else then thats wrong.

# Dodge and burn tools
- exposure means effect level of brush, range means on what pixels you wanna work.
- then select dodge to add highlights and burn to add shadows.
- use sponge tool to saturate or desaturate.
- you can achieve the same using curves and masks.