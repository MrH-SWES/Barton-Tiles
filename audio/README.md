# Audio Files for Barton Tiles

This directory contains audio files for the Reading Tile Board application. Each tile can play a sound when clicked to help learners associate letters and letter combinations with their sounds.

## Required Audio Files

The following 57 audio files are needed for full functionality:

```
a-apple.mp3
a-cake.mp3
air-pair-share.mp3
ar-jar.mp3
aw-haul-hawk-ball.mp3
b-bat.mp3
c-cut.mp3
ch-chick.mp3
d-dip.mp3
e-elephant.mp3
e-team.mp3
ear-hear.mp3
er-herd-bird-turn.mp3
f-fun.mp3
g-get.mp3
h-hat.mp3
hw-whip.mp3
i-igloo.mp3
i-kite.mp3
j-gem-giant-gym.mp3
j-jog.mp3
k-kit.mp3
l-lip.mp3
m-mug.mp3
n-gnome.mp3
n-knife.mp3
n-nap.mp3
ng-ring.mp3
o-octopus.mp3
o-rope.mp3
oi-soil-toy.mp3
oo-book-bush.mp3
oo-boot-new.mp3
or-fork.mp3
ou-how-out.mp3
p-pick.mp3
qu-quest.mp3
r-rid.mp3
s-cent-cirus-cycle.mp3
s-his.mp3
s-sit-mess.mp3
Schwa-What.mp3
sh-ship.mp3
th-the.mp3
th-thin.mp3
t-tuck.mp3
u-lute-glue.mp3
u-up.mp3
u-use-cue.mp3
ure-lure.mp3
v-van.mp3
w-will.mp3
wr-wrist.mp3
x-mix-rocks.mp3
y-yes.mp3
z-zip-buzz.mp3
```

## Adding Audio Files

### From Windows Network Drive

If your files are currently at:
```
\\Files\StaffHome\whenderson\My Documents\Tiles App\Audio\
```

**Copy all `.mp3` files to this directory:**
1. Navigate to the network location in File Explorer
2. Select all `.mp3` files (57 files total)
3. Copy them to this `audio/` folder in your repository
4. Verify all files are present

### File Requirements

- **Format**: MP3
- **Naming**: Must match exactly as listed above (case-sensitive on some systems)
- **Location**: All files should be in `/audio/` (no subdirectories)

## Current Status

- [x] Audio mapping documentation created
- [ ] Audio files copied to repository
- [ ] Audio playback functionality implemented
- [ ] Testing completed

## Audio Mapping

See [AUDIO_MAPPING.md](./AUDIO_MAPPING.md) for detailed information about:
- Which audio file corresponds to which tile
- Phonetic categories
- Book level organization
- Implementation guidelines

## Technical Details

### File Usage

Audio files will be referenced in the application using the pattern:
```javascript
const audioPath = `audio/${tileName}.mp3`;
```

Where `tileName` is determined by mapping the tile text to the appropriate audio file.

### Browser Compatibility

All modern browsers support MP3 playback via the HTML5 `<audio>` element or Web Audio API.

## Next Steps

1. Copy audio files from your Windows network drive to this directory
2. Implement audio playback functionality in `index.html`
3. Test audio playback across different devices
4. Consider adding volume controls and mute functionality
