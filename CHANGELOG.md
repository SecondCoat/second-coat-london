# Changelog

## 0.1.8

### New
- Volumetric clouds under the High lighting: a deck of real cumulus that
  drifts with the sky's own cloud layers, gathers a minute before rain and
  clears over the two minutes after it. A Clouds setting picks them, a
  faster version of them or the flat layers.
- A full moon in the High night sky, behind the clouds.
- Rain, much wetter:
  - Puddles form where a street holds water: in the gutters at the foot of
    the kerbs, in dips, between the cobbles before over their tops. They
    have a depth and a murky bottom, fill in a minute and a half and take
    ten minutes to dry, after the rest of the street.
  - Wet streets read as a sheen with highlights and glints, the grit of
    the asphalt catching the light, and dry in patches: the sunlit side
    and the crown first, gutters and shade last.
  - Drops beat on the pools and the soaked street; wet materials darken
    as they really do; facades facing the rain soak and streak.
  - Water drips from awnings, balconies, eaves and cars; a heavy downpour
    hangs a mist of splashes over the street and draws the fog in.
  - Wet cars bead up and pick up the road's grime on their lower body.
- Snow keeps the traffic's ruts far down the street, not just near you.
- The hedges behind London's railings are real bushes, and keep the view
  closed in every season.
- Cars knock down police officers and mission characters on foot as they
  do pedestrians: they get up again, or die from a hard enough hit.
- The mouse pointer hides while you play with a gamepad.
- The Mods tab shows each mod's version.

### Changed
- The High graphics preset grows its trees with lighter hedges (Generated
  fast), for frame rate.
- Characters and cars collide with the rooms and stairwells they walk and
  drive through as the original does, room by room.

### Fixed
- The brothel mission (Frank):
  - The street's facade no longer stands across the corridors and the hall.
  - The back stair no longer stops you at its foot.
  - On the ledges over the collapsed floor, turning the camera no longer
    pulls you out of cover and fails the mission.
  - The police no longer shoot the disarmed Jake: they arrest him, and the
    mission completes.
  - People in the street by the doorway are no longer lit by the light
    inside.
- The van chase to Snow Hill no longer fails ("YOU LOST THE VAN!") while
  the van is still in sight, before you have rammed it.
- The skips with planks are ramps again, as in the original: cars drive up
  them and jump off.
- Bodies slide off cars and can be driven over, instead of being pushed
  along on the bonnet.
- Cut-scenes: the inside of the van no longer crushes to black, and a
  half-lit face no longer burns white.
- Faces near a car at night no longer shine like metal, and a street full
  of headlamps is no longer too dark.
- The river's reflections lose their blocky dark outlines, and the
  bridge's piers stop flickering in them.
- The loading screen's texture count no longer disappears while textures
  are still being converted.
- A game that cannot start FSR 3.1 uses TAA instead of quitting.
- A possible crash when a multiplayer game reopens the world.

### Performance
- Fewer stutters while playing: car models and paints load and upload in
  the background and are shared between traffic and damage, a dent's new
  body is built in parallel, blood on a car is cheaper, and the pause
  menu opens at once.
- The mods' shaders are compiled behind the loading screen and kept on
  disk.
- Dry streets under the High lighting draw with lighter shaders.
- Two settings trade a little of the picture for speed: Clouds
  "Volumetric fast" and Trees "Generated fast".

### Multiplayer
- A server can play its own mods: when you join a server with another
  world (a car pack, say), the game offers to download it and opens the
  server's world. It asks once per server, and again when its mods change.
- Car tuning, decals and neon, stunt tracks and the sky race work online,
  through the server's mods.
- The official server runs the character creator, the tuning garage and
  the sky race: on your first join you make your character, and the
  server keeps your look and your car under your name. Nothing to
  install: the server hands you what it needs, and a mod you already have
  at the server's version is used as it is.
- A carjacked driver gets out for everyone, not just for you.
- The player name starts empty and must be filled in before you join or
  host.
- It needs Multiplayer 1.2.2 from the mods page.

### Mods
- Mod API 0.67 to 0.77: a server's mods offered to its players; paint and
  tuning of the player's own car; decals and lights on cars and models; a
  waypoint and a route by road; boost pads and stunt tracks a car drives
  loops on; traffic lights as a mod's models; and one settings window for
  every mod (F5).
- New on the mods page:
  - Tuning garage: at the wheel of your own car, stopped, press U to drive
    into a workshop and change its model, paint, tuning, decals and neon.
    In a car taken from the street, U makes it your car.
  - Sky race: ten stunt courses in the sky, with jumps, loops and wall
    rides. Press O anywhere outside a mission.
  - London map view: M opens a map of the whole city to search, set a
    waypoint, or jump onto a street.
  - Car pack and Car pack 2002: modern cars, or only those on the road in
    2002, in place of the game's and in traffic.
  - UK traffic lights.
