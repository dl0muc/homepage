---
layout: page
title: Digipeater
permalink: /db0muc/digipeater
categories: [project, db0muc]
project: 'Digipeater'
---

Unser DB0MUC Digipeater befindet sich aktuell noch in der Planungsphase

## Allgemeines

| HAMNET-IP  | 44.225.22.133        |
| URL        | aprs.db0muc.ampr.org |
| Frequenz   | 438.450 MHz -7.6     |
| Bandbreite | 25kHz                |

## Technische Daten (geplant)

| TX                  | Motorola MC-Micro mit [MCmega-Hack von DG1YFE](http://mc70.stus-disco.de/mods/cpu-modboard.html) |
| RX                  | Motorola MC-Micro mit [MCmega-Hack von DG1YFE](http://mc70.stus-disco.de/mods/cpu-modboard.html) |
| TNC                 | *unbekannt*, zu beginn vmtl. Soundmodem |
| Duplexweiche        | *unbekannt* |
| Rechner             | vermutlich Raspberry Pi 3 |
| Spannungsversorgung | 12V Netzteil mit Vorbereitung zur Not-Batterieversorgung |
| Gehäuse             | 19" 2-4HE |

## Geplanter Funktionsumfang

* automatisch/manuell umschaltbar von 1k2 auf 9k6
* BBS mit Anbindung an diese Homepage, muCCC Kalender etc
* Versenden und Empfangen von APRS und Pagernachrichten
* Anbindung an das HAMNET
* Fernsteuern von Funkstationsfunktionen
* uvm.

## Erste Testinstallation

### Test mit LinBQP (Linux Variante von BQP32)

* Installation auf Rapsberry Pi 3
* Benötigte Libs
  * libconfigg++8
  * libpcap0.8-dev
* Source von [Github](https://github.com/g8bpq/LinBPQ.git)


