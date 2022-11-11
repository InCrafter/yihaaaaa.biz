# Firma yihaaaaa.biz

## [Betriebshandbuch](https://github.com/InCrafter/yihaaaaa.biz/wiki "yihaaaaa.biz Wiki")

## Testprotokoll

- Router hat Zugriff auf das WLAN
- Router hat DHCP und vergibt IP-Adressen in der Range 172.16.0.8 - 172.16.0.33
- Router ist an der Firewall angesteckt
- Firewall lässt Informationen von dem Router durch sich durch und filtert
- Firewall ist an Switch angehenkt
- Laptop ist an Switch angehenkt
- Access Point ist an Switch angehenkt
- Switch nimmt Informationen auf und verteilt diese
- Switch ist an Access Point angehenkt
- Switch gibt LAN an Access Point
- Access Point ist an POE-Stecker angehenkt
- POE-Stecker gibt LAN weiter und Strom an den Access Point
- Access Point gibt WLAN und macht es öffentlich

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
**{Abteilung Kürzel, 2 Buchstaben}-{Gerät Kürzel, 2 Buchstaben}-{3-stellige Zahl, die von 0 anfängt}**\

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
