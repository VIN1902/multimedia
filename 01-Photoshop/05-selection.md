# Selection
- to work upon selected area of layer only. (paint, effect, etc.)
- first click which layer you want to make selection from.
- then click which layer you want to use that previously made selection.
- `ctrl + D` for deselect. `ctrl + shift + I` for inversing the selection.
- `ctrl + left-click` on the layer icon in panel to select the pixels of a layer. if layer is fully pixeled then full layer will be selected.
- after selection you can right click in the area to acess more options, layer-via-copy/via-cut makes new layers out of the selected pixels.

# Tools

## Marquee tool
- selection out of basic shapes.
- press `shift` to maintain ratio.
- press `spacebar` while selecting to move the selection.
- use add, subtract & intersect options.

## Lasso tool
- for free-hand selections, just click-hold and drag mouse.
- polygon-lasso just keep clicking and use backspace to remove points and enter to connect.
- magnetic-lasso just click once and then move mouse along the edge of subject. backspace/enter works plus add,sub,intersect works too here.
    - only issue with mag-lasso is the image needs to have very clear pixel edge seperation, even if there's slight lighting blend it won't work.

## Object selection tool
- can choose b/w lasso or rect mode.
- just draw selection around the object and ai handles the job.

## quick selection tool
- paint the selection rought using a brush.
    - brush size with `[ & ]` and subtract brush with `alt` key hold.
- usefull for minute operations.

## Magic wand tool
- tolerence controls the color range of what will be selected upon click.
    - if its 1 then only the colors at the pixel you clicked will be selcted.
- contiguous controls that if checked then only 1 object with that color will be selected otherwise all the objects with that color will be selected.

## Pen tool
- for path, shapes and selection.
- `P` to select pen tool. hold `shift` to make straight lines at a fixed angle.
- `ctrl` to move and select the anchor points.
- hold and drag the mouse to curve it and introduce two handles.
    - `ctrl` to move handles.
    - `alt` to break the handles and move them individually.
    - the left handle controls curve of left line and right handle controls curve of right line.
- `alt`and click on an achor point to switch b/w linear and curve. 

# Feather
- right click selection and set feather for smoothnes of selection border.

# Expand/Shrink
- select > modify > expand/shrink.
- used for modifying the selection boundary by a few pixels.

# Masks
- just like blending we aim to control transparency with masks, but instead of brightness basis we self paint either black or white to choose which part of the layer to hide or show respectively.
- used for non-destructive editing.
    - you don't work directly on source image but on another layer.
- select something and instead of operating directly on that selection we make a mask first.
- use brush tool to adjust the mask (black/white) to hide/reveal parts of source image. whatever happens on mask doesn't directly apply on source.
- `alt + click` on mask in layer panel shows the mask in main screen.
- `shift + click` on mask in layer panel temporarily hides the mask.

# Refine Edge
- used to refine edges of soft subject like hair which is not possible by normal selection tools.
- select image, select quick select tool, go to 'layer and mask' option to go into new panel/window.
- in this window first refine tool use then maybe contrast/feather n all and then export as new layer with mask.
- double click on the mask in layer panel to back to that window and at bottom before export click 'decontaminize' then export, view both the mask layers.
