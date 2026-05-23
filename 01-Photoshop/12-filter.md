# convert to smart object before applying any filter
- later on if you want to edit the filter settings using saved info of original image.

# Camera Raw
- theory:
    - raw has more data and whatever adjustment you make on that vast data, the finer details are retained. whereas in jpg the data in compressed so less data to work with and finer details are lost can't be brought back.
    - RAW = sensor captured much more light/color information → edits have more “room” before image quality breaks.
    - JPG = camera already compressed + processed the image → some information is permanently discarded.
    - RAW does NOT automatically look better. It simply gives you more editing flexibility before degradation happens.
    - ex: Suppose sky pixels in JPG are already pure white (255,255,255) hat means no cloud detail exists anymore, In RAW maybe sensor captured (248,250,252) Camera only clipped it during JPG conversion. Now RAW editor can recover cloud texture.
    - RAW = more editable information
    - JPG = less editable information
    - Camera Raw filter = convenient adjustment workspace (sliders, all-in-one adjustment instead of layers upon layers, etc.)
- press alt to reset and click on any adjustment to reset.
- first handle the white balance.
    - White balance is the process of adjusting the colors in a photo, so that objects appearing white in person are rendered white in your image.
    - the camera sensor just collects data, the camera processor was supposed to think what is white and not in the image, but since we are not using the processed/compressed image and instead using raw image data, we have to use your own processing unit (brain) to tell what is white.
- texture = detailing in an image (like on skin), works smartly on skin-like area and not on overall lights. (highlight)
- clarity = just like texture but works on overall contrast. (midtones)
- dehaze = drastically change the darks and lights. (shadow)

# Liquify
- used mostly for changing body shape/parts.
- brush:
    - set pressure and density around 30-40 and take a slight bigger brush size then work in iterations.
    - pressure is the force you apply on mop/brush.
    - density is the area of effect of mop/brush.
- forward warp to make the changes (most used), then reconstruct tool to revert those changes.
- after the above tools few zig-zag pattern may appear to make that uniform use smoothing tool.
- use warp tool to tilt forward (click) or backward (alt + click).
- bucker and bloat expands or shrinks from center.