# hot3d-motion-filter-demo

Static preview for the HOT3D Aria per-object motion filter.

Live: https://jianingnz.github.io/hot3d-motion-filter-demo/

Each card shows, for one detected sub-clip:
- **Original RGB** (full 150-frame source video, motion window highlighted).
- **Sub-clip** (trimmed to the motion window).
- **Sub-clip + 2D tracks** (the subject object's 2D track points overlaid with
  short decaying trails; 120 points subsampled from the 2,000 per-object points).

Filter params: threshold = 0.005 m/frame,
min-run = 15 frames, close-kernel = 3 frames.
Aggregate: 2534 sub-clips across
1279 of 1415 source clips.
