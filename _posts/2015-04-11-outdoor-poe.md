---
layout: post
title:  "Outdoor PoE Switch"
author: "DC1MIL"
date:   2015-04-11 00:00:00
categories: [logbuch, post]
project: [Clubstation, Empfaengr, HAMNET]
---

Da auf dem Dach immer mehr Netzwerkfähige Geräte installiert werden, wurde die Verkabelung zwischen Mast und Aufzugsraum immer aufwendiger. Deshalb haben andz (DC1MIL) und Chris (DL1COM) einen VLAN fähigen PoE-Switch in einem Wetterfesten Schaltschrank untergebracht.

{% include image.html url="/assets/posts/post031.jpg" caption="Outdoor PoE-Switch" width=300 align="left" %}
<br style="clear: both;"> 

Dieser wurde daraufhin von andz, Chris und Markus am Mast montiert. Auch eine Outdoor-Steckdose für längere Aufenthalte auf dem Dach wurde mit Integriert.

Im selben Zug wurde ein Freifunk-Node installiert, welcher unseren benachbarten Massmannpark seit dem mit Freifunk versorgt.

{% include image.html url="/assets/posts/post032.jpg" caption="Massmann Freifunk-Node" width=300 align="left" %}
<br style="clear: both;"> 

Leider mussten wir unseren Empfaengr vorrübergehen abbbauen. Es gab zum einen Co-Site Probleme mit der VHF/UHF Antenne, welcher den Eingansfilter des RTL-SDR zerstörten. Zum andderen war das Wetterfeste gehäuse anscheinend nicht gut abgedichtet, weshalb dieses voll mit Wasser lief. Der Beaglebone konnte durch ein Ultraschallbad mit destiliertem Wasser wieder zum leben erweckt werden.

Durch einen starken Sturm in München gab es einige Schäden. Diese wurden begutachtet:
* Oberer Halter der KW-Antenne leicht verbogen -> Weiter beobachten
* Eine Abstimmspule hat sich gelöst -> Fix offen
* Antenne wurde vorrübergehen vom Shack abgeklemmt
* Mastabdeckung (Gasflaschendeckel) hat sich gelöst -> Ersatz wurde montiert
* Ansonsten keine weiteren Schäden

Auch der HAMNET-Node wurde durch eine Ubiqiti Nanostation ersetzt. Der vorherige Node war mit siner 23dBi Antenne zu überdimensioniert, weshalb es bereits beschwerden der Sysops von DB0TVM gab, da die Eintreffende Feldstärke viel zu hoch war.