- Minimap 1.2 draws the route to your destination; the minimap's, the day
  cycle's and the seasons' settings moved to the F5 window (F11 is gone).
- The character creator is redone: tabs, undo and redo, random looks, and
  looks saved by name.

## 0.1.7

### New
- The pause menu's MISSION BRIEFING, as in the original: during a story
  mission it shows the current objective in the game's language, lets you
  page back through the chapter's earlier ones (COMPLETE / ACTIVE) and
  plays the spoken briefing.
- A failed mission says why under "Mission failed", as the original does:
  "YOU RAN OUT OF TIME!", "YOU LOST THE VAN!", "YASMIN WAS KILLED!".
- A memory meter on every options tab, in both menus: the video memory in
  use now, an estimate for the page's settings, what the selected setting
  costs, and on the Mods tab what each mod takes. A new Texture memory
  setting (Auto, or 1 to 12 GB) under Texture quality caps what the
  textures may use.
- A Frame rate cap (Off, Below refresh for VRR screens, or 30 to 144 fps)
  and Low latency (on by default), which starts each frame as late as it
  can so your input is fresher.
- Vehicle damage has two new steps below Original: Low and Medium, the
  original's rules at a quarter and at half strength.

### Changed
- Smoother motion: with v-sync on, the game no longer drops to a fraction
  of your screen's rate, the game's clock follows the display's own
  timing, and ragdolls, knocked objects and the driving camera move
  smoothly at any frame rate.
- What the game would build the first time it is seen is built behind the
  loading screen, and kept on disk for the next start: fewer stutters the
  first time a car, an effect or a street comes into view.
- Pedestrians on Tuned traffic (the default) walk somewhere: they follow
  the pavements to a destination, cross at junctions and lights rather
  than in the middle of a street, and keep to their side of the road.
  They react in proportion: they step aside only for a car that is
  actually heading at them, complain at one that nudges them, flee from
  an attack they see close by, and raise their hands only at a gun aimed
  at them. The Original setting keeps the PS2's behaviour.

### Fixed
- Retrying a failed mission starts it afresh, as the original does. Before,
  the last attempt carried over:
  - In chapter 7's van chase the van came back still smoking and failed
    every retry at once.
  - On mission 1's retry the police and the gangs were hostile again, and
    traffic stayed five times thinner than it should, in later missions
    too.
  - Mission 2's warehouse kept the last attempt's broken props, and its
    retry could undo what mission 1 had done.
  - The street sounds and the engine of your car stayed silent.
  - Bodies, skid marks, bullet marks and a burnt-out van stayed lying
    around, and the player could walk back to the car he had been getting
    into.
