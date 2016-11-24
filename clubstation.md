---
layout: page
title: Clubstation
permalink: /clubstation/
---

# Transceiver

## KW
* TS-440S
* IC-9100

## UKW
* Motorola GM1200 UHF
* Motorola MC Micro VHF 

# Antennen

## X-200 144/430 MHz Dual Band Colinear Antenna 

[Thiecom Link](http://www.thiecom.de/diamond/x200.htm) 

| ---------: | :----------------------------------| 
| **Gain**   | 6.5 dB (144 MHz), 9.5 dB (430 MHz) |
| **Power**  | 200 W                              |
| **VSWR**   | 1.5                                |
| **Length** | 2.2 m                              | 
| **Weight** | 1.5 kg                             |

## HF-6V - 5-Band vertical antenna 

[WiMo Link](http://wimo.de/antenna-butternut_e.html#hf6v)

| ----------------------------------: | :---------------------------------------------------------| 
| **Height**                          | 7.9m                                                      |
| **Weight**                          | 5.4kg                                                     |
| **Impedance**                       | 50 Ω with included stub cable                             |
| **VSWR (center of band)**           | 1:1.5 or better on all bands                              |
| **Max. power (PEP)**                | 80,40,20,15,10m: 2000 W  \\ 30m: 500 W                    |
| **Max. wind speed**                 | (w/o guy wires) 129 km/h                                  |
| **Wind load**                       | 0.19 m²                                                   |
| **Bandwidth at VSWR 1:2 or better** | 10m: full band                                            |
|                                     | 15m: full band                                            |
|                                     | 20m: full band                                            |
|                                     | 30m: full band                                            |
|                                     | 40m: 250-300kHz                                           |
|                                     | 80m: 40-100kHz                                            |

# Anbindung zwischen Dach und Shack

## 3x RF (1/2 Zoll)

| Farbcode | Anschluss Dach | Anschluss Shack |
| -------- | -------------- | --------------- |
| rot      | X-200          | IC-9100 2m/70cm |
| grün     | **free**       | **free**        |
| blau     | HF-6V          | IC-9100 KW      |

## 2x CAT6 Ethernetanbindung

| Farbcode | Anschluss Dach | Anschluss NOC   |
| -------- | -------------- | --------------- |
| grün     | **FIXME**      | **FIXME**       |
| blau     | **FIXME**      | **FIXME**       |

## Strom 3 Phasen 5 x 2,5 mm

Sicherungen: **FIXME**

# HAMNET
  * Ubiquiti Nanostation M2 Loco ist auf dem Dach montiert. 
  * Userzugang DB0TVM Süd 2327MHz
  * IP: 192.168.1.20 (DHCP Server) wird über VLAN 3900 im Clubnetz verteilt <del>(aktuell nur auf Dose B8 im Labor)</del>
  * Wir haben ein /27 Netz von der AMPR zugewiesen bekommen. Derzeit wird das Netz integriert und eingerichtet

