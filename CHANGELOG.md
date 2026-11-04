# Changelog

## 0.3.1

### New
- The original's camera as an option: Locked camera (Off, Original) puts
  the PS2's cameras in place of the free view, on foot holding its
  bearing while you move and swinging behind you when you stop, at the
  wheel with each car's own framing, the reverse and wall swings and the
  cab views. Car camera (Close, Medium, Far, Original) sets how far the
  chase camera hangs behind. The Gameplay preset's Original level sets
  both, and both apply at once from the pause menu.
- A First person switch on the Gameplay tab. In first person a car's
  indicators show as two green arrows at the bottom of the screen and
  blink the controller's light bar amber.
- Options > Mods > Mod controls rebinds every mod's keys and pad
  buttons, as the Controls tab does the game's.
- The mods' windows are played with a pad: the d-pad moves through them,
  LB and RB go from window to window, the right stick scrolls, B backs
  out. A mod can give the pad a pointer of its own, and an on-screen
  keyboard (the new Virtual keyboard mod) types with the pad.
- The mod manager says when the texture cache lacks textures for the
  mods you turned on, and prepares them there and then.

### Changed
- A failed mission's result stays on the screen for 4 seconds, long
  enough to read why, before the mission starts again.
- The city is silent under a cut-scene or a film: its police radio,
  sirens and crashes no longer play through them.
- Long hair hangs looser and falls over the shoulders: in the opening
  cut-scene Yasmin's hair no longer turns with her head as one bundle.
- A wiped windscreen beads up again as fast as the rain falls on it.

### Fixed
- The shoot-out with the Soho gang ends once they are down, and its
  groups surrender: the mission never ended, however many of them died.
- The Yardies can be killed: they kept the full health their paths gave
  them.
- The prison van in the escort mission no longer stops for the cars of
  its own escort.
- In the drug factory, the masked men stand on the lab's floor, in
  sight: they stood on a hidden floor just above it and shot through
  the walls, unseen. Feet no longer float there either, and after a
  restart the lab is drawn instead of a grey box.
- The car you tail through the city keeps left, overtakes only when the
  other lane is clear, waits for the go on its handbrake (it reversed
  across the police station's courtyard) and no longer gets stuck at the
  lamp post under the arch or behind a closed road.
- A mission's cars that follow a route brake before bends and get
  unstuck.
- The river under a bridge no longer flickers to the sky in the
  reflections.
- Upscaling the textures no longer fails on NVIDIA graphics cards.
- The Windows package no longer needs the VC++ runtime installed.

### Performance
- Shoot-outs: the debris knocked off walls is simulated off the main
  thread and over several cores, and a settled pile lies still until
  something reaches it. Before, it could take most of the main thread.
- Deep snow and the falling flakes are much cheaper to draw.

### Mods
- Mod API 0.92 to 0.99: messages between mods, map blips on the minimap
  and the London map view, the player's outfits, dark rooms, muffled
  sound indoors (where the rain and the night also stay out), the pad's
  buttons in prompts and scripts, the pad's pointer, the on-screen
  keyboard, and a hair style's front line.
- Safe house 1.2.1: the flat furnished, with first-aid kits, a laptop to
  order guns and kits, a wardrobe of outfits, a light switch, a house on
  the maps and your last car parked at the door.
- Open interiors 1.2.0, Minimap 1.3.0 and London map view 1.1.0 for the
  above; Strand hair: Yasmin long 1.1.0 keeps her hair behind her
  shoulders, in front only beside her face; Cheats 1.0.3 and
  Multiplayer 1.2.4 use the touch pad only where the pad has one; Sky
  race shows the pad's buttons.
- Update them from the mods page.
- New on the mods page:
  - London life: buy the missions' buildings and Reggie's pub, keep a
    stash in each, collect their daily takings, and shop on a 2002 web
    from the laptop: an estate agent, a car dealer whose cars wait at
    your door, an importer of guns, a bank and an evening paper. Needs
    Economy and Safe house; free roam, offline.
  - Economy: a wallet the other mods pay from and into, £2,500 to start
    and a statement; online the server keeps it.
  - Virtual keyboard: an on-screen keyboard to type with a pad, for
    other mods' text fields such as London life's address bar. The PS5
    title ships it.

## 0.3.0

### New
- Upscale the textures yourself: the mod manager's Tools > Upscale the
  textures… makes the HD textures from your own disc on the graphics card
  (4x-UltraSharpV2, the ground 4x-PBRify), the cars' paint, lamps and
  cut-scene cars included, and the generated materials (DeepBump) with
  them, into the HD textures and Generated materials mods. The networks
  are downloaded once from our file host. On the PS5 the launcher's HD
  textures page has Upscale from the disc. No PCSX2 pack needed (Linux,
  Windows and the PS5).
- A new mod manager: the mods in load order with their switches, the
  ones that are off below, a search and filters (All, On, Off, Problems)
  with why a mod does not load in its row, a page per mod with what it
  needs and what needs it, and mods installed by dropping them on the
  window.
- Faces: the original characters' painted eyes shade as eyes (a round
  iris with a limbal ring, the whites kept, no glint under the lids),
  their lips have a wet sheen, and brows and lashes grow as strands with
  the strand hair. Lip sync is smooth in the cut-scenes (Options >
  Gameplay > Lip sync: ORIGINAL or SMOOTH). Face enhancements can be
  turned off under Advanced Graphics > Characters, and are off in the
  Original preset.
