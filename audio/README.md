# Audio Files for Barton Tiles

This folder contains MP3 audio files for tile sound playback.

## File Naming Convention

Audio files should be named using the pattern: `{phoneme}-{example-word(s)}.mp3`

For example:
- `a-apple.mp3` - short "a" sound
- `a-cake.mp3` - long "a" sound (used for ai, ay, etc.)
- `ch-chick.mp3` - ch digraph
- `ar-jar.mp3` - r-controlled vowel "ar"

## Required Audio Files

Based on the AUDIO_MAP in the application, here are the expected audio files:

### Single Consonants
- b-bat.mp3
- c-cut.mp3
- d-dip.mp3
- f-fun.mp3
- g-get.mp3
- h-hat.mp3
- j-jug.mp3
- k-kit.mp3
- l-lip.mp3
- m-map.mp3
- n-net.mp3
- p-pig.mp3
- qu-quit.mp3
- r-rat.mp3
- s-sit.mp3
- t-tip.mp3
- v-van.mp3
- w-wig.mp3
- x-fox.mp3
- y-yak.mp3
- z-zip.mp3

### Consonant Digraphs
- ch-chick.mp3
- ck-duck.mp3
- sh-ship.mp3
- th-thick.mp3
- wh-whip.mp3
- ph-phone.mp3

### Single Vowels (Short)
- a-apple.mp3
- e-elephant.mp3
- i-igloo.mp3
- o-octopus.mp3
- u-umbrella.mp3

### Vowel Teams (Long Vowels)
- a-cake.mp3 (used for: ai, ay, ey, eigh, ei)
- e-team.mp3 (used for: ee, ea, ie, y as long e)
- i-kite.mp3 (used for: igh)
- o-boat.mp3 (used for: oa, oe, ow, eau)
- u-cube.mp3 (used for: ue, ew, eu, tu)
- oo-moon.mp3

### R-Controlled Vowels
- ar-jar.mp3
- or-fork.mp3
- er-herd-bird-turn.mp3 (used for: er, ir, ur)
- ear-hear.mp3

### Other Vowel Patterns
- air-pair-share.mp3
- oi-oil-boy.mp3 (used for: oi, oy)
- aw-haul-hawk-ball.mp3 (used for: au, aw, augh)
- ou-cloud.mp3

### Silent Letters
- ps-psychology.mp3
- rh-rhino.mp3
- mn-autumn.mp3
- wr-write.mp3
- kn-knock.mp3
- gh-ghost.mp3
- gn-gnome.mp3
- que-antique.mp3
- gu-guitar.mp3
- gue-league.mp3

### Units (Red Tiles)
- all-ball.mp3
- ang-bang.mp3
- ing-sing.mp3
- ong-song.mp3
- ung-lung.mp3
- ank-tank.mp3
- ink-pink.mp3
- onk-honk.mp3
- unk-trunk.mp3
- oll-doll.mp3
- old-cold.mp3
- olt-bolt.mp3
- ost-most.mp3
- ild-wild.mp3
- ind-kind.mp3
- ture-picture.mp3

## Instructions

1. Place all MP3 files in this `audio` folder
2. Ensure file names exactly match the naming convention above (case-sensitive)
3. Files should be in MP3 format
4. The application will automatically find and play the correct audio file when tiles are clicked

## Fallback Behavior

For tiles without audio files (such as prefixes, suffixes, and roots), the application will use Text-to-Speech (TTS) to pronounce the text.

## Multi-Tile Pronunciation

When clicking on connected tiles (groups), the application will:
1. Speak the entire group as a word using TTS
2. Use stored pronunciation context if available (for syllables broken from known words)

## Adding New Audio Files

To add audio for additional tiles:
1. Create the MP3 file following the naming convention
2. Add an entry to the `AUDIO_MAP` object in `index.html`
3. Place the file in this folder

Example:
```javascript
AUDIO_MAP: {
  // ...
  'newphoneme': 'newphoneme-exampleword',
  // ...
}
```
Then create: `audio/newphoneme-exampleword.mp3`
