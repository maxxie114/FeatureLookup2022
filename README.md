# FeatureLookup2022

[![Python Version](https://img.shields.io/badge/python-3.x-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

> A command-line phonological features lookup tool for linguistics research and education.

FeatureLookup2022 is a Python-based interactive program that provides easy access to phonological feature data for phonemes. It's designed to help linguistics students and researchers quickly look up, compare, and analyze phonological features based on standard phonological feature charts.

## Table of Contents

- [Background](#background)
- [Features](#features)
- [Install](#install)
- [Usage](#usage)
  - [Basic Commands](#basic-commands)
  - [Advanced Commands](#advanced-commands)
  - [Examples](#examples)
- [Data](#data)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Background

This program is a compilation of feature data for use in phonology, originally created for UCSC LING 101, Spring 2022, with Professor Jaye Padgett. It's based on standard phonological features charts (Hayes 2009) and provides an interactive command-line interface for easy feature lookup and comparison.

Phonological features are the basic building blocks used to describe the sounds of human language. This tool makes it easy to:
- Look up features for specific phonemes
- Compare features across multiple phonemes
- Filter phonemes by specific feature values
- Work with sets of phonemes for analysis

## Features

- **Interactive Command-Line Interface**: Easy-to-use CLI with helpful prompts
- **Comprehensive Phoneme Database**: Includes vowels, consonants, and various IPA symbols
- **Multiple Lookup Methods**:
  - List all phonemes or specific phoneme features
  - Compare features across multiple phonemes
  - Contrast features between two phonemes
  - Filter phonemes by feature values
- **Set Management**: Build and manipulate custom phoneme sets for analysis
- **Abbreviation Support**: Use shortened feature names for faster input
- **Feature Coverage**: 22 phonological features including syllabic, vocalic, high, low, back, round, ATR, sonorant, approximant, coronal, anterior, distributed, dorsal, labial, pharyngeal, continuant, strident, lateral, nasal, voice, aspirated, and glottalized

## Install

### Prerequisites

- Python 3.x (tested with Python 3.12)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/maxxie114/FeatureLookup2022.git
cd FeatureLookup2022
```

2. Run the program:
```bash
python3 FeatureLookup2022.py
```

No additional dependencies are required!

## Usage

### Basic Commands

Start the program:
```bash
python3 FeatureLookup2022.py
```

Once running, you can use the following commands:

- **`help`** - Display help information
- **`list`** - List all phonemes in the database
- **`list <phoneme>`** - Display all features for a specific phoneme
- **`list <feature> <+/-/0>`** - List all phonemes with a specific feature value
- **`compare <phoneme1> <phoneme2> ...`** - Show shared features among phonemes
- **`contrast <phoneme1> <phoneme2>`** - Show differing features between two phonemes
- **`advanced`** - Display advanced functionality help
- **`end`** - Exit the program

### Advanced Commands

The program includes set management functionality:

- **`set`** - Display current phoneme set
- **`set clear`** - Clear the current set
- **`set add <phoneme>`** - Add a specific phoneme to the set
- **`set add <feature> <+/-/0>`** - Add all phonemes with a specific feature value
- **`set add all`** - Add all phonemes to the set
- **`set delete <phoneme>`** - Remove a specific phoneme from the set
- **`set delete <feature> <+/-/0>`** - Remove phonemes with a specific feature value
- **`set filter <feature> <+/-/0>`** - Keep only phonemes with a specific feature value

### Examples

**List all phonemes:**
```
>> list
i    ɪ    u    ʊ    e    ɛ    o    ɔ   
a    ɑ    æ    y    ʏ    ø    œ    ɘ   
...
```

**Look up features for /i/:**
```
>> list i
syllabic: [+]
vocalic: [+]
high: [+]
low: [-]
...
```

**List all voiced phonemes:**
```
>> list voice +
d    z    ɮ    ð    ʒ    ɟ    ʝ    dʒ  
...
```

**Compare features between /p/ and /b/:**
```
>> compare p b
syllabic: [-]
vocalic: [-]
high: [-]
...
```

**Contrast /p/ and /b/:**
```
>> contrast p b
voice: [-/+]
```

**Use abbreviations:**
```
>> list voi +
Interpreted: < list voice + >
d    z    ɮ    ð    ʒ    ɟ    ʝ    dʒ  
...
```

## Data

The program includes data for 75 phonemes covering:
- Vowels: i, ɪ, u, ʊ, e, ɛ, o, ɔ, a, ɑ, æ, y, ʏ, ø, œ, ɘ, ʌ, ɯ, ɨ
- Approximants: j, w, ɥ
- Nasals: m, n, ɳ, ɲ, ŋ, ɴ
- Liquids: l, ɭ, ʎ, r, ɽ, ʀ
- Stops: t, d, ʈ, ɖ, p, b, k, g, q, ɢ, ʔ
- Fricatives: s, z, ɬ, ɮ, θ, ð, ʃ, ʒ, ç, ʝ, ɸ, β, f, v, x, ɣ, χ, ʁ, ħ, ʕ, h, ɦ
- Affricates: tʃ, dʒ, ts, dz, pf, bv
- Palatals: c, ɟ

Each phoneme is characterized by 22 phonological features with values of `+` (present), `-` (absent), or `0` (not applicable).

## Contributing

Contributions are welcome! Here's how you can help:

1. **Report Bugs**: Open an issue describing the bug and how to reproduce it
2. **Suggest Features**: Open an issue with your feature request
3. **Submit Pull Requests**: 
   - Fork the repository
   - Create a feature branch (`git checkout -b feature/AmazingFeature`)
   - Commit your changes (`git commit -m 'Add some AmazingFeature'`)
   - Push to the branch (`git push origin feature/AmazingFeature`)
   - Open a Pull Request

### Areas for Contribution

- Add support for diacritics
- Expand phoneme database
- Add export/import functionality
- Create GUI version
- Add unit tests
- Improve documentation

## License

This project is available under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgments

- Created by NS Dawn
- Originally developed for UCSC LING 101, Spring 2022
- Professor Jaye Padgett
- Based on the Phonological Features Chart (vers. 2015-2, Hayes 2009)

---

**Note**: This program covers basic phonemes and does not currently include diacritics. Feature values are based on standard phonological theory and may vary depending on theoretical framework.
