# Audio Files Directory

This directory contains mp3 audio files for the Barton Tiles reading application.

## Directory Structure

```
audio/
├── consonants/    # Blue tiles - consonant sounds
├── vowels/        # Yellow tiles - vowel sounds
├── units/         # Red tiles - unit sounds
├── endings/       # Green tiles - ending sounds
├── prefixes/      # Orange tiles - prefix sounds
├── roots/         # Purple tiles - root sounds
└── alphabet/      # Individual letter sounds (a-z)
```

## File Naming Convention

Name your audio files to match the tile text content. Use lowercase and replace spaces/special characters with underscores.

**Examples:**
- `consonants/b.mp3` - for the "b" consonant
- `consonants/ch.mp3` - for the "ch" consonant
- `vowels/a.mp3` - for the "a" vowel
- `units/ar.mp3` - for the "ar" unit
- `endings/ed.mp3` - for the "ed" ending
- `alphabet/a.mp3` - for letter "a"

## How to Add Audio Files

1. Place your mp3 files in the appropriate subdirectory
2. Name them according to the convention above
3. Commit and push to the repository
4. The files will be publicly accessible via the repository

## Accessing Audio Files in Code

Audio files can be referenced using relative paths:

```javascript
// Example: Playing the "b" consonant sound
const audio = new Audio('audio/consonants/b.mp3');
audio.play();
```

## File Requirements

- Format: MP3
- Keep file sizes small for faster loading (recommend < 100KB per file)
- Use consistent audio quality across all files
