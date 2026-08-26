Create Codex v2 pet look row 10 for `chatgpt-longniang` as exactly 8 full-body frames in this order: 180, 202.5, 225, 247.5, 270, 292.5, 315, 337.5.

Use the canonical base, standard contact sheet, layout guide, approved four-cardinal strip, and `qa/look-mechanics.md`. Draw the complete eight-pose row as one coherent animation family, interpolating even 22.5-degree steps between the cardinal pose families. Keep the same pet identity, face construction, materials, palette, markings, and props. Each direction must read correctly at pet size and join continuously at the 000 and 180 boundaries.

DIRECTION TARGETS — use these to shape the coherent row, not as pixel-level landmark gates:

1. `180`: vertical DOWN; no horizontal requirement.
2. `202.5`: horizontal SCREEN-LEFT and vertical DOWN.
3. `225`: horizontal SCREEN-LEFT and vertical DOWN.
4. `247.5`: horizontal SCREEN-LEFT and vertical DOWN.
5. `270`: horizontal SCREEN-LEFT; no vertical requirement.
6. `292.5`: horizontal SCREEN-LEFT and vertical UP.
7. `315`: horizontal SCREEN-LEFT and vertical UP.
8. `337.5`: horizontal SCREEN-LEFT and vertical UP.

Cardinals must be unmistakable. Intermediate poses should broadly occupy the intended quadrant and advance naturally through the ordered loop. Minor pupil, nose, eyelid, or aiming-feature deviations are acceptable when the overall direction, continuity, identity, and motion remain coherent. Do not deform the character merely to make every intermediate axis independently obvious.

LEFT-HALF LANDMARK LOCK: frames 2-8 must never read screen-right. Move the nose/face plane and both complete irises toward SCREEN-LEFT, with progressive screen-left cheek/ear/horn reveal and far screen-right eye/ear/horn/ornament-side occlusion. Make `270` a clear screen-left three-quarter/profile without swapping the ornament. Make `180` unmistakably DOWN using low irises with visible eye-fill above, lowered open lids and a tucked chin.

WRAP-CONTINUITY HARD REPAIR: use a symmetric yaw arc around `270`. Start `180` frontal, increase left yaw evenly through `202.5`, `225`, `247.5`, reach maximum profile only at `270`, then reduce yaw evenly through `292.5`, `315`, and a near-frontal `337.5`. Both eyes and most of the face must be visible at `337.5`; its center, width, area, scale, baseline, horn/tail/wing spread and overall silhouette must nearly match approved `000`. Keep only a subtle screen-left nose/iris cue plus a strong upward eye/chin cue. Never leave `337.5` narrow, side-on, rear-facing, or offset.

HARD LAYOUT AND CONTINUITY CONTRACT — DETERMINISTIC REGISTRATION: draw exactly eight separated pose groups in left-to-right direction order. Keep enough chroma-only space between neighboring poses that each complete pose can be detected without cutting through foreground. Approximate the guide's equal spacing, but do not distort a pose merely to hit an exact source-canvas coordinate; deterministic assembly will crop the eight ordered groups, then apply one shared scale and baseline.

COMPONENT-SEPARATION HARD GATE: leave a clearly visible, uninterrupted full-height pure-yellow corridor between every adjacent pose. No hair strand, horn, wing tip, tassel, dress edge, hand, shoe, or tail scale may enter or bridge these corridors. Keep generous yellow padding at both outer canvas edges. Count eight visually isolated foreground islands before returning.

Use the same body height, head size, baseline, and planted-body position across the generated family. Never overlap neighboring poses, merge two poses into one connected group, crop foreground at the outer canvas edge, or resize one pose independently.

Keep the feet, base, or lower torso planted at the same coordinates across all eight frames. Express direction through the eyes, face, head, upper body, and physically appropriate prop movement, not by moving, rotating, or rescaling the entire sprite.

ROW-BOUNDARY LOCK: 180 must continue directly from row 9's 157.5, matching its body size, baseline, planted anchor, expression, and construction. 337.5 must be one even 22.5-degree step before 000: near-frontal and nearly up-facing, with only a slight screen-left eye/nose cue. Match 000's center, width, area, scale, baseline and overall silhouette closely enough that the wrap looks like one small step.

PRE-RETURN CHECK: reject this result if it does not contain eight separated pose groups in the required order; neighboring poses overlap; foreground is cropped at the outer canvas edge; any frame changes sprite scale, body or head size, baseline, or planted-body position; the row visibly reverses into the wrong half of the loop; 180 does not continue from 157.5; or 337.5 remains side-on/narrow/offset instead of returning near-front to meet 000. Compare 337.5 directly with approved 000: center, width, area, scale, baseline and silhouette must be close.

Use a flat pure yellow #FFFF00 background. One complete unclipped pose per invisible slot. No whole-sprite rotation, replacement eyes, labels, guide marks, shadows, glows, scenery, detached effects, or #FFFF00 colors in the pet.
