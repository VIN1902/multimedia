# Blend Mode
- Darken = hiddes the lighter parts of the layer.
- Lighten = hiddes the darker parts of the layer.
- create tones for images by blending solid or gradient layers to background.
 
# Shortcuts
- `ctrl + j` for duplicate layer.
- `ctrl + g`for grouping selected layers.

# Layer styles

- layer style > blending options > blend if:
    - automatically hides or reveals parts of a layer based on brightness or color channels.
    - Current Layer:
        - Dragging the Dark/Shadows (left) slider right makes the dark parts transparent (remove).
        - Dragging the Light/Highlights (right) slider left makes the bright parts transparent.
    - Underlying Layer: Controls how the layers beneath your current layer peek through.
        - Dragging the Dark/Shadows (left) slider right lets the darks of the underlying layer show through your current layer.
        - Dragging the Light/Highlights (right) slider left lets the brights of the underlying layer show through.
    - use `alt` to smooth out the effect's edge/fade.

# Opacity vs Fill
- both control the transparency of layer.
- opacity effects the entire layer (the main object and all effects applied on it).
- fill effects only the main object of layer and doesn't control the transparency of any of its effects.

# Layer types
- Raster Layer
    - shown my no symbol.
    - the image data is in hard-coded pixel values. (no. of pixels used, rgb value of each pixel, etc.)
    - when you resize the image (change the pixel data) then the original pixel value is forever lost. any further resizing refers (or starts from) the previous updated data and not the original data.
    - so this results in image getting pixalated each time the pixel data is changed.
- Vector Layer
    - shown my symbol of square shape.
    - the image data is not hard-coded pixels, instead it is dynamically calculated mathematicaly. A math equation is stored instead of the pixel values.
    - when you resize the image each time the image is recalculated based on the stored formula and shown with 0 data loss based on any screen size.
    - but the image file size can shoot up a lot and can take a lot of space.
- Smart Object Layer
    - shown my symbol of a file maybe.
    - Adobe's solution to reach somewhat of a middle ground b/w raster and vector.
    - the raster image's pixel data is stored in a file that persists in the software itself.
    - any resizing starts from this saved state of pixel data and not from the previous state.
    - this leads to achieving a 'vector-like' effect even though the image is not vector.

# Bakcground/Foreground color
- `D` for defualt values (black and white).
- `X` for switching b/w chosen foreground and background colors.
- `alt + backspace` for applying foreground color to entire layer.
- `ctlr + backspace` for applying background color to entire layer.
- for a smaller layer on top of main layer, to do all the above operations withing that confined area of that layer:
    - make the layer a selection by `ctrl + lmb` on the layer in layers panel.
    - check the 'lock transparent pixels' icon.

# Pattern
- Edit > fill > pattern gives more options than pattern panel.
- to make own pattern make a square selection and then edit > define pattern.

# Merge layers
- `ctrl + alt + shift + E` for making a seperate merged layer of all the layers.
- right click and merge down for merging 1by1. or `ctrl + alt + E`.