- Saving in a mission: a save from the pause menu during a mission
  resumes it where you saved, at a quiet moment (otherwise CAN'T SAVE NOW
  and why). Retries still start the mission over.
- Free roam is kept: where you were, your health and guns, and your car
  wherever you left it, with its paint and damage. Free Roam offers
  CONTINUE and RESTART when there is a save.
- Proximity voice chat in multiplayer: push to talk, heard from where
  the speaker stands, on servers that offer the Multiplayer voice mod
  (which the packages ship). Linux, Windows and the PS5, where the
  DualSense's microphone works and voices play on the TV or the
  controller's speaker.
- Reflections at the lower settings: a planar mirror on the wet streets
  and local reflection probes around the camera, on in REMASTER MEDIUM.
  Where reflections are traced, night puddles mirror the lit windows and
  tremble with the rain.
- Android: a gamepad plays the game, a device's own controls or a
  Bluetooth pad; the touch controls hide while it plays.
- A small "Baking lighting" spinner at the top right while the lighting
  bakes in the background during play.

### Changed
- The options are simpler: Display, Graphics and Gameplay show a row per
  group (lighting, shadows, reflections, traffic, damage, assists, …),
  each a preset that reads CUSTOM once you change one of its settings.
  Every single setting is still there on the Advanced tab.
- Strand hair: long hair stays out of the body (it lies on the shoulders
  and moves aside for the arms and hands), holds still at rest, starts
  at rest after a cut, and no longer curls in the rain. Without MSAA the
  strands blend instead of speckling under FSR 3.1 or the TAA; with MSAA
  fine hair no longer turns into a veil. Light scatters through long
  hair, so it keeps a soft sheen in its depth. The simulation runs on the
  graphics card.
- Cut-scenes: the depth of field focuses on the speaker's eyes, a face in
  close-up stays sharp with the street behind it soft, and the focus
  moves to the next speaker as they begin. Rain drops on a windscreen
  blur with the depth of field, and a car's cabin seen from inside stays
  dry.
- The graphics benchmark asks before it applies what it suggests.
- `menu_font` in settings.ron sets the menus in a font you have
  installed, such as the original's Gill Sans.
- The packages no longer ship Dawn.

### Fixed
- The aim assist locks onto police officers coming for you.
- The Republic's restaurant no longer vanishes as the camera comes in
  from the entrance hall or looks down in the bar.
- A police car on your trail no longer appears inside a building (on
  The Republic's first floor).
- Stepping past the end of a wall in cover no longer counts as sneaking.
- An oncoming car's headlamps no longer leave a white blob or cloud
  down a wet street at night.
- A new game starts the sky afresh: a second new game of the same
  mission kept the last one's clock, and its rain came early.
- No triangles in the faces' ambient occlusion with CACAO (the PS5's
  settings).
- In the opening cut-scene a lamp no longer lights Mark's car red from
  inside: a cut-scene car takes the scene's lamps as in the original.
- The player no longer gets stuck half way down some stairs.
- The loading screen's count no longer jumps.

### Performance
A measured pass over the whole game, every change keeping the picture
and the game exactly as they were.
- Loading: behind the loading screen the city is placed as fast as it
  comes in instead of a piece a frame, textures are read in half the
  time with half the memory, a pedestrian's far model shares its near
  model's textures instead of loading its own, and the clouds' noise is
  made in the background and kept for the next start. The shaders'
  pipelines are built side by side, and with AMD's driver on Linux the
  pipeline cache now finds them again at the next start.
