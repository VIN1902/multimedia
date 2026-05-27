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

# Blur
- Blur: removes all the details/texture, mixes the general colors together.
- blur tool is used for small cases such as smoothing hard edges of a cut-out.
- sharpen tool does opposite of blur but still for small tasks.
- workflow: duplicate -> smart object -> select and mask the subject + background -> filter > blur > guassian blur.
    - adjustment and filters from menu on raster permanently changes the pixels, so we first convert it to smart object.
    - for heavy bluring and background work we don't use the tool instead use filter menu.
    - if you want to make a new background w/o the subject then select the general area of subject then edit > fill > content-aware.
- lens blur only works on raster image. select and maske after duplicating.
    - the thing in focus of camera will be in black and thing to be blurred by camera, out of focus, will be in white. (concept of depth map)
    - blur focus distance is for bluring on in-focus subject.
    - radius is for bluring out-of-focus subject.
    - specular highlights add bokeh effect. When out of focus brightest point are made more brighter and defined into geometrical shapes like circles/hexagon.
- motion blur after applying it whole image, create duplicate select & mask the subject and inverse the mask then paint it for better effect.
- smart blur is like guassian but we have control over edges whether to blur them or not.
- check out blur galler from filters.

# Distort
- displace: depth of texture layer carries over to top layer, not just simple blending.
    - the texture layer should be first made black and white using adjustment, for making a displacement map. then saved alone as a psd file.
    - then in new file add texture layer image + top layer image and do regular blending.
    - then select top layer, convert to smart object and go to filter > distort > displace, then chose the earlier saved psd.
    - blending: normal blend options in layer panel -> blend if -> distor > displace.
- pinch: sort of like bevel and imboss. if you want the top layer to blend following the curvatur of below layer.
- polar coordinate: covert a straight (rectangular) image into round (polar) and vica-versa. 
    - anything above the straight pixels will go inside the circle.
    - anything below the straight pixels will go outside the circle.
    - the canvas should be sqaure dimensions for perfect circle or else it will be oval.