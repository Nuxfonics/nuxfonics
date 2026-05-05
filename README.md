# Nuxfonics  
A practical phonetic encoding system for global real-world use

---

## What is Nuxfonics™?

Nuxfonics is a deterministic phonetic writing system that converts spoken language into consistent, keyboard-friendly text that both humans and AI can read and reproduce accurately.

It is designed for everyday use, written communication, and structured machine-readable data. Using only standard QWERTY characters, it reduces the inconsistency found in traditional phonetic systems (such as IPA) and provides a keyboard-native alternative for representing speech.

It enables:
- Consistent phonetic representation  
- Practical everyday use in real-world environments  
- AI-compatible text processing  
- Cross-language pronunciation recovery  
- Full keyboard compatibility for global usage
- Compatible with existing languages. Can be easily mixed   

Origin of the name

Nuxfonics™ = “New Phonics” written in Nuxfonics. 

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

- Words are encoded based on how they are spoken
- This creates the stable, predictable spelling.
- Not based on historical or visual spelling  
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
| `v, w` | Stress / energy |
| `q` | Texture (articulation) |
| `~` | Tone |
| `k` | Meaning ID (homophone resolution) |

---
### 6. Multi-Axis Encoding
Speech is encoded across multiple dimensions:

| Tier | Function |
|------|--------|
| T0–T1 | Core sound identity |
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
| Knight | nixtk | silent letters removed + ID |
| Night | nixt | base sound |
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

- Core engine rules  
- Sound grid definitions  
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

To navigate the **Nuxfonics™** engine and the **IFA** standards, use the following directory map:
```text
 ├── ai_code/            # Deterministic AI scripts and the [LOGIC_PIPELINE]
 ├── dictionaries/       # Phonetic word mappings for English, and other languages
 ├── docs/               # Technical specs for the 19x4 Sound Grid and UWSE scale
 └── README.md           # Core project specifications and architectural pillars
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
