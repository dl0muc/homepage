---
layout: page
title: HAMNET
permalink: /db0muc/hamnet
categories: [project, db0muc]
project: 'HAMNET'
---

DB0MUC und DL0MUC sind über [DV0TVM](http://hamnetdb.net/?m=as&q=db0tvm) direkt an das HAMNET angebunden (siehe auch [hamnetdb.net](http://hamnetdb.net/?m=as&q=db0muc))

Wir haben von Jann (DG8NGN) einen /27 IP-Range zugeteilt bekommen (44.149.22.128/27).

Technisch sind wir über eine Strecke im ISM-Band and DB0TVM angeschlossen. Realisiert mit einem [MikroTik QRT5](https://routerboard.com/rb911g-5hpnd-qrt).

## IP Adressen

| IP            | DNS                        | Beschreibung                                               | aktiv |
| ------------- | -------------------------- | ---------------------------------------------------------- | ----- |
| 44.148.10.166 | bb-db0tvm.db0muc.ampr.org  | Routing ISM                                                | ja    |
| 44.149.22.129 | router.db0muc.ampr.org     | HAMNET Router                                              | ja    |
| 44.149.22.130 | db0muc.ampr.org            | VM für Services                                            | ja    |
| 44.149.22.131 | digi.db0muc.ampr.org       | [Digipeater](/db0muc/digipeater.html)                      | nein  |
| 44.149.22.132 | empfaengr.db0muc.ampr.org  | Web-SDR                                                    | nein  |
| 44.149.22.133 | aprs.db0muc.ampr.org       | [APRS-Digi](/db0muc/aprs.html)                             | ja    |
| 44.149.22.137 | p0wer.dl0muc.ampr.org      | Netzwerksteckdose Shack                                    | nein  |
| 44.149.22.138 | shack.dl0muc.ampr.org      | Schackrechner                                              | -
| 44.149.22.139 | contr0l.dl0muc.ampr.org    | Shacksteuerung (Siehe [AVM Funktisch](/projects/avm.html)) | nein  |
| 44.149.22.140 | rot0r.dl0muc.ampr.org      | Rotorsteuerung                                             | nein  |
| 44.149.22.143 | d-amprnet.db0muc.ampr.org  | Routing und DNS Services (veraltet)                        | nein  |
| 44.149.22.144 - \\ 44.149.22.158 |         | User DHCP-Range                                            | -     |


## Netzaufbau

Der Router ist an unserem Antennenmast montiert und über unseren Outdoor PoE Switch mit dem Clubnetz verbunden. Dort wird über die VLAN ID *3900* das Hamnet an mehrere Dosen sowie an die VMs verteilt.

| Dosennummer | Position |
| ----------- | -------- |
| B27         | Shack    |
| B28         | Shack    |