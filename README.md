# Firma yihaaaaa.biz

## [Betriebshandbuch](https://github.com/InCrafter/yihaaaaa.biz/wiki "yihaaaaa.biz Wiki")

## Testprotokoll

#### Projekt: yihaaaaa.biz
#### Autor: Arlind, Cenis, Maximilian, Mustafa und Rilind
#### Letzte Änderung: 11.11.2022

### Übersicht
- Router, Switches, Access Point, Firewall, Workstations
- Sonstiges: Alle Manuals von den Geräten, die wir gebraucht haben
- Tester: Arlind, Cenis, Maximilian, Mustafa und Rilind
- Datum: 11.11.2022

#### Testfälle
1. Router DHCP Range konfiguriert
2. Router routed aussherhalb vom Netzwerk
3. Firewall lässt Informationen von dem Router durch sich durch und filtert
4. Access Point hat die richtige IP und lässt Wi-Fi aus
5. Alle IP-Adressen, die vergeben wurden stimmen überein mit unserer Subnetztabelle

### Testfall 1, DHCP Range

1. Erwartetes Ergebnis: Wenn man ein Gerät verbindet, sollte man eine IP zwischen 172.16.0.8 und 172.16.0.33 kriegen.

2. Tatsächliches Ergebnis: Wenn man ein Gerät verbindet, kriegt man eine IP zwischen 172.16.0.8 und 172.16.0.33.

3. Testergebnis Stimmt des tatsächliche Ergebnis mit dem erwarteten Ergebnis überein?: **Ja**

### Testfall 2, Netzwerk zugriff

1. Erwartetes Ergebnis: Wenn man eine Website aufruft, sollte man auf die Website gelangen.

2. Tatsächliches Ergebnis: Wenn man eine Website aufruft, landet man auch auf diese.

3. Testergebnis Stimmt des tatsächliche Ergebnis mit dem erwarteten Ergebnis überein?: **Ja**

### Testfall 3, Firewall filtert Informationen

1. Erwartetes Ergebnis: Wenn ich etwas im Internet mache, sollte es zuerst durch die Firewall und umgekehrt.

2. Tatsächliches Ergebnis: Wenn man etwas im Internet macht, geht alles zuerst durch die Firewall und umgekehrt.

3. Testergebnis Stimmt des tatsächliche Ergebnis mit dem erwarteten Ergebnis überein?: **Ja**

### Testfall 4, Access Point gibt Wi-Fi aus und funktioniert mit DHCP

1. Erwartetes Ergebnis: Wenn ich mich mit dem Access-Point verbinde, sollte ich automatisch eine IP-Adresse kriegen im DHCP Range.

2. Tatsächliches Ergebnis: Wenn ich mich mit dem Access-Point verbinde, kriege ich eine IP-Adresse von der DHCP Range.

3. Testergebnis Stimmt des tatsächliche Ergebnis mit dem erwarteten Ergebnis überein?: **Ja**

### Testfall 5, Alle IP-Adressen die vergeben wurden stimmen überein mit unserer Subnetztabelle

1. Erwartetes Ergebnis: Alle IP-Adresse sollten übereinstimmen mit unserer Subnetztabelle.

2. Tatsächliches Ergebnis: Alle unsere IP-Adressen übereinstimmen mit unserer Subnetztabelle. Dies haben wir mach geschaut, in dem wir alle Web-Guis geöffnet haben und ipconfig auf unseren Geräten ausgeführt haben.

3. Testergebnis Stimmt des tatsächliche Ergebnis mit dem erwarteten Ergebnis überein?: **Ja**

## Antworten zu den Fragen

#### Was für Geräte werden benötigt, damit diese Netzwerk-Infrastruktur aufgebaut werden kann?

Für unsere Infrastruktur brauchen wir einen Router, einen Accesspoint, Firewall, Switches sowie Workstations.

---

#### Wieviele von den von euch aufgezeigten Geräten benötigt ihr?

Wir brauchen alle Geräte.

---

#### Wie sieht euer möglicher Vorschlag der Subnets aus? Wie gross sind die einzelnen Subnetze?

Unserer bester Vorschlag für eine Subnetzmaske wäre 255.255.255.192, in diesem Subnetz passen 62 Clients

## Stückliste

| Typ          | Name                            | Anzahl | Kosten      |
|--------------|---------------------------------|--------|-------------|
| LAN Kabel    | digitec Ethernet Kabel          | 50     | 965 CHF     |
| PCs          | Apple MacBook Pro – Late 2021   | 27     | 179'091 CHF |
| Switch       | Netgear GS108T Network Switches | 4      | 259 CHF     |
| Router       | Ubiquite EdgeRouter X           | 1      | 59 CHF      |
| Access point | Ubiquiti Access Point           | 1      | 199 CHF     |
| Firewall     | PC Engine apu2c4                | 1      | 304 CHF     |
| **TOTAL**    |                                 | 84     | 180'877 CHF |

## Subnet-table

| Gerät        | Start-IP    | End-IP      |
|--------------|-------------|-------------|
| Netzwerk-ID  | 172.16.0.0  |             |
| Router       | 172.16.0.1  |             |
| Firewall     | 172.16.0.2  |             |
| Switch       | 172.16.0.3  | 172.16.0.6  |
| Access-Point | 172.16.0.7  |             |
| Workstation  | 172.16.0.8  | 172.16.0.33 |
| Reserve      | 172.16.0.34 | 172.16.0.62 |
| Broadcast    | 172.16.0.63 |             |

# Namenskonvention
\
Die Namenskonvention haben wir in 3 Abschnitte, Abteilung, Gerät-Abkürzung und eine 3-Stellige Zahl, die von 000 anfangt.
**{Abteilung Kürzel, 2 Buchstaben}-{Gerät Kürzel, 2 Buchstaben}-{3-stellige Zahl, die von 0 anfängt}**

\
Beispiele:\
PR-FW-001 (Firewall)\
PR-RT-001 (Router)\
PR-WS-001 (PC)\
PR-SW-001 (Switch)\
PR-AP-001 (Access Point)\
PR-PR-001 (Drucker)

## Netzwerkplan

[![logischer Plan](/Planungsarbeiten/Netzwerkplan.png)](https://github.com/InCrafter/yihaaaaa.biz/blob/main/Planungsarbeiten/Netzwerkplan.png)
[![Physischer Plan](/Planungsarbeiten/Physical.png)](https://github.com/InCrafter/yihaaaaa.biz/blob/main/Planungsarbeiten/Netzwerkplan.png)