- Fewer stutters: pedestrians', enemies' and crowd figures' textures and
  models come in on the loaders instead of the main thread, the drivable
  cars are read once instead of at every swap, a mod car's normal maps
  are not decoded again, and the combat sounds are prepared once.
- The simulation: the traffic's drivers decide side by side on every
  core, and a getaway driver plans its lines several times faster (it
  cost up to 19 ms a frame on a PS5). The pedestrians, the enemies'
  poses, the paths on foot, the collision lookups, the night's lights
  and the lit windows, the feet on the ground and the strand hair all do
  less work or share it over the cores. Mods' placed interiors no longer
  cost up to 14 % of the main thread in free roam.
- The graphics: the skin's light scattering runs only with a face near
  enough to show it, the city's plain walls lay their depth without a
  shader, and the rain's drops, the TAA, the motion blur, the shadows, the
  reflection probe and the rain on the lens are all cheaper. Fewer of
  the GPU's waits between passes.
- The PS5: the title is built with link-time optimisation for the
  console's own CPU, and its memory comes from eight heaps so the
  threads no longer wait on each other to allocate.

### Mods
- Mods can let the player ride along in their vehicles and let the
  world's time pass at once (a taxi, a bus, a bed to sleep in), keep a
  panel behind the others, set how much litter a tyre kicks up, and hear
  when free roam starts.
- London ground 0.9.0: thin autumn leaves on the road are kicked up far
  less.
- Tuning garage 0.2.2: a click beside an item no longer locks the
  garage, and its car list offers only cars you can drive.
- Strand hair: Yasmin long 1.0.1: her hair stays on her shoulders and
  rises from the crown.
- Update London ground, Tuning garage and Strand hair: Yasmin long from
  the mods page.
