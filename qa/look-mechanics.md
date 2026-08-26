# Look mechanics for chatgpt龙娘

## Physical construction and anchor

- Humanoid chibi dragon girl with an oversized but rigidly proportioned head, tiny torso, planted shoes, long layered hair, two rigid horns, pointed ears, small folded wings, a worn knot-flower hair ornament with tassels, and one large scaled tail attached at the hip and curled close to the body.
- Keep the shoes, lower torso, hip, body scale, baseline, and cell registration anchored through all 16 poses. Do not translate, rotate, skew, or affine-tilt the whole sprite to fake a direction.
- Preserve the exact head width, eye spacing, horn roots, face proportions, dress silhouette, ornament anatomy, wing attachment, and tail attachment. The ornament and tail must never swap anatomical sides.

## What leads and follows

- The large lavender eyes lead. Redraw each complete eye surface coherently: iris, pupil, sclera/eye fill, highlight, eyelid rim, and lash line move together inside the original eye aperture. Never paste new googly eyes or slide detached pupils over fixed eyes.
- Eyelids and brows reinforce vertical direction: upper gaze opens the upper eye area and lifts the brow/face attention; downward gaze lowers the upper lid and brings the iris toward the lower aperture without changing eye size.
- The head and neck follow with restrained pitch/yaw. Preserve skull and facial-feature spacing; no soft warp, stretched cheeks, stretched bangs, or changing head size.
- Bangs, side locks, pointed ears, horn overlap, and visible face plane reinforce yaw. The far-side ear/horn/hair is modestly occluded; the near side becomes slightly more visible. Keep the knot-flower ornament physically attached to its canonical hair side.
- Hair tips and tassels lag the head by a small even amount. Folded wings stay attached and follow the upper torso subtly. The coiled tail remains close to the body and may lag a little at the tip, but its hip attachment and overall side remain stable.

## Cardinal pose families in viewer/screen coordinates

- `000 up`: both irises and pupils sit unmistakably in the upper part of the original eye apertures, leaving visible lower sclera/eye-fill beneath them; the whole eye surfaces aim upward, the chin and face pitch slightly up, upper eyelids open/lift and brows support the upward read, and the bangs part or lift subtly. At 192x208 it must read UP without a label, never neutral/front.
- `090 screen-right`: pupils, irises, nose/face plane, head and upper torso turn unmistakably toward the viewer's screen-right edge. The screen-right face side is more visible and the opposite ear/horn/hair side is more occluded. Ornament, wings and tail remain on their canonical anatomical sides.
- `180 down`: both irises and pupils sit unmistakably in the lower part of the original eye apertures, leaving visible upper sclera/eye-fill above them; the chin tucks down, upper lids descend into a clearly lowered gaze, and bangs overlap the forehead/upper-eye area a little more. Keep the eyes open enough to read direction, and keep body scale and feet fixed. At 192x208 it must read DOWN without a label, not sad neutral/front.
- `270 screen-left`: the nose tip and face plane project toward the viewer's SCREEN-LEFT edge; both irises/pupils occupy the screen-left side of their apertures; the screen-left cheek/ear/horn side is revealed while the far screen-right eye, ear, horn and ornament-bearing hair side become partly occluded by nose, bangs and skull. The flower ornament stays on its canonical side and may recede behind the head; it must never swap sides. The coiled tail remains on its canonical body side. At 192x208 this must read LEFT without a label, never front or right.

## Interpolation and motion budget

- Interpolate one continuous clockwise family in even 22.5-degree steps. Each adjacent pose changes eye aim, eyelids, head yaw/pitch, hair overlap, ear/horn visibility, tassel lag, wing follow-through, and tail-tip lag by roughly one equal visual increment.
- Row 9 progresses `000 -> 022.5 -> 045 -> 067.5 -> 090 -> 112.5 -> 135 -> 157.5`; row 10 progresses `180 -> 202.5 -> 225 -> 247.5 -> 270 -> 292.5 -> 315 -> 337.5`, with `157.5 -> 180` and `337.5 -> 000` each exactly one smooth step.
- Diagonals must visibly contain both required axes. Up-right and up-left retain clear upward eye/head pitch plus the correct horizontal yaw; down-right and down-left retain clear downward eye/head pitch plus the correct horizontal yaw.
- Avoid sudden changes in head size, eye design, body position, wing opening, tail curl, ornament position, dress shape, or silhouette width. No whole-body rocking, no pose mirroring, no independent per-cell restyling, no new props, labels, clocks, arrows, degree text, shadows, glows, scenery, or detached effects.
