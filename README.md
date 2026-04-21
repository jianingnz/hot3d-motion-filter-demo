# hot3d-motion-filter-demo

Static preview for the HOT3D Aria per-object motion filter.

See the live page: https://jianingnz.github.io/hot3d-motion-filter-demo/

## What this shows

For a handful of source clips from the HOT3D Aria RGB + tracks dataset, each
card displays:

- **Left:** median per-point displacement (m/frame) for each object block,
  with the motion threshold dashed and *kept* motion windows shaded red.
- **Right:** the source video with 2D track points drawn only while an object
  is inside a kept window.

Filter params used for this preview:

- threshold = 0.008 m/frame (≈ 24 cm/s @ 30 fps)
- min contiguous-motion run = 15 frames
- morphological close kernel = 3 frames
- Skip any object block that is never visible in the clip.
- Skip any motion window that has no visible frame.

Aggregate: detected 1,986 sub-clips across 1,136 of 1,415 source clips.