- New on the mods page: Faster cars (every car with 1.5 times the power
  and 1.15 times the top speed, traffic and police included), Safe house
  (Mark's flat in free roam: a crate that keeps your guns and a bed that
  sleeps the clock forward and heals; needs Day cycle) and Open interiors
  1.1.0 (Mark's flat to walk in).

## 0.2.0

### New
- The PS5. A jailbroken PS5 with native homebrew (etaHEN) runs the
  remaster as the title "Second Coat: London" (PPSA99020): install it
  under `/data/homebrew/` or through ProsperoStore and copy your disc image
  to `/data/secondcoatlondon/game.iso` over FTP. A launcher in the style
  of the console's home screen checks the disc, moves the PCSX2 HD pack
  into place, prepares the textures, and turns mods on and off, updates
  and installs them from the mods page. The first start is set for 40 to
  50 fps (FSR 3.1 Performance, REMASTER MEDIUM effects with the ray
  tracing kept), with PlayStation prompts. The DualSense's haptics carry
  the rumble, its adaptive triggers follow the gun in your hand and the
  car's pedals, the police radio plays from its speaker and the light bar
  flashes in a pursuit. The touch pad's left half opens the cheats, its
  right half multiplayer. Generated materials, London ground, the
  MakeHuman characters, strand hair, the cheats and multiplayer ship with
  it.
- The cut-scenes' particles: cigar and cigarette smoke and the breath
  they exhale, a lighter's spark and flame, the steam off a coffee, spat
  blood and the cars' smoke, as the original plays them.
- REMASTER MEDIUM effects: the remaster's effects with cheaper settings
  for the costly ones (reflections, light shadows, indirect light and
  clouds), between ORIGINAL and REMASTER HIGH. The graphics benchmark now
  tunes the effects too, and steps them down before the resolution. It
  aims at a frame rate you choose (30 to 165 fps, Options > Display >
  Benchmark target), times the CPU beside the GPU and says when the CPU
  sets the frame rate.
- Playing in VR no longer needs a setting edited by hand: the Linux and
  Windows packages carry `getaway-vr`, which starts the game in the
  headset.

### Changed
- Strand hair looks more real: the hair shadows itself and the skin and
  clothes under it, catches the lamps' and the sky's highlights, and
  clumps and hangs heavier in the rain. It no longer flickers, shows
  triangles or covers the ears, covers the whole head, and is lit as the
  skin beside it (Susie's blonde no longer goes grey at night). Long hair
  lies over the shoulders and down the back, slides off them and falls
  with gravity, and trails the head's moves. The hair no longer bounces
  at an uneven frame rate or lags a walking figure at a low one, and
  under FSR 3.1 it is no longer speckled. A Strand hair quality setting
  (LOW, MEDIUM, HIGH) sets how much of it you get.
- Local lights and the indirect light are cheaper, with the same picture.
- Fewer stutters at speed: London ground's cover and facades are placed
  near the camera first, and the rain's puddles move with you more
  cheaply.

### Fixed
- Wet ground with screen reflections off no longer mirrors the bright
  sky under facades and roofs, where the puddles read as snow.
- The game no longer stops with a fatal error when a multiplayer server's
  world opens again.
- Starts on more graphics cards: Intel's UHD 620 on Windows, and the
  Adreno 650 and 740 phones (the 740 without the fire's volumes). Android
  phones trace rays only when an option asks for it.
- A car no longer shows itself in its own ray-traced reflections: in
  the opening cut-scene the gang's car mirrored its beige cabin on its
  bonnet and roof.
- One failing pedestrian figure no longer leaves every figure after it
  missing.

### Mods
- Mods can give strand hair flyaways, baby hairs at the hairline and
  coiled locks (dreadlocks, braids).
- London ground 0.8.0: the autumn leaves keep off the road's lanes, lie
  in drifts drawn out along the wind, and turn from golden to russet in
  the distance.
- Strand hair 1.0.1: Susie's hair is fuller.
- Update London ground and Strand hair from the mods page.
- New on the mods page: Strand hair: Yasmin long, with Yasmin's hair let
  down from her bun to the middle of her back, in the cut-scenes and in
  the game. It loads after Strand hair.

## 0.1.10

### Fixed
- In Mark's chapter after the boiler-suit escape, the van is waiting
  where the mission sends him again: it was placed far away before he got
  there and was gone by the time he arrived. Continuing the story with
  the Tuning garage mod also no longer swaps that van for your tuned car.
- In the next mission, McCormack walks his route upstairs again instead
  of standing in the corridor until Mark set off the triggers downstairs.
- No more strips of snow on the floors indoors along the walls in a
  winter fall.
- A mod's panel without a set width no longer wraps its text one letter
  a line: the Day cycle mod's clock went narrow at 11:50 and stayed so.

### Changed
- Fewer stutters while driving: the leaves and debris on the streets and
  the puddles in the rain do their work off the main thread.

### Mods
- Update Tuning garage to 0.2.1 from the mods page.

## 0.1.9

### New
- Gamepad rumble. The PS2's vibration is ported: crashes, kerbs,
  misfires, fire, being hit, blasts, shots and a mission's end. A Rumble
  setting (Options > Controls) picks the original's patterns, or Tuned
  (the default): as strong as what happened and silent in the menus, with
  a strength slider.
- Button prompts for the pad you hold: Xbox, PlayStation, Steam Deck or
  Switch. The Controls tab shows the pad's buttons, there is a Button
  prompts setting, and Options > Controls > Controller layout shows the
  whole pad.
- In a police car, an ambulance or a fire engine, a tap of the horn turns
  the roof lights and siren on and off; held, it is still the horn. With
  the siren on, the police lose interest as they do in a pursuit. The
  recovery truck only has its lights.
- As in the original, the holster key throws a big gun away: it lands
  behind you with the rounds in its magazine and can be picked up again
  after a moment, but the spare ammunition is gone. The pistol stays
  drawn. Not while you aim, fire, reload, pick something up or hold a
  hostage.

### Changed
- Healing against a wall ends by itself at full health: you stand up off
  the wall and do not lean again until you are hurt.
- The game starts faster: the renderer's shaders are built side by side.

### Fixed
- The game no longer starts below the street when a mod has built
  something under the start point.

### Mods
- Mods can place their own models in the world: buildings, interiors,
  stairs and moving platforms that carry you along, with their own
  collision and openings cut into the city's ground. Online the server
  places them for everyone. Placements are written in `world/<name>.ron`
  or from a script, and the placement editor (F9, F10 saves) places them
  in the game.
- Mods can play their own sounds and music (Ogg, MP3, FLAC, WAV), at a
  fixed point or on the car, the player or a character, in 3D.
- The Car radio mod: your own music as radio stations in the car, tuned
  with the mouse wheel or the d-pad on a station wheel. Out of the car it
  sounds muffled behind the doors.
- London ground 0.7.0: the autumn leaves lie as a real layer on the
  paving, and wheels and footsteps kick them up; a car's wake carries
  them along. Falling leaves take their shapes.
- Mod shortcuts can use the game's own actions.
- Update Multiplayer to 1.2.3 and Cheats to 1.0.2 from the mods page.

### Multiplayer
- The protocol has changed: 0.1.9 and 0.1.8 cannot play together.

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
