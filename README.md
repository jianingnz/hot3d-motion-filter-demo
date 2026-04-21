# hot3d-motion-filter-demo

Grouped preview for the HOT3D Aria per-object motion filter.

Live: https://jianingnz.github.io/hot3d-motion-filter-demo/

Each card is one source clip (200 random picks from those with at least one
detected moving object). **Left:** the original 150-frame source RGB with
all detected motion windows striped along a bottom bar (one color per
object block) and a corresponding MOVING tag banner on top. **Right:** each
sub-clip of that source with the moving object's 2D track points overlaid
as short decaying trails.

Videos autoplay muted and loop; an IntersectionObserver pauses offscreen
videos so hundreds on the page don't all run simultaneously.

Filter params: threshold = 0.005 m/frame,
min-run = 15 frames, close-kernel = 3 frames.
Aggregate: 2534 sub-clips across
1279 of 1415 source clips.