- Passengers (your companion, pursuers' crews) poked through the car's
  roof when it bounced over a kerb.
- Reflections on car paint and glass shimmered around thin things such as
  fire escapes.
- In a cut-scene, a speaker seen in profile at the edge of the frame lost
  the focus.
- The Effects tab's titles in the options sat under the top bar.
- Opening or redrawing the pause menu could freeze a frame for 90 ms on
  wide screens.

### Performance
- Fewer stutters while playing: textures, car and pedestrian models,
  lighting and ray tracing data are uploaded a little per frame instead
  of all at once, the sun's shadows refresh one layer per frame, the log
  is written on its own thread, and traffic and pedestrians do their
  checks only against what is near them.

### Multiplayer
- A server browser: public servers are listed, and you join without
  forwarding a port, through your router. Public hosting is off by
  default; the host page warns that players who join see the host's IP
  address. It needs Multiplayer 1.1.0 from the mods page.

### Mods
- Mod API 0.63 to 0.66: scripts can read the player's health, guns, the
  police's heat, the car and the story, and hear events for them; draw a
  HUD of their own (hiding the game's, with their own fonts); build a
  weapon wheel with slow motion; manage an inventory; draw their own
  widgets in their own style; and use other mods as libraries.
- Seasons for the world: mods can set the day of the year for the sun,
  turn and drop the generated trees' leaves, colour the grass and pile
  leaves on the ground. The new Seasons mod on the mods page runs a
  London year in two hours, with rain and winter snow. Driving in snow is
  easier.

## 0.1.6

### Fixed
- Inside buildings the world could vanish around the camera, worse since
  0.1.5: going up the stairs of the Soho restaurant, or aiming a gun on
  them, the restaurant disappeared and only the city's far skyline showed
  over an empty grey plane.

### Android
- Mods go in `Android/data/dev.secondcoat.london/files/mods/` on the
  phone's storage, where a file manager or a PC over USB can put them.

## 0.1.5

### Fixed
- The prison van mission (Mark's chapter 4) could still get stuck: the van
  stood behind the convoy's burning police car and never drove off, and
  the road blocks the mission lifts at the van stayed standing.
- Ramming a car you chase from the side works as in the original: the hit
  counts by how fast you close in across its flank, kicks the car aside,
  breaks its tyres loose for a moment and rocks it. Only your car pins it,
  no longer the traffic waiting at a light.

### Performance
- Less CPU time per frame on busy streets: pedestrians are posed in
  parallel, the police look for you once per officer per frame, dents
  and ragdolls near cars do less work, and the game finds pedestrians,
  enemies and traffic without searching through all of them.

### Android
- The app was renamed, so 0.1.5 installs beside 0.1.4 instead of updating
  it: delete the old app and choose your disc image again.

## 0.1.4

### New
- On a Steam Deck, a phone or any touchscreen: ONLINE and CHEATS buttons at
  the top right open the multiplayer and cheats windows with a tap, and a
  text field brings up the on-screen keyboard (Steam's on a Steam Deck).

### Multiplayer
- Other players' cars and the traffic move smoothly: busy streets update
  every tick, the cars steer and roll their wheels, keep turning through a
  bend between updates and no longer jump when an update catches up.
- A car you ram stays where you pushed it, for everyone.
- The server checks every player's moves: no driving or running faster
  than the game allows, and no passing through walls.
- A hosted game plays the disc's London: world mods are left out while you
  host and come back when the session ends. Joining a server whose world
  differs from yours opens that world and joins again.
- Cancelling a join while it connects goes back to playing offline.
- 0.1.4 cannot play online with 0.1.3.

### Fixed
- Guns are held as in the original: long guns such as the shotgun and the
  AK47 with both hands, and every gun aimed, drawn, holstered, carried in a
  roll, in cover and around a corner with its own arm poses. Enemies too.
- In Charlie's warehouse (mission 2), the stairwell could vanish into the
  sky half way up, with the camera pressed against its wall.
- In story missions only the police report a crime, as in the original:
  in chapter 7 so many police cars and road blocks came after the van
  that the missions could not be finished in time. In free roam passers-by
  still call the police.
- Road blocks go up as in the original: never on the sites only missions
  use, the streets you just drove or while a getaway route runs, and only
  when the traffic has room for their cars.

## 0.1.3

### New
- A Contrast setting beside Brightness (Options > Display > Picture), and a
  Brightness & contrast page that shows both as sliders over a clean picture.
  From the main menu you set them on a live London street, with the traffic
  and pedestrians passing by; from the pause menu, on the paused game.

### Fixed
- With eye adaptation on Full (the default), a strip of sky over a shaded
  street burned white; the street now keeps its shades and the sky its
  colour.
- The prison van mission (Mark's chapter 4) never ended: the van could not
  be rammed to a stop. The same goes for the later convoy mission that works
  the same way.
- Mission cars that stand waiting, such as the convoy before it leaves,
  were empty; their drivers now sit in them until they get out.
- Police cars could drive into Hammond's museum through its doors and down
  its stairs.
- Looking sideways across the park beside the road in Kensington, the
  ground could vanish, leaving the trees standing over the sky.

### Performance
- Indoors, such as in Hammond's museum, the trees outside no longer cost
  GPU time: up to 10 ms a frame less. Outdoors, trees hidden behind
  buildings are cheaper too.

## 0.1.2

### Changed
- Eye adaptation is now Full by default. Under the High lighting, shaded
  streets and the cars in them look the way your eye would see them in the
  street, where before they were nearly black.
- Car glass is now High by default and part of the Effects preset (Effects >
  Cars): car windows break like real glass. The ORIGINAL preset keeps the
  PS2's glass.

### Fixed
- A "device lost" crash on NVIDIA cards the first time a car hit a wall.
- Under the High lighting, shaded streets were far too dark and the cars in
  them looked black under their reflections.
- Under the High lighting, the sides of a car (Mark's car's doors, for
  example) could turn black.

## 0.1.1

### New
- **macOS**: a universal Getaway.app for Apple silicon and Intel, macOS 12 or
  newer. Not tested on a Mac yet, as we have no Mac hardware; if it does not
  start, please report it.
- Resting against a wall, as in the original: hurt and standing still beside
  a wall, you lean on it with one hand and recover faster.
- A log file: the game writes `logs/getaway.log` and keeps the last five
  sessions. Attach it to a bug report.

### Fixed
- A crash in Hammond's museum mission when an enemy changed route mid-fight.
- An occasional "device lost" crash on NVIDIA cards with FSR 3, more likely
  at higher settings.
- A blurry picture on the Steam Deck and other AMD APUs: they now start at
  Medium with FSR 3.1 Quality. Integrated GPUs pick their texture quality by
  the memory they can use.
- Xbox controllers over Bluetooth with a firmware the game did not know lost
  the right stick and the triggers.
- Cut-scene soundtracks and combat grunts follow the speech language instead
  of always being English. With subtitles off, the scenes with foreign-language
  lines still subtitle those lines, as on the PS2.

## 0.1.0

The first test release, for Windows and Linux.
