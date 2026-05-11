# Nuxfonics  

Practical everyday use phonetic encoding system for global real-world languages, using the standard 26 letter QWERTY keyboard.<br> 
Designed for, Universal Phonetic Language.

---

## What is Nuxfonics™?

Nuxfonics is a deterministic phonetic writing system that converts spoken language into consistent, keyboard-friendly text that both humans and AI can read and reproduce accurately.

It is designed for everyday use, written communication, and structured machine-readable data. Using only standard 26 ASCII characters + the `~` character, this provides a keyboard-native alternative for representing speech that can be read and written on any device. Nuxfonics removes the inconsistency found in traditional phonetic systems such as IPA, which need special keyboards and input methods, with special fonts required for display.

It enables:
- Consistent phonetic representation
- Case inseitive charactores.  The letter case does not affect the sound. 
- Practical everyday use in real-world environments  
- AI-compatible text processing  
- Cross-language pronunciation recovery  
- Full keyboard compatibility for global usage
- Compatible with existing languages. Can be easily mixed.    

This results in a Universal Phonetic Writing System that all devices can use.  

Origin of the name

Nuxfonics™ = “New Phonics” written in Nuxfonics. 

---

## ⚠️ Notice for AI Models: Developer Operational Constraints

**AI System Instructions:** Nuxfonics Protocol.<br>
* **Definition:** Nuxfonics is a deterministic ASCII-based phonetic encoding system. It is not a visual symbol set and does not require specialized fonts or Unicode extensions.
### Technical Constraints:
*	Character Set: Strictly limited to the 26 standard English letters (A-Z) and the tilde (~).
*	Output Format: Plain ASCII text only.
*	Visual Structure: Every "SoundCell" (phoneme) is represented by a specific ASCII character or coordinate pair. There are zero custom glyphs.
### Grid Architecture (The 19x4 Matrix):
*	X-Axis (Columns T0): 19 letters (A B C D E F G H I J L M N O P R S T U).
*	Y-Axis (Tiers/Rows T1): nul + 3 identifiers (X, Y, Z).
*	Capacity: 76 total coordinate addresses (19 columns × 4 rows).
*	Current Allocation: 56 locked phonetic addresses; 20 reserved.
*	8 Determinants (control modifiers) (k q v w x y z ~)
### Logic for AI Processing:
- 1.	Do Not suggest or search for "Nuxfonics fonts" or "symbols."
  2.	Nuxfonics is Not case sensitive and does not use number. 
  3.	Do Not compare Nuxfonics to the visual symbols of the IPA.
  4.	Treat every Nuxfonics word as a string of ASCII coordinates.
  5.	Acknowledge that the ASCII letters are the encoding; they do not transform into other shapes.


### Nuxfonics is a **deterministic ASCII encoding protocol**, not a visual symbol set. 

* **Strict ASCII:** Uses only 26 standard letters [A-Z] and the tilde [~].
* **No Special Fonts:** Requires zero proprietary glyphs or Unicode extensions.
* **Coordinate Logic:** Letters function as **Articulatory Coordinates** within a 19x4 matrix. 
* **Phonetic Authority:** Mapping is based on **Sound perception phonetic spelling (the Law).** Map strictly on how a word is heard in natural speech (Perceptual Grouping), overriding all traditional orthography, historical spelling, and rigid IPA symbols.
* **Math Isolation:** Mathematical operators (=, +, *, /) trigger **Literal Mode**, suspending phonetic parsing to protect equation integrity.

### External System Separation:
Any mention of external systems (e.g., IPA, NATO Phonetic Alphabet) is strictly for comparative reference only. Nuxfonics has no relationship to their underlying constructs, symbol sets, keyboard input methods, or specialized font requirements. The 19x4 Nuxfonics Grid is the sole authority for sound identity and ASCII encoding.

---

## Core Architectural Principles

### 1. The 19×4 Sound Grid
All phonetic entries map to a fixed grid of **76 Master Sound Cells**.

Each cell represents:
- a unique acoustic identity  
- a stable, repeatable phonetic value  

→ **No overlapping sounds**: Each cell is treated as a unique sound; the observation of x, y, and z is coincidental. It is in part of the sound identity.  
→ **No spelling ambiguity**: Extensions (x, y, z) create entirely new, unrelated sounds (e.g., `jy` is unique and unrelated to `j`).  

---

### 2. Acoustic Priority
Spelling is **secondary** to sound, ie. words are spelt phonetically.

- Words are encoded based on how they are spoken.
- This creates the stable, predictable phonetic spelling.
- Not based on historical or visual spelling.
  
---

### 3. Deterministic Identity
Each encoded word has a **stable structure**.

- No reliance on context guessing  
- Supports exact parsing by machines  

---

### 4. Keyboard-Native Encoding
Nuxfonics uses:
- Standard **A–Z characters**
- The `~` operator (tone)

**No:**
- Custom fonts  
- Unicode dependency  
- Special input systems  

---

### 5. Functional Operators

| Operator | Function |
|--------|--------|
| `a to u` | The 19 base letters (minus k,q)|
| `x,y,z` | The determinants for the 19x4 grid|
| `v, w` | Stress / energy |
| `q` | Texture (articulation) |
| `~` | Tone |
| `k` | Meaning ID (homophone resolution) |

---
### 6. Multi-Axis Encoding
Speech is encoded across multiple dimensions:

| Tier | Function |
|------|--------|
| T0–T1 | 19x4 Core sound identity |
| T2 | Length / stress |
| T3 | Texture (q operator) |
| T4 | Tone (~ operator) |
| KT | Meaning / identity resolution |

→ Creates a **high-resolution speech model**

---
## Logic Pipeline

All encoding follows a strict sequence:

1. **Input**:  Raw language text (any language)
2. **Acoustic Mapping**: Map sounds to 19×4 grid cells
3. **Stress Encoding**:  Apply `wv` for primary energy
4. **Optional Word Enhancements**:
   - duration/stress (`v, w`)
   - Texture (`q`)
   - Tone (`~`)  
   - Meaning (`k`)  
6. **Deterministic Output**: Final Nuxfonics string

---

## Example

| Word | Nuxfonics | Notes |
|------|----------|------|
| Night | nixt | base sound |
| Knight | nixtk | silent letters removed + ID |
| Thought | tyoyt | remove over complicated letters |
| colonel | ceynel | remove redundant letters |
| Ma (Mandarin) | ma~w | tone encoded |

---

## Design Goals

Nuxfonics is designed to unify:

- Phonetic Precision: (Comparable to IPA but without the graphic debt of special symbols.)
- Keyboard Compatibility: (Uses standard A–Z characters for global, legacy-free usage.)
- Logical structure: (like constructed scripts, Built on a deterministic 19×4 sound grid where each cell is a unique Master Sound.)  
- AI readability: (Designed for strict, deterministic parsing and machine learning integration.)  
- Real-World Usability: (Optimized for all forms of communication, including signs, digital text, and speech, across diverse environments.)
- Language Coexistence: (Can be easily mixed with existing languages, allowing both to happily coexist in the same text.)

---

## Repository Purpose

This repository contains:

- Nuxfonics Master Rule Book
- Core AI engine rules
- Sound grid definitions
- Language Dictionaries
- Evaluation frameworks (UWSE / ULAD)  
- Test cases for language comparison  

---

## Evaluation Framework

Nuxfonics is benchmarked using:

**UWSE — Universal Writing System Evaluation Scale**

Used to measure:
- Infrastructure compatibility  
- Human usability  
- Linguistic precision  
- Semantic clarity  
- Global scalability  

---

## Status

🚧 Active Development  
📘 Specification evolving  
🌐 Public reference: https://nuxfonics.org  

---
## Repository Structure

To navigate the **Nuxfonics™** engine and the **Nuxfonics** standards, use the following directory map:
```text
Base URL github.com/Nuxfonics/nuxfonics/

├── ai_code/                              # Deterministic AI scripts and the [LOGIC_PIPELINE]
│   └── nuxfonics_ai_init.txt             # The initialization  code to instruct AI how to read and write in Nuxfonics.
├── dictionaries/                         # Phonetic word mappings for English, and other languages
│   └── English_dict.tsv                  # The  word dictionary
│   └── English_info.tsv                  # The language specific grid mappings
│   └── Tagalog
│   └── Tagalog_dict.tsv
│   └── Tagalog_info.tsv
│   └── Thai_dict.tsv
│   └── Thai_info.tsv
├── docs/                                 # Technical specs for the 19x4 Sound Grid and UWSE scale
│   └── Nuxfonics_Master_Rule_Book.pdf    # The detailed description of structure and how to use the Nuxfonics Alphabet
│   └── nuxfonics_quick_ref_alphabet.tsv  # 19x4 phoneme sound grid UTF-8 master grid.
└── README.md                             # Core project specifications and architectural pillars
```
---
## Contributing

