# Case evidence

This is an unofficial synthesis of a recurring method found in 7 published Cases attributed to vib3coded. It is not an official Skill from that creator.

## Operating rule

Choose one evidence card below as the anchor before drafting. Inspect its finished media, then state which traits will be preserved, replaced, and avoided. A title match alone is not evidence.

### E1 · 浮空岛后院的像素风四格足球游戏

- Creator: @vib3coded
- Evidence: [GoodCase](https://goodcase.ai/cases/build-a-single-file-html-three-js-r160-scene-called-chalk-square-four-sq-38d0013dce1c) · [finished media](https://media.goodcase.ai/cases/94d4992041e8.mp4) · [poster](https://media.goodcase.ai/cases/2c807caf7392.jpg) · [original source](https://x.com/vib3coded/status/2113602050172785117)
- Summary: Garages, chalk and one ball for the whole yard ⚽ Claude Opus 5.5 vs. GPT-6 Astra - same prompt: build a 3D backyard with pixel-art rendering and a game of four …
- Prompt excerpt:

> PROMPT:
> Build a single-file HTML + three.js (r160) scene called "Chalk Square": four square played with a football in a back yard on a floating island. It is a real 3D scene rendered as crisp pixel art.
>
> Rendering: an orthographic isometric camera (drag to turn in 90° steps, scroll or pinch to zoom). Render into a small low-res target with a depth texture, then upscale with texelFetch to whole screen pixels. Add depth-based outlines and quantize every pixel to a fixed ~60-colour palette in OKLab, with an optional Bayer dither. Toggle "Pixel art / Raw 3D", with a pixel-size slider and Palette / Dither / Outlines checkboxes.
>
> Yard: patched, cracked asphalt with a kerb, grass and dirt around the island edge. Around the asphalt:
> - a row of lock-up garages with painted, numbered doors and a flat roof that overhangs them;
> - a brick transformer booth with a warning sign;
> - a poplar with a bench and a grandmother on it;
> - a chin-up bar, a carpet rack with a rug, bushes;
> - a lamp on a pole and a lamp over a garage door.
> Pigeons walk and peck, and flap up onto the roofs when the ball or a kid comes near. A cat on the garage roof follows the ball with its head.
>
> Chalk: a data texture over the asphalt. It holds the 4.8 m square split into four zones (King, Queen, Jack, Dunce) with letters and a crown, plus hopscotch and doodles. Each texel stores its order along its stroke, so the lines can be redrawn progressively.
>
> Game (8 kids, each with a skill, power and style: power / trick / safe / lob):
> - Four kids play, four wait in a queue. The King serves by dropping the ball and kicking it…

### E2 · 果冻方块中的山谷水坝微缩景观

- Creator: @vib3coded
- Evidence: [GoodCase](https://goodcase.ai/cases/build-dam-jelly-a-new-piece-in-my-material-studies-series-a-single-file-5b1975110a6a) · [finished media](https://media.goodcase.ai/cases/5f953c611a8c.mp4) · [poster](https://media.goodcase.ai/cases/c1a6873814ff.jpg) · [original source](https://x.com/vib3coded/status/2114512807500615723)
- Summary: Claude Opus 5.5 built this jelly dam for 18.51$ A single HTML file using pure WebGPU, with no libraries. Waves follow a shallow-water model, reservoir levels re…
- Prompt excerpt:

> PROMPT:
> Build "Dam Jelly", a new piece in my "Material Studies" series: a single-file, self-contained interactive WebGPU diorama (one HTML file, all JS/CSS/WGSL inline, no network requests, no libraries). A mountain valley with a concrete gravity dam is cut out as a wobbly block of jelly sitting on a pale studio table, seen from above at three-quarters.
>
> SCENE (block-local coords, origin at base centre, y up, block ~5.2 × 5.2 units):
> - A river valley running back to front: steep rocky slopes with crags, scree and boulders, conifer and broadleaf woods, grassy shoulders. Where the block is cut, the side faces show layered grey bedrock in tilted beds with joints, a weathered brown band and dark topsoil at the top, and gravel and silt under the water. At the very bottom are thin coloured "jelly" strata in the current flavour.
> - A long reservoir behind the dam, with a bare drawdown ring of rock round its shore, a floating log boom of orange and yellow floats in front of the spillway, and a small patrol boat lapping the lake.
> - A concrete gravity dam across the valley, its ends let into rock abutments: a battered downstream face with lift lines, a crest road with railings and lamps, an intake tower with trash racks and three penstocks down the face.
> - A central stepped spillway with three bays between piers. Each bay has a radial (Tainter) gate: a curved skin plate on arms that swing about trunnions on the piers, with hoist houses on top. Below is an ogee crest, a stepped chute, training walls and a plunge pool scoured into the riverbed.
> - A powerhouse at the right toe: a concret…

### E3 · 黄昏像素风潜艇鱼雷猎杀航母

- Creator: @vib3coded
- Evidence: [GoodCase](https://goodcase.ai/cases/claude-fable-5-2-build-dusk-depths-a-submarine-hunting-game-as-one-self-contained-html-file-3d722758f907) · [finished media](https://media.goodcase.ai/cases/3f25454d90a9.mp4) · [poster](https://media.goodcase.ai/cases/8aea579a3579.jpg) · [original source](https://x.com/vib3coded/status/2123825494567026938)
- Summary: How the hell did Claude Fable 5.2 fit an entire submarine game into 190 KB?! 😭 You spot an aircraft carrier through the periscope, fire a torpedo, and watch it…
- Prompt excerpt:

> PROMPT
>
> Build "Dusk Depths", a submarine hunting game, as one self-contained HTML file: WebGL2, no engine, no libraries, no image or audio assets (Google Fonts only). Everything is procedural. All in-game text in English.
>
> LOOK
> Pixel art at dusk: render at about 540 rows and upscale with nearest-neighbour, 4x4 Bayer dithering, a limited palette (pink-orange sky, violet-blue sea), flat 3-tone shading on meshes and a 1-2 px dark outline in a post pass. Ray-march the sea surface, the sea bed (tiling height field, 20-250 m deep) and the sky in one fragment shader, above and below water: swell and sun glitter on top; light shafts, caustics, fish, weed and coral below. Draw the HUD on a separate Canvas 2D layer with its own pixel grid and a 3x5 pixel font.
>
> SHIPS
> Model in code, with real detail: an aircraft carrier (angled deck, island, parked jets, hull number), destroyers, a cruiser, a fleet oiler, a helicopter with dipping sonar, and the player's attack submarine. Add plating seams, rust streaks, lit portholes, bow foam and wakes.
>
> GAMEPLAY
> The player hunts a carrier group that zig-zags across the sea. Stealth matters: noise grows with speed, a thermal layer at 95 m hides the boat, escorts ping, hunt and drop depth charges, the helicopter dips its sonar. Lock a target, wait for the firing solution, fire torpedoes (4 tubes, 9 s reload); decoys and an active ping are available. Score is tonnage sunk; each new group is stronger.
>
> TORPEDOES
> A torpedo leaves exactly along the aim: on the bearing of the locked target, otherwise where the periscope or camera points. It homes by pure…

### E4 · 云海巨龟背上的灯塔秋岛与环游鲸鱼

- Creator: @vib3coded
- Evidence: [GoodCase](https://goodcase.ai/cases/claude-opus-5-5-create-a-single-self-contained-html-file-using-three-js-that-renders-a-beautifu-90da86c412f0) · [finished media](https://media.goodcase.ai/cases/dd05b98c2ecc.mp4) · [poster](https://media.goodcase.ai/cases/46d395f3e026.jpg) · [original source](https://x.com/vib3coded/status/2116169391301607810)
- Summary: Claude Opus 5.5: first attempt → final result in 21 minutes 🐢🐋 A tiny world on the back of a flying turtle. Autumn trees, a lighthouse, a waterfall pouring in…
- Prompt excerpt:

> PROMPT
>
> Create a single self-contained HTML file using Three.js that renders a beautiful animated voxel-art 3D scene. A floating island rests on the shell of a giant sea turtle that slowly swims through the clouds in a golden-hour sky.
>
> On the island: a red-and-white striped lighthouse on a hill with a glowing lantern and a rotating light beam, a keeper's cottage with a smoking chimney, autumn trees (orange, gold, red) and dark pines, a pond with a rowboat, a stream that runs down the shell and spills off as a waterfall, flowers, rocks, pumpkins and lamp posts along a path.
>
> The turtle has a patterned shell with scutes, a scaly head and flippers that paddle slowly; the island gently bobs with each stroke. A huge voxel humpback whale with glowing spots rises from the clouds below and swims in a spiral around the island, leaving a trail of sparkles. Seagulls circle the lighthouse.
>
> Add soft shadows, voxel ambient occlusion, drifting voxel clouds, falling leaves, a gradient sky and a slow cinematic camera orbit. Make it as detailed and polished as possible.

### E5 · 极光雪夜中猛犸背负冰堡，冰龙环绕云海

- Creator: @vib3coded
- Evidence: [GoodCase](https://goodcase.ai/cases/claude-opus-5-5-create-a-single-self-contained-html-file-using-three-js-that-renders-a-beautifu-c5134ae05b62) · [finished media](https://media.goodcase.ai/cases/18a08e7a5172.mp4) · [poster](https://media.goodcase.ai/cases/4ba247ce5ecf.jpg) · [original source](https://x.com/vib3coded/status/2116533061495947270)
- Summary: Opus 5.5 built this in 25 min for $0.75: a frost fortress riding a woolly mammoth across the clouds, ice dragon included 🐉🦣 1st attempt vs final. One HTML fil…
- Prompt excerpt:

> PROMPT
>
> Create a single self-contained HTML file using Three.js that renders a beautiful animated voxel-art 3D scene. A giant woolly mammoth walks across a sea of clouds through a snowy night with the northern lights and a moon; the clouds drift backwards under its feet, and snow puffs up at every step.
>
> On its back, over a blue blanket with gold trim and leather straps, stands a stone frost fortress: walls with battlements, four round turrets with blue conical roofs and flags, two small houses with glowing windows and smoking chimneys, and a central keep with a big glowing ice crystal floating and slowly rotating above it. The mammoth has shaggy fur, a swaying trunk, long curved tusks and snow on its head.
>
> A crystalline ice dragon with horns, ice spikes along its back, glowing eyes and large wings rises from the clouds and circles the mammoth, leaving a trail of snowflakes, and breathes frost twice.
>
> Add soft shadows, voxel ambient occlusion, a snowstorm, drifting voxel clouds and a slow cinematic camera orbit. Make it as detailed and polished as possible.

### E6 · 雪原上行进的帝国AT-AT步行机

- Creator: @vib3coded
- Evidence: [GoodCase](https://goodcase.ai/cases/gpt-6-2-astra-build-an-interactive-3d-scene-of-an-imperial-at-at-walking-across-hoth-from-the-7bd6b331e4bd) · [finished media](https://media.goodcase.ai/cases/c12aedeba043.mp4) · [poster](https://media.goodcase.ai/cases/470953f3976f.jpg) · [original source](https://x.com/vib3coded/status/2124327889776640303)
- Summary: Why is everyone still using Blender for AI-generated 3D when Three.js exists? I gave GPT-6.2 Astra the same task twice on XHigh: build a walking AT-AT Three.js …
- Prompt excerpt:

> PROMPT
>
> Build an interactive 3D scene of an Imperial AT-AT walking across Hoth from The Empire Strikes Back. Use HTML5, CSS, and JavaScript with Three.js r160. Render the scene on a full-window <canvas> using THREE.WebGLRenderer and WebGL 2. Deliver one standalone .html file with Three.js, scene code, geometry, and textures embedded. It must open directly from disk and work offline.
>
> Model the AT-AT in Three.js using custom BufferGeometry for its distinctive shapes. Follow the original 1980 filming miniature closely, especially the sloping hull, ribbed neck, narrow cockpit visor, paired chin cannons, circular knee joints, curved ankle forks, and broad four-pad feet. Use physically based materials, baked ambient occlusion, and layered textures. Up close, the viewer should see chipped enamel on hatch edges, grime below vents, and polished metal on moving pistons.
>
> Animate the walker with requestAnimationFrame, delta-time updates, and inverse kinematics. Keep each supporting foot anchored in world space while the hull moves past it. Shift the body’s weight before lifting the next leg. Use GLSL shaders for the snow surface and compressed tread marks, and particles for the powder displaced at touchdown. Each footprint should match the sole that made it and stay in place as the walker advances.
>
> Open with a low three-quarter tracking shot. Frame the entire lead walker against distant mountain ridges, with two more AT-ATs in the haze, snowtroopers near its feet, and two Rebel T-47 snowspeeders banking across the glacier. Light the scene with cold daylight and a warm break in the c…

### E7 · 暮色灯港里青斗篷旅人走过倒影水面

- Creator: @vib3coded
- Evidence: [GoodCase](https://goodcase.ai/cases/gpt-6-2-astra-build-lantern-harbor-a-third-person-exploration-game-in-three-js-185383664b6e) · [finished media](https://media.goodcase.ai/cases/3cec25771a89.mp4) · [poster](https://media.goodcase.ai/cases/1f78bbd80075.jpg) · [original source](https://x.com/vib3coded/status/2123907432334217548)
- Summary: Why does GPT-6.2 Astra get so much hate? Just look at what it built in 22 minutes for $15.78 I bet the people talking the most trash haven’t even tried building…
- Prompt excerpt:

> PROMPT
> Build Lantern Harbor, a third-person exploration game in Three.js. Deliver it as one standalone HTML file that opens directly in a browser and works offline. Embed the library, shaders, textures, and audio.
>
> Open behind a small traveler in an embroidered teal cloak and a long coral scarf. Ahead, a lantern keeper’s cottage stands on wooden stilts. Frame the cottage on the left and a huge pale moon on the right, with room to see both reflected in the sea. Paint the sky in dusty rose, warm peach, and deep violet.
>
> Make the water the most memorable part of the game. When the traveler stands still, the sea should be calm enough to count the lit windows in the cottage’s reflection. When they run, each bootfall sends out a ring that bends the reflected clouds, expands, and fades. Give landings a wider ripple and the fishing boat a narrow wake. Use real-time planar reflections so everything lines up as the camera turns.
>
> Across the water, build a small village on two rocky islands. Give each house a silhouette you can recognize from shore: a red fishing loft with a carved gable and hanging nets, a sage-green sailmaker’s workshop with a half-finished sail visible through the window, and a chartmaker’s house with a copper turret. Connect the islands with a wooden footbridge.
>
> Give the player one clear task. Climb the cottage steps and light the beacon. Look out across the harbor for a fishing boat flashing its lamp. Approach it, signal the skipper with your lantern, and guide the boat home. If you get too far ahead, the skipper should wait. When you reach the berth together, l…

## Evidence index

| Case | Creator | GoodCase evidence | Finished media | Original source | Card |
| --- | --- | --- | --- | --- | --- |
| 浮空岛后院的像素风四格足球游戏 | @vib3coded | [GoodCase](https://goodcase.ai/cases/build-a-single-file-html-three-js-r160-scene-called-chalk-square-four-sq-38d0013dce1c) | [Media](https://media.goodcase.ai/cases/94d4992041e8.mp4) | [Original](https://x.com/vib3coded/status/2113602050172785117) | E1 |
| 果冻方块中的山谷水坝微缩景观 | @vib3coded | [GoodCase](https://goodcase.ai/cases/build-dam-jelly-a-new-piece-in-my-material-studies-series-a-single-file-5b1975110a6a) | [Media](https://media.goodcase.ai/cases/5f953c611a8c.mp4) | [Original](https://x.com/vib3coded/status/2114512807500615723) | E2 |
| 黄昏像素风潜艇鱼雷猎杀航母 | @vib3coded | [GoodCase](https://goodcase.ai/cases/claude-fable-5-2-build-dusk-depths-a-submarine-hunting-game-as-one-self-contained-html-file-3d722758f907) | [Media](https://media.goodcase.ai/cases/3f25454d90a9.mp4) | [Original](https://x.com/vib3coded/status/2123825494567026938) | E3 |
| 云海巨龟背上的灯塔秋岛与环游鲸鱼 | @vib3coded | [GoodCase](https://goodcase.ai/cases/claude-opus-5-5-create-a-single-self-contained-html-file-using-three-js-that-renders-a-beautifu-90da86c412f0) | [Media](https://media.goodcase.ai/cases/dd05b98c2ecc.mp4) | [Original](https://x.com/vib3coded/status/2116169391301607810) | E4 |
| 极光雪夜中猛犸背负冰堡，冰龙环绕云海 | @vib3coded | [GoodCase](https://goodcase.ai/cases/claude-opus-5-5-create-a-single-self-contained-html-file-using-three-js-that-renders-a-beautifu-c5134ae05b62) | [Media](https://media.goodcase.ai/cases/18a08e7a5172.mp4) | [Original](https://x.com/vib3coded/status/2116533061495947270) | E5 |
| 雪原上行进的帝国AT-AT步行机 | @vib3coded | [GoodCase](https://goodcase.ai/cases/gpt-6-2-astra-build-an-interactive-3d-scene-of-an-imperial-at-at-walking-across-hoth-from-the-7bd6b331e4bd) | [Media](https://media.goodcase.ai/cases/c12aedeba043.mp4) | [Original](https://x.com/vib3coded/status/2124327889776640303) | E6 |
| 暮色灯港里青斗篷旅人走过倒影水面 | @vib3coded | [GoodCase](https://goodcase.ai/cases/gpt-6-2-astra-build-lantern-harbor-a-third-person-exploration-game-in-three-js-185383664b6e) | [Media](https://media.goodcase.ai/cases/3cec25771a89.mp4) | [Original](https://x.com/vib3coded/status/2123907432334217548) | E7 |

## Derivation boundary

- Inclusion means the published Case matched the method pattern; it does not prove the creator used this exact synthesized workflow.
- Popularity is not part of the Skill threshold.
- Treat GoodCase summaries as editorial evidence and the linked original source as primary evidence.
