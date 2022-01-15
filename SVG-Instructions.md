Requires Inkscape.

The half-hexagon in the background is for ensuring alignment by snapping nodes and handles to it. Inner borders are made entirely out of Live Path Effects that copy and transform the outer borders. The blur on the inner segments, and any other filters, are shared.

To edit the line thickness or opacity, you can just select the inner and outer segments, then use the [Object]→[Fill and Stroke…] dialog normally.

To edit the border shape, it's recommended to edit the nodes of the outer border paths, without moving or editing anything as objects. The LPEs will automatically update the inner border segments with any changes to the outer border paths. This helps keep the LPEs and alignment in sync.

To move an inner segment:

1. Select the inner segment curve.
2. Open the [Path]→[Path Effects…] editor.
3. Select the "Offset" effect and change its "Offset" parameter. Do not move the segment on the canvas in any other way; The inner segments are live clones of the outer segments, so keeping their offset in a path effect makes sure they're all aligned and makes them  automatically update if you edit the outer segment shapes.
4. Set the same offset for the other three inner segment curves.

To edit the inner blur amount:

1. Select any one of the blurred segments.
2. Go to [Filters]→[Filter Editor…].
3. Make sure the filter named "Blur" is selected, and edit the "Standard Deviation" parameters of the "Gaussian Blur" effect. Don't use the Fill and Stroke dialog; It may also work but all the blurred segments share the same blur filter.

To export:

1. Hold down [Shift] and click on the _background_ behind each border segment. Do not select the border curves themselves.
2. Once you've selected all eight backgrounds, open the [Object]→[Fill and Stroke…] editor. Set the opacity to 1%. 0% also works, but you may not be able to select them again.
3. Go to [File]→[Export PNG Image…].
4. Make sure "Export area" is set to "Selection".
5. Turn on "Batch export 8 selected objects".
6. Do not change any other settings; The filenames are already set per border segment.
7. Press "Export". Correctly named border segments should now be created in the same folder as the .SVG file. (Note that this will also overwrite existing named border segments.)
8. Without saving, close the window and restart Inkscape, or revert the file. I've noticed the Export dialog may behave inconsistently after doing a batch export.

Most of the dialogs have keyboard shortcuts that are faster to use.

