# Cleanup
Adobe Illustrator script to clean up vector data prior to laser cutting.

# Changelog

# v2.3:
- Speck removal now only touches cuts (exact green 0,255,0 or pink 255,0,255 strokes, including global/CC library swatches).
- Tiny engraving, marking, scoring and perforation bits are kept, and counted in the alert as "Tiny Non-Cut Items Kept".
- Paths with 0–1 anchor points are still deleted whatever their colour.

# v2.2:
- Fixed duplicates being moved but not recoloured (happened with lines pulled out of compound paths, and with zero/hairline strokes).

# v2.1:
- Partial overlaps.
- Lines that share a stretch of at least 1 mm (but where neither fully covers the other) are marked on the "duplicates" layer with a thick yellow copy of the shared stretch + a dashed yellow circle, grouped and named "Overlap 1", "Overlap 2"... The original lines are untouched.
- Items already on the "duplicates" layer are ignored, so re-running the script never treats its own markers as artwork.

# v2.0:
Tolerant duplicate detection (0.05 mm), short-on-long lines, direction/start point independent, compound path fixes.

# v1.4:
Speck detection uses bounding box diagonal as well as area.
