# Changelog

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
