# Changelog

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
