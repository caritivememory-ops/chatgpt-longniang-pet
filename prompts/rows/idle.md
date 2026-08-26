Create one horizontal animation strip for Codex pet `chatgpt-longniang`, state `idle`.

Use the attached canonical base for identity. Use the attached layout guide only for slot count, spacing, centering, and padding; do not draw the guide.

Output exactly 6 full-body frames in one left-to-right row on flat pure yellow #FFFF00. Treat the row as 6 invisible equal-width slots: one centered complete pose per slot, evenly spaced, with no overlap, clipping, empty slots, labels, or borders.

Identity: same pet in every frame: Match the supplied character reference closely: one compact full-body chibi anime dragon girl with oversized rounded head and tiny body; very long white hair with pale lavender underside, thick center bangs and one curled ahoge; two pale textured dragon horns; large lavender gradient eyes; pointed ears; an ornate white knot-flower hair ornament with tassels on the reference side; small folded pale-lavender bat-like dragon wings; one large white scaled dragon tail curled tightly beside the body on the reference side; ornate layered white dress with pale lavender shadows, knot ornaments, diamond jewelry and short tassels; rounded hands and small decorated white shoes. Preserve the reference asymmetry and gentle calm expression. Simplify only micro-filigree that cannot read at 192x208. The screenshot white background, black side bars, watermark, all text and all logos are not part of the pet.. Preserve silhouette, face, proportions, markings, palette, material, style, and props.
Style: Pet-safe sprite: compact full-body mascot, readable in a 192x208 cell, clear silhouette, simple face, stable palette/materials, and crisp edges for chroma-key extraction. Style `auto`: Infer the most appropriate pet-safe style from the user request and reference images, then keep that exact style consistent across every row. User style notes: Preserve the supplied 2D chibi anime illustration look: delicate dark-violet linework, clean cel shading with very soft pastel lavender shadows, high-key white-and-lilac palette, polished cute game mascot finish, compact readable silhouette. Do not turn it into pixel art, 3D, plush, painterly realism or a generic western cartoon..
Animation continuity: keep apparent pet scale and baseline stable within the row unless the state itself intentionally changes vertical position, such as `jumping`. Move the pose within the slot instead of redrawing the pet larger or smaller frame to frame.

State action: Calm low-distraction resting loop: subtle breathing, tiny blink, slight head/body bob, and only quiet persona-preserving motion.

State requirements:
- CRITICAL: idle is the low-distraction baseline state and the first frame is also used as the reduced-motion static pet.
- USER REPAIR TARGET: the previous idle loop could lose the lower-right portion in the app. Redraw all 6 frames as complete whole-body poses with the entire large curled tail, its outer scales and tip, the lower-right wing/dress layers, both shoes, all hair ends and every tassel fully present.
- HARD SAFE-AREA GATE: keep every visible sprite pixel comfortably inside each invisible 192x208 slot. Reserve at least about 24 px of clean yellow on the right and bottom of every pose, with similarly generous breathing room elsewhere. Nothing may touch, fade into, or be cut by a slot edge or the outer strip edge.
- Keep the complete silhouette slightly more compact inside the slot if necessary; do not solve padding by deleting, hiding, flattening, or shortening the tail, dress, wing, hair, shoes, or ornaments.
- Use only subtle idle motion: gentle breathing, a tiny blink, a slight head or body bob, a very small material sway, or another quiet motion that fits the pet persona.
- Keep the pet essentially in the same pose, facing direction, silhouette, markings, palette, and prop state across all 6 frames.
- Idle variation must stay calm but still read as animation; do not repeat effectively identical copies across the loop.
- Do not show waving, walking, running, jumping, talking, working, reviewing, emotional reactions, large gestures, item interactions, or new props.
- Feet, base, body, or object anchor should remain planted or nearly planted.
- The first and last frames should be very close visually so the loop feels calm and does not pop.

Clean extraction: crisp opaque edges, extra-safe right and bottom padding, no cropped or missing lower-right anatomy, no scenery, text, guide marks, checkerboard, shadows, glows, motion blur, speed lines, dust, detached effects, stray pixels, or chroma-key colors inside the pet.