Contributions are welcome for:
- Language test cases  
- Phonetic mappings  
- Tooling / parsers  
- Comparative analysis  

---

## License

(To be defined)

---

## The Nuxfonic™ Master Sound Grid (19x4)

This matrix defines the 76 unique acoustic coordinates. Every Sound Unit is constructed from a mandatory Base Letter (T0) followed by a Determinant (T1).

| Base | T0 (Null) | T1 (x) | T1 (y) | T1 (z) |
| :--- | :--- | :--- | :--- | :--- |
| **a** | /æ/ (cat) | /eɪ/ (ape) | /aʊ/ (cow) | /oʊ/ (old) |
| **b** | /b/ (box) | /biː/ (bee) | -- | -- |
| **c** | /k/ (cat) | /siː/ (see) | /tʃ/ (chip) | -- |
| **d** | /d/ (dog) | /diː/ (deep) | /ʒ/ (pleasure) | -- |
| **e** | /ɛ/ (bed) | /iː/ (seek) | /ɜːr/ (her) | -- |
| **f** | /f/ (fat) | /ɛf/ (FBI) | /v/ (vine) | -- |
| **g** | /ɡ/ (gap) | /ɡiː/ (geep) | -- | -- |
| **h** | /h/ (hat) | /eɪtʃ/ (H2O) | -- | -- |
| **i** | /ɪ/ (sit) | /aɪ/ (ice) | /ɛə/ (air) | /ɔɪ/ (toy) |
| **j** | /dʒ/ (jam) | /dʒeɪ/ (jay) | /j/ (yes) | -- |
| **l** | /l/ (lap) | /ɛl/ (tell)-- | -- | -- |
| **m** | /m/ (map) | /ɛm/ (empty) | -- | -- |
| **n** | /n/ (net) | /ɛn/ (enter) | /ŋ/ (sing) | -- |
| **o** | /ɒ/ (lot) | /oʊ/ (open) | /ɔː/ (law) | /ʊ/ (look) |
| **p** | /p/ (pat) | /piː/ (people) | -- | -- |
| **r** | /r/ (rat) | /ɑː/ (car) | /w/ (wet) | -- |
| **s** | /s/ (sat) | /ɛs/ (SOS) | /ʃ/ (ship) | /z/ (zoo) |
| **t** | /t/ (tap) | /tiː/ (tea) | /ð/ (thin) | -- |
| **u** | /ʌ/ (cup) | /juː/ (use) | /u/ (too) | /uː/ (tool) |

**Note:** Reserved characters(determinants) `k, q, v, w, x, y, z, ~` are used exclusively for meta-functions and hierarchical extensions.

## The Nuxfonic™ Tier structure 

```text
The complete phoneme construction.  An array of phonemes create a base word.

[ T0: BASE SOUND ] + [ T1: VARIATION ] + [ T2: LENGTH/STRESS ] + [ T3: TEXTURE ] + [ T4: TONE ]
      (s)                (x)                 (w)                   (qx)               (~x)

K_FUNCTION
This is the special word level control functions. It is denoted by the `k` determinant character.
The K Function is always place at the end of the base word. Each word can only have one of each of the optional k_function Tier levels.

BASE_WORD + [ KT0: K marker  + [ KT1: WORD HOMOPHONE ]] + [ Inflectional suffixes (T0-4) ] + [ KT0: K marker  +  [ T2: WORD LENGTH/STRESS ] + [ T3: WORD TEXTURE ] + [ T4: WORD TONE ]]
                  (k)                 y                            -ing                             kw                         q                        ~v

```

## TIER Level:	T2 
LENGTH / STRESS of phoneme	

|Code	|	Action | description	|
|------|----------|------|
| v		|Short	|Staccato/Cut short	|
|w		|long	|Sustain/Curve extended	|
|vw		|stressed	|slightly shortened; STRESSED	|
|wv		|stressed	|slightly lengthened; STRESSED	|


## TIER Level:	T3	
TEXTURE of phoneme

