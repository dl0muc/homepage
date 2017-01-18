---
layout: page
title: APRS Digipeater
permalink: /db0muc/aprs/config
categories: [project, db0muc]
project: 'APRS'
---

## Hardware Konfiguration

Der APRS-Digi ist komplett in einem 19" 2HE Metallgehäuse integriert. Auf der Rückseite befinden sich Anschlüsse für die Antenne (N-Buchse), Netzwerk, Kaltgerätestecker sowie ein Powerpol für die Notstromversorgung.

An der Vorderseite befinden sich das Bedienelement für das Motorola MCMicro, 3 LEDs zur Statusanzeige (TX, RX und Power) sowie eine Erdungsbuchse (Bananen). Die bereits in dem Gehäuse verbaute Spannungsanzeige ist derzeit nicht angeschlossen.
Ebenfalls an der Vorderseite sind ein Feinsicherungshalter (4A) und ein Schalter zur Unterbrechung der Spannungsversorgung integriert.

Die TX und RX LEDs werden direkt vom TNC angesteuert, die Power-LED vom Netzeil. 

Als Netzteil wird ein geregeltes 12V Netzteil mit bis zu 120W Ausgangsleistung verwendet. Das MCMicro ist direkt mit der Sekundärseite des Netzeils verbunden, zum Raspberry ist ein. 5V Spannungsregler zwischengeschaltet.
Die Versorgung des TNC erfolgt direkt über den Raspberry. Der Vorbereitete PowerPol Stecker zur Notstromversorgung ist aktuell noch nicht angeschlossen.

Die Verbindung zwischen MCMicro und TNC erfolgt über die [Erweiterungsschnittstelle](http://www.batlabs.com/micro.html) auf der Rückseite des Motorola mit folgender Pin-Konfiguration (Beides 9-pol Sub-D)

| MCMicro        | TNCPi | 
| -------------- | ----- |
| 1 PTT IN       | 4     |
| 2 AUDIO GND    | 6     |
| 3 GND          | 6     |
| 4 SPEAKER +    | NC    |
| 5 SPEAKER -    | NC    |
| 6 MIC IN       | 1     |
| 7 AUDIO OUT    | 5     |
| 8 ALERT OUT    | NC    |
| 9 EMERGENCY IN | NC    |

## Software Installation

Auf dem Raspberry ist Raspbian in der aktuellen Version installiert (Nov. 2016), so konfiguriert, dass kein X-Server gestartet wird.
Die Netzwerkonfiguration wurde auf DHCP belassen.

Der TNC-Pi und das zugehörige AX-25 Interface wurde laut [Anleitung](http://tnc-x.com/TNCPi.pdf) konfiguriert.
APRX wurde über apt installiert und Konfiguriert.
APRSC wurde über die sourcen kompiliert.
Die Konfigurationsfiles für APRX und APRSC finden sich auf [Github](https://github.com/dl0muc/db0muc_digipeater/tree/master/aprs).

Die Sopel Konfiguration ist aktuell noch nicht sinnvoll vorgenommen worden.

Nun wird noch APRX und APRSC über die *rc.local* beim booten des Raspberrys gestartet.

Insgesamt ist die Installation recht straight forward ohne komplexe Änderungen der Grundonfiguration.
