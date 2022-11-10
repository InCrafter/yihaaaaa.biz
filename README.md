# Firma yihaaaaa.biz

## [Betriebshandbuch](https://github.com/InCrafter/yihaaaaa.biz/wiki "yihaaaaa.biz Wiki")

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
| PCs          | Apple MacBook Pro – Late 2021   | 27     | 179'091 CHF |
| Switch       | Netgear GS108T Network Switches | 4      | 259 CHF     |
| Router       | Ubiquite EdgeRouter X           | 1      | 59 CHF      |
| Access point | Ubiquiti Access Point           | 1      | 199 CHF     |
| Firewall     | PC Engine apu2c4                | 1      | 304 CHF     |
| **Total**     |        |       | 179’912 CHF     |

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

## Namenskovention

**{Abteilung}-{Gerät Abkürzung}-{3 Stellige Zahl}**
Beispiel: **PR-RT-001**
**Produktion-Router-001**

weitere Beispiele:
PR-FW-001 (Firewall)
PR-WS-001 (PC)
PR-SW-001 (Switch)
PR-AP-001 (Access Point)
PR-PR-001 (Drucker)

## Netzwerkplan

[![plan](/Planungsarbeiten/Netzwerkplan.png)](https://github.com/InCrafter/yihaaaaa.biz/blob/main/Planungsarbeiten/Netzwerkplan.png)
