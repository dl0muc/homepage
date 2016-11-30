---
layout: page
title: APRS Digipeater
permalink: /db0muc/aprs
categories: [project, db0muc]
project: 'APRS'
---

Unser APRS Digipeater läuft seit dem 13. November 2016 im Testbetrieb. Siehen auch [DB0MUC auf aprs.fi](http://aprs.fi/DB0MUC).

{% include image.html url="/assets/pages/aprs_01.jpg" caption="APRS Digipeater" width=600 align="center" %}
{% include image.html url="/assets/pages/aprs_02.jpg" caption="Geöffnetes Gehäuse beim Aufbau" width=600 align="center" %}
<br style="clear: both;"> 

## Allgemeine Informationen

| Sysops           | DC1MIL, DL1COM       |
| HAMNET-IP        | 44.225.22.133        |
| URL              | aprs.db0muc.ampr.org |
| Frequenz         | 144.800 MHz          |
| Ausgangsleistung | 6W                   |

## Technische Daten

| TRX     | Motorola MC-Micro mit [MCmega-Hack von DG1YFE](http://mc70.stus-disco.de/mods/cpu-modboard.html) |
| TNC     | [TNC-Pi](http://tnc-x.com/TNCPi.htm) |
| Rechner | Raspberry Pi 3 mit Raspbian |
| Spannungsversorgung | 12V Netzteil mit Vorbereitung zur Not-Batterieversorgung |
| Gehäuse | 19" 2HE |

## Software

* [APRX](http://ham.zmailer.org/oh2mqk/aprx/) als APRS Digipeater
* [APRSC](http://he.fi/aprsc/) als lokaler APRS-IS
* [Sopel](https://github.com/sopel-irc) als IRC-Bot für zukünftige Funktionen

Konfigurationsfiles finden sich auf [Github](https://github.com/dl0muc/db0muc_digipeater).

## Aktueller Funktionsumfang

Im Moment befindet sich der APRS-Digi in unserem Shack und ist an die X-200 auf dem Dach angebunden. Zukünftig soll der Digi zusammen mit weiter Hardware im Hausmeisterraum installiert werden.

### APRX ist als Digipeater eingerichtet
  * Sendet alle 10min Beacon über die Funkschnittstelle
  * Alle 20min Telemetrie über den IS
  * Repeated direkt empfangene Pakete über die Funkschnittstelle und IS

### APRSC als lokaler IS

APRX kommuniziert nicht direkt mit einem IS im HAMNET/Internet, sondern zunächst mit einer lokalen Instanz von APRSC welcher dann die Pakete zu einem IS im HAMNET weiterleitet.

Dies hat den Grund, da APRSC nur mit einem IS direkt kommunizieren kann. Zu APRSC kann man sich jedoch mit mehreren Clients verbinden. So können z.B. unter Verwendung des [Python APRS Packages](https://pypi.python.org/pypi/aprs/4.0.0) die vom APRX empfangenen Pakete weiterverarbeitet werden.

## Zukünftiger/Geplanter Funktionsumfang

* Versenden des aktuellen Clubstatus (Down, Closed, Member, Public) über den Beacon
* Weiterleitung von empfangenen Direktnachrichten an den IRC-Channel
* Versenden der Daten der (noch zu bauenden) Wetterstation
* Fernsteuern von bestimmten Funkstationsfunktionen
* Weiterleitung von APRS Direktnachrichten an diverse HAMPAGER
