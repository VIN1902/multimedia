# Tools

1. Move
- auto-select on means you don't need to manage layer selection. Stuff will get auto selected based on cursor position which you want to move.
- in the options for alignment the selected layers align among themselves. if want to align them relative to background then select background too along with those layers.

2. zoom
- workflow:
    - from any tool use `ctrl + space` and turn off scrubby zoom  for this. then just select area on which to zoom.
    - zoom to fit by pressing `ctrl + 0`.
    - or just use `alt + scroll wheel` for random zoom.

3. pan
- use `space` from any tool to pan over the canvas retaining the zoom level.

4. transform
- `ctrl + T` for free transform and then press enter when done.

5. erase
- mostly useless we use masks instead.
- but 'erase to history' option checked erases all the work done to bring back original layer.
    - if you use file > revert then all the layers you added (expect the very first one) are gone too. but with erase to history you can revert a single layer back to original
- background erase tool: the crosshair samples the pixel data and circle delets that sampled pixel everywhere.