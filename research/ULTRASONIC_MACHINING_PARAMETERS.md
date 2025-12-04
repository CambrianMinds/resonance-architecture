# Ultrasonic Machining: Frequency and Parameter Reference

## Modern Ultrasonic Machining Parameters

This document compiles frequency and parameter data from the peer-reviewed literature on ultrasonic and rotary ultrasonic machining (RUM), providing context for how these techniques might relate to ancient stone-working methods.

---

## Operating Frequencies

### Standard Ultrasonic Machining (USM)

| Parameter | Typical Range | Optimal | Source |
|-----------|---------------|---------|--------|
| Frequency | 18-40 kHz | 20-25 kHz | Industry standard |
| Amplitude | 10-100 μm | 15-50 μm | Application dependent |
| Tool rotation | 0 RPM (stationary) | — | Traditional USM |

### Rotary Ultrasonic Machining (RUM)

| Parameter | Typical Range | Optimal | Source |
|-----------|---------------|---------|--------|
| Frequency | 20-40 kHz | 20 kHz | Most common |
| Amplitude | 5-25 μm | 10-15 μm | For hard materials |
| Tool rotation | 1000-8000 RPM | 3000-5000 RPM | For granite/ceramics |

### Friction Reduction Applications

From Luo et al. (2024), *Scientific Reports*:

| Parameter | Value | Effect |
|-----------|-------|--------|
| Frequency | 26 kHz | Optimal for friction reduction |
| Amplitude | 0.35 μm | 89% friction reduction achieved |
| Mode | Longitudinal vibration | Most effective |

### Piezoelectric Granite Weakening

From Saksala et al. (2023), *Rock Mechanics and Rock Engineering*:

| Parameter | Value | Effect |
|-----------|-------|--------|
| Frequency | 274.4 kHz | Natural frequency of sample |
| Voltage | 150 kV | Required for 10% weakening |
| Mode | HF-HV-AC excitation | Piezoelectric actuation |

---

## Material Removal Rates

### Conventional vs. Ultrasonic Drilling in Granite

| Method | Feed Rate | Relative Speed |
|--------|-----------|----------------|
| Modern diamond drill (900 RPM) | 0.0002 in/rev | 1x (baseline) |
| Ancient Egyptian cores (Petrie) | 0.100 in/rev | **500x** |
| Rotary ultrasonic (predicted) | 0.001-0.01 in/rev | 5-50x |

The ancient feed rate exceeds even modern ultrasonic predictions, suggesting either:
1. Higher power/amplitude than modern industrial practice
2. Resonant amplification effects not yet replicated
3. Multi-physics coupling (acoustic + piezoelectric + thermal)

---

## Mechanism: How Ultrasonic Vibration Enhances Machining

### 1. Friction Reduction

- Vibration causes periodic separation between tool and workpiece
- Average friction force drops by up to 89%
- Tool advances during low-friction phase of each cycle

### 2. Impact Fragmentation

- Abrasive particles receive kinetic energy from vibration
- Each particle acts as a micro-hammer
- Material removal through repeated micro-impacts

### 3. Cavitation (in wet machining)

- Ultrasonic vibration in liquid creates cavitation bubbles
- Bubble collapse generates localized high pressure
- Enhances abrasive action and debris removal

### 4. Resonant Weakening (piezoelectric materials)

- Quartz crystals in granite resonate at natural frequencies
- Resonance causes internal stress and micro-fracturing
- Harder quartz becomes easier to remove than softer matrix

---

## Power Requirements

### Modern Industrial USM

| Application | Power | Frequency |
|-------------|-------|-----------|
| Precision machining | 50-500 W | 20 kHz |
| Heavy material removal | 500-2000 W | 20-40 kHz |
| Industrial cutting | 1-10 kW | 20 kHz |

### Acoustic Power Generation (Non-Electric)

Potential ancient power sources:

| Method | Estimated Power | Notes |
|--------|-----------------|-------|
| Single voice (sustained) | 0.001-0.01 W | Fundamental only |
| Resonant chamber amplification | 10-100x | Standing wave formation |
| Coordinated group (100 voices) | 0.1-1 W + resonance | Plus piezoelectric feedback |
| Drums/percussion | 1-10 W | Impulse energy |

The gap between acoustic power and industrial ultrasonic power is significant. However:
- Resonant amplification in tuned chambers could bridge part of the gap
- Piezoelectric feedback from quartz in granite walls adds energy
- Slower processing (hours/days vs. minutes) allows lower power

---

## Key Frequencies for Granite

Based on the literature, these frequencies are significant:

| Frequency | Significance |
|-----------|--------------|
| 20-26 kHz | Optimal friction reduction range |
| 110-117 Hz | Measured resonance of ancient chambers |
| ~274 kHz | Natural frequency for piezoelectric quartz weakening |
| 100-200 Hz | Human voice fundamental range |

**Note**: 110 Hz chambers could generate harmonics. The 24th harmonic of 110 Hz is 2,640 Hz; the 240th harmonic is 26,400 Hz (26.4 kHz)—within the ultrasonic friction reduction range.

---

## Summary

Modern ultrasonic machining operates at:
- **20-40 kHz** for friction reduction and material removal
- **Amplitudes of 5-100 μm** depending on application
- **Power levels of 50 W to 10 kW** for industrial use

The ancient drill cores suggest feed rates 500x modern diamond drilling. This is achievable through ultrasonic assistance, particularly if:
1. Resonant amplification concentrated acoustic energy
2. Piezoelectric response of quartz added to the effect
3. Processing time was not a constraint

---

## Sources

1. Luo, L. et al. (2024). *Scientific Reports*, 14, 22449. — 89% friction reduction at 26 kHz
2. Saksala, T. et al. (2023). *Rock Mechanics and Rock Engineering*, 56, 7655-7672. — Piezoelectric granite weakening
3. Popov, M. (2020). *Frontiers in Mechanical Engineering*, 6, 69. — Vibration-friction contact mechanics
4. Industry references on rotary ultrasonic machining parameters

---

*Compiled for resonance-architecture repository, December 2025*