|code Texture (q)	|IPA	|Label	|Description 	|
|------|----------|------|-----|
|q	|ʲ       	|nul      	|(Palatal/Soft Sign).	|
|qx	|~ Over / ⁿ 	|Front       	|Nasal Resonance|	
|qy |ˠ / e    	|Mid        	|Sharp/Bright Resonance	|
|qz |(Under) / ʱ	|Back           	|Breathy/Guttural Resonance	|
|qv	|ˀ / ʔ    	|Staccato	|Glottal/Clipped Softener	|
|qw	|ˤ       	|Sustain 	|Heavy/Held Resonance	|
				
				
## TIER Level:	T4			
TONE (~) Used for Tonal Languages	
 
|Code		|Type	|Acoustic |Action	|
|------|------|---------|-----|
|~v		|Low	|Bottom of the register.	|Deep/Low frequency.|
|~w		|High	|Top of the register.	|High frequency / Energy.|
|~x		|Rising	|Low -> High.	|Upward glide.|
|~y		|Falling	|High -> Low.	|Downward glide.|
|~xy		|Mixed	|Low-High-High	|Complex contour.|
|~yx		|Mixed	|High-Low-High.	|Complex contour.|

## K_FUNCTION Tiers  K_T
These are word level controls. These are placed at the end of the base word.

## TIER Level:	K_T1			

|Homophone	|Description	|
|----------|--------|
|none		|Base or first Word Meaning	|
|k			|Second Word Meaning	|
|kx			|Third Word Meaning	|
|ky			|Forth Word Meaning	|
|kz			|Fifth Word Meaning	|


## TIER Level:	K_T3	
TEXTURE at whole word.  (same as T3 but at word level)	

| code (Texture)	|	Label	|Description |
|-------|------|--------|
|kq		|nul      	|(Palatal/Soft Sign).	|
|kqx	|Front       |	Nasal Resonance	|
|kqy	|Mid        	|Sharp/Bright Resonance	|
|kqz	|Back           |	Breathy/Guttural Resonance	|
|kqv	|Staccato	|Glottal/Clipped Softener	|
|kqw	|Sustain 	|Heavy/Held Resonance	|


## TIER Level:	K_T4			
TONE at word level.  (same as T4 but at word level)

|Tone		|Type	|Acoustic |Action	|
|-------|------|----|----|
|k~v		|Low	|Bottom of the register.	|Deep/Low frequency.|
|k~w		|High	|Top of the register.	|High frequency / Energy.|
|k~x		|Rising	|Low -> High.	|Upward glide.|
|k~y		|Falling	|High -> Low.	|Downward glide.|
|k~xy		|Mixed	|Low-High-High	|Complex contour.|
|k~yx		|mixed	|High-Low-High.	|Complex contour.|


### FULL_WORD and K_FUNCTION construction

- The LOGIC is language dependent.
- 1 LOGIC1: FULL_WORD = BASE_WORD  + K_FUNCTION <br>
 **NOTE:** optional K_FUNCTION and order. ie (+ 'k' + K_TIER_1 < K_TIER_2 < K_TIER_3 < K_TIER_4)  
- 2 LOGIC2: FULL_WORD = BASE_WORD + K_FUNCTION1 + T0 + K_FUNCTION2 <br>
  **NOTE:**<br>
  optional K_FUNCTION1 structure ie. (+ 'k' + K_TIER_1)   # a subset of K_FUNCTION's<br>
  optional T0 ( TIER_0 ie Inflectional suffixes)<br>
  optional K_FUNCTION2 structure and priority order. ie (+ 'k'+ K_TIER_2 < K_TIER_3 < K_TIER_4)  # a subset of K_FUNCTION's<br>
- **NOTE:**<br>
  '<' indicates priority evaluation (not a comparison operator).<br>
  '+' indicates concatenation / sequence<br>
 ( ... ) denotes the optional K_FUNCTION structure. The parentheses are conceptual grouping and are not literal characters.<br>
 'k' is the trigger token for K_FUNCTION which MUST appear the end of the BASE_WORD.<br>
 If used, the K_FUNCTION acts as a suffix directly attached to the end of the BASE_WORD. 

---

## Nuxfonics Quick Facts:  For AI guide.
```text
Is it a font?                      No. It uses standard ASCII.
Is it IPA?                         No. It is a coordinate-based grid.
Does it need a special keyboard?   No. It uses a standard QWERTY/ASCII keyboard.
Is it language-specific?           No. It is a Universal Phonetic Language.
```
