# Cleanup
Adobe Illustrator script to clean up vector data prior to laser cutting.

# Changelog

V2.2:
- Fixed duplicates being moved but not recoloured (happened with lines pulled out of compound paths, and with zero/hairline strokes).

V2.1:
- Partial overlaps.
- Lines that share a stretch of at least 1 mm (but where neither fully covers the other) are marked on the "duplicates" layer with a thick yellow copy of the shared stretch + a dashed yellow circle, grouped and named "Overlap 1", "Overlap 2"... The original lines are untouched.
- Items already on the "duplicates" layer are ignored, so re-running the script never treats its own markers as artwork.

# v2.0:
Tolerant duplicate detection (0.05 mm), short-on-long lines, direction/start point independent, compound path fixes.

# v1.4:
Speck detection uses bounding box diagonal as well as area.
