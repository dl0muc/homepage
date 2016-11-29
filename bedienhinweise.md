---
layout: page
title: Bedienhinweise zum Shack
permalink: /dl0muc/bedienhinweise
categories: dl0muc
---

## SDR Empfaenger

<del>Auf dem Dach ist ein BeagleBone Black mit RTL-SDR Dongle an einer Diamond D-3000N Discone (http://www.diamondantenna.net/d3000n.html) installiert.
Samples können über rtl_tcp verschickt werden und auf einem Client Rechner mit z.B. GnuRadio oder gqrx weiterverarbeitet werden.</del>

Aufgrund eines Wasserschadens ist der SDR leider gerade nicht auf dem Dach. Wird demnächst ersetzt.

##  Shackrechner

Der Shackrechner ist aktuell ein HP mit einem Core2 und Debian 8.

User und PW bitte beim Shackbenutzer des Vertrauens erfragen.

Admin sind aktuell chris007 (DL1COM) und andz (DC1MIL)
### Logbuchsoftware CQRLOG

Zum loggen von QSOs verwenden wir [CQRLOG](http://www.cqrlog.com/) \\
Das Programm verbindet sich automatisch mit dem IC-9100 um Frequenz und Betriebsart einzutragen.

**Hinweise zum Eintragen von QSOs:**
* Bitte ins Kommentarfeld "op: <RUFZEICHEN>" eintragen, damit eine Zuordnung der QSOs zum jeweiligen Op möglich ist.
* qsl_s Feld: "SB" bedeutet "Send via bureau", die QSL Karte muss also noch erstellt/verschickt werden. "B" bedeutet "Sent via bureau", die QSL Karte ist also bereits erstellt/verschickt.

## IC-9100

* Der IC-9100 besitzt einen eingebauten Tuner. Für optimales SWR darauf achten, dass dieser aktiv ist ("TUNE" Indikator wird im Display angezeigt).

### Digimodes mit fldigi

Um mit dem Stationsrechner Digitalbetrieb mit dem Programm [fldigi](http://www.w1hkj.com/Fldigi.html) (Konfiguriert wie [hier](https://sites.google.com/site/ubuntuhamoperator/blog/ic-9100usbfldigiset-up) beschrieben) zu machen, muss der IC-9100 folgendermaßen eingestellt sein:  
* **Betriebsmodus**: SSB (und zwar IMMER USB, egal in welchem Band), evtl. SSB Taste lange halten um in "D" Modus (schmalbandiger Rx-Filter) zu kommen
* Darauf achten, dass keine Sprachkompression o.ä. aktiviert ist.
* **Option 58** (Data Off Mod): "USB" ("Menu"-Taste lange halten, um ins Konfigurationsmenü zu kommen). \\ (Dies bewirkt, dass im nicht-Datenmodus die zu sendenden Daten über die USB Audioschnittstelle angenommen werden.)
* **Option 56** (USB Mod Level) Hier muss das USB-Gain so angepasst werden, dass der Sender gerade nicht in den ALC geht (z.B. 32% bei PSK31 oder 50% bei SSTV. Gerne darf auch noch weiter herunter gegangen werden, damit die abgegebene Leistung nur ca. 25 Watt beträgt. Digimodes benötigen kein qro).
  
**Denn:** fldigi moduliert die jeweilige Betriebsart bereits selbst in ein Audiosignal, das dann über die USB-Audio Schnittstelle zum Transceiver geschickt wird.

**Hinweis**: Bitte nach dem Digitalbetrieb bitte Option 58 wieder auf "MIC" konfigurieren, damit der nächste Operator wieder mit dem Mikrofon arbeiten kann.

### WSPR

TRX Einstellungen siehe fldigi (Digimode Betrieb; Data Off Mod USB, immer USB)

* Aufruf der Software: *wspr*
* Stationsparameter wie [hier](http://www.wsprnet.org/drupal/node/3428) beschrieben wählen (19200, /dev/USB0, 8 Daten, 2 (!) Stoppbits, Handshake: None -C ptt_type=RIG).
* Rx Noise sollte auf ca. 0 dB eingestellt sein.
* Ein USB Mod Level von 40% entspricht etwa 40 dBm.
* Audio Level mit *pavucontrol* regulieren, so dass nichts übersteuert.


### SSTV mit qsstv

* Um mit [qsstv](http://users.telenet.be/on4qz/qsstv/index.html) SSTV (z.B. 14,230 MHz) zu empfangen, einfach im Receive-Reiter auf Receive drücken.
* Um zu senden, im Sende-Reiter ein Bild öffnen und einen passenden Modus wählen (z.B. Scottie 2). Anschließend ins "TO" Feld "CQCQCQ" bzw. den gewünschten Empfänger eintragen.
