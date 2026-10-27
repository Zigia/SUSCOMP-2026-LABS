# Week 2 – Personal CO2 Footprint Estimation

**Author:** Žiga Rogelj (GitHub: Zigia)
**Date:** 27 October 2026

Carbon intensity of Slovenian electricity: **166 g CO2e/kWh** (ARSO, 2023, https://kazalci.arso.gov.si/en/node/63390).

## Inventory

| # | Device | Owned since | Supporting equipment |
|---|--------|-------------|----------------------|
| 1 | MacBook Air M2 (2022, 256 GB) | 14 Nov 2024 | 30 W USB-C adapter |
| 2 | iPhone 13 Pro 512 GB | Nov 2021 | 20 W USB-C charger (battery replaced twice) |
| 3 | HomePod (2nd gen) – also HomeKit hub | 15 Sep 2023 | mains cable |
| 4 | UniFi U6 Pro access point | 1 Mar 2022 | PoE from switch |
| 5 | Toshiba 1 TB HDD for NAS/NVR (backups + camera recording) | ~Aug 2023 (27 765 power-on hours) | NAS/NVR enclosure |
| 6 | 2 × Shelly Plus 2PM (roller-shutter controllers, Home Assistant) | 30 Oct 2023 | 2 shutter motors |

---

## 1. MacBook Air M2

![MacBook Air](photos/macbook.jpg)

**Usage:** ~3 h/day (≈ 21 h/week, ≈ 1 095 h/year), the rest in sleep; mostly on the desk, plugged in.

| Device | Active power when in use | Power in idle/sleep mode | Power when turned off | kWh daily | kWh weekly | kWh yearly | kg CO2e yearly |
|--------|--------------------------|--------------------------|-----------------------|-----------|------------|------------|----------------|
| MacBook Air M2 | 10 W | 0.3 W (sleep, 21 h) | 0 W | 0.036 | 0.254 | 13.3 | 2.2 |

Lifetime so far (1.95 years): 26 kWh → 4.3 kg CO2e.

---

## 2. iPhone 13 Pro 512 GB

![iPhone](photos/iphone.jpg)

**Usage:** ~4 h screen time/day; ~1 950 charge cycles over 5 years (3 batteries) = 390 cycles/year × 11.97 Wh / 0.85 charger efficiency.

| Device | Active power when in use | Power in idle mode | Power when turned off | kWh daily | kWh weekly | kWh yearly | kg CO2e yearly |
|--------|--------------------------|--------------------|-----------------------|-----------|------------|------------|----------------|
| iPhone 13 Pro | ≈ 2.5 W | ≈ 0.13 W | 0 W | 0.015 | 0.105 | 5.5 | 0.9 |

Lifetime so far (5 years): 27.5 kWh → 4.6 kg CO2e.

---

## 3. HomePod (2nd gen)

![HomePod](photos/homepod.jpg)

**Usage:** music 1–2 h *per week* at ~30 % volume; powered 24/7 as the HomeKit hub.

| Device | Active power when in use | Power in idle mode | Power when turned off | kWh daily | kWh weekly | kWh yearly | kg CO2e yearly |
|--------|--------------------------|--------------------|-----------------------|-----------|------------|------------|----------------|
| HomePod 2 | 8.3 W (playback) | 1.0 W (low-power mode, Apple PER) | n/a (never off) | 0.027 | 0.189 | 9.9 | 1.6 |

Lifetime so far (3.1 years): 31 kWh → 5.1 kg CO2e. 95 % of the energy goes into standby, 5 % into music.

---

## 4. UniFi U6 Pro access point

![U6 Pro](photos/u6pro.jpg)

**Usage:** 24/7 since 1 Mar 2022.

| Device | Active power when in use | Power in idle mode | Power when turned off | kWh daily | kWh weekly | kWh yearly | kg CO2e yearly |
|--------|--------------------------|--------------------|-----------------------|-----------|------------|------------|----------------|
| UniFi U6 Pro | 8.5 W | 8.5 W (no idle state) | n/a | 0.204 | 1.428 | 74.5 | 12.4 |

Lifetime so far (4.66 years): 347 kWh → 58 kg CO2e.

---

## 5. Toshiba 1 TB HDD for NAS/NVR

![Toshiba HDD](photos/hdd.png)

**Usage:** 24/7, continuously recording cameras and backups. SMART data: 27 765 power-on hours (3.17 years), 7 200 rpm, 46 °C, 0 bad sectors.

| Device | Active power when in use | Power in idle mode | Power when turned off | kWh daily | kWh weekly | kWh yearly | kg CO2e yearly |
|--------|--------------------------|--------------------|-----------------------|-----------|------------|------------|----------------|
| Toshiba DT01ACA100 | 6 W (read/write) | 4.5 W (spinning idle) – never reached | n/a | 0.144 | 1.008 | 52.6 | 8.7 |

Lifetime so far (3.17 years, measured): 167 kWh → 28 kg CO2e.

---

## 6. 2 × Shelly Plus 2PM (roller-shutter controllers)

![Shelly Plus 2PM](photos/shelly.jpg)

**Usage:** permanently powered since 30 Oct 2023, Wi-Fi to Home Assistant; each shutter moves ~0.75×/day (motor ~300 W for ~25 s per movement).

| Device | Active power when in use | Power in idle mode | Power when turned off | kWh daily | kWh weekly | kWh yearly | kg CO2e yearly |
|--------|--------------------------|--------------------|-----------------------|-----------|------------|------------|----------------|
| 2 × Shelly Plus 2PM | 1 W each | 1 W each (standby) | n/a | 0.048 | 0.336 | 17.5 | 2.9 |
| 2 × shutter motors (the useful work) | 300 W | 0 W | 0 W | 0.006 | 0.044 | 2.3 | 0.4 |

Lifetime so far (3 years): 53 kWh → 8.7 kg CO2e. The controllers use ~8× more energy than the motors they control.

---

## Summary

| Device | Power (typ.) | Hours/day | kWh daily | kWh weekly | kWh yearly | kg CO2e yearly | Share |
|--------|--------------|-----------|-----------|------------|------------|----------------|-------|
| iPhone 13 Pro | 2.5 W | 4 | 0.015 | 0.105 | 5.5 | 0.9 | 3.2 % |
| HomePod 2 | 1.0 W | 24 | 0.027 | 0.189 | 9.9 | 1.6 | 5.7 % |
| MacBook Air M2 | 10 W | 3 | 0.036 | 0.254 | 13.3 | 2.2 | 7.7 % |
| 2 × Shelly Plus 2PM | 2 W | 24 | 0.048 | 0.336 | 17.5 | 2.9 | 10.1 % |
| Toshiba 1 TB HDD | 6 W | 24 | 0.144 | 1.008 | 52.6 | 8.7 | 30.4 % |
| UniFi U6 Pro | 8.5 W | 24 | 0.204 | 1.428 | 74.5 | 12.4 | 43.0 % |
| **Total** | | | **0.47** | **3.32** | **173.3** | **28.8** | 100 % |

Household comparison (yearly): washing machine 80–150 kWh, fridge 70–120 kWh, 100 W TV at 4 h/day ≈ 110 kWh. One Wi-Fi access point (74.5 kWh) uses about as much as a fridge; the phone and laptop I actually use every day (~19 kWh together) use less than a fifth of one. The whole inventory (~173 kWh) is about 3.5 % of the ~5 000 kWh per person per year quoted in the lecture.

## Reflections

The ranking is the reverse of how much I *use* each device. The phone and laptop are in my hands for hours every day and are at the bottom; the three devices at the top – access point, hard disk, shutter relays – are ones I never consciously use at all. They have no idle state and no off state, so even 1–8.5 W turns into 17–75 kWh/year simply because they run 8 760 hours a year. Cumulative energy is driven by powered-on time, not by work done: the hard disk's own SMART counter shows 27 765 hours and 167 kWh for a single drive, and the Shelly relays spend ~8× more energy waiting for a command than the shutter motors spend moving.

Battery devices are at the other extreme because battery life is a selling point, so they are engineered for low power: five years of iPhone use cost less electricity than four months of the access point. The HomePod sits in between – a personal device that behaves like infrastructure (always on as a HomeKit hub), kept to ~10 kWh/year only by Apple's low-power mode.

The practical lesson: my charging habits are irrelevant; what matters is every box that is on 24/7. Each of those is a 10–75 kWh/year decision, and the question to ask is not "how efficient is it?" but "does it need to be on all the time?"

### Extension: energy of network traffic

My devices move roughly 150 GB/month ≈ 1 800 GB/year through the Internet. Using ~0.015 kWh/GB for core and access networks (Aslan et al. 2018, extrapolated to 2026): **≈ 27 kWh/year ≈ 4.5 kg CO2e** – twice the laptop and five times the phone, but only about a third of what my own access point consumes to serve that same traffic (74.5 kWh), because the upstream network is shared by millions of users while my equipment serves only me. Against household appliances, the traffic energy is about a quarter of a fridge; the access point alone equals one. Data-centre energy behind the services is not included.

## Sources

- ARSO, Intensity of GHG emissions from electricity production, 2023: https://kazalci.arso.gov.si/en/node/63390
- Apple Product Environmental Reports: MacBook Air M2 (June 2022), iPhone 13 Pro (Sept 2021), HomePod 2nd gen (Jan 2023) – power figures
- Ubiquiti U6 Pro datasheet; Toshiba DT01ACA100 datasheet + SMART data from the NAS; Shelly Plus 2PM datasheet
- NEA, Electricity Consumption Around the Home
- Aslan, J. et al. (2018). Electricity intensity of Internet data transmission. *Journal of Industrial Ecology*, 22(4), 785–798.
- Lecture 2 slides, Sustainable Computing, UL FRI
