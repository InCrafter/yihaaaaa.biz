Welcome to the yihaaaaa.biz user Guide!

# Namenskonvention
\
Die Namenskonvention haben wir in 3 Abschnitte, Abteilung, Gerät-Abkürzung und eine 3-Stellige Zahl, die von 0 anfangt.
**{Abteilung}-{Gerät Abkürzung}-{3-stellige Zahl}**\
\
Beispiele:
PR-FW-001 (Firewall)\
PR-RT-001 (Router)\
PR-WS-001 (PC)\
PR-SW-001 (Switch)\
PR-AP-001 (Access Point)\
PR-PR-001 (Drucker)

# Systemübersicht
![](https://github.com/InCrafter/yihaaaaa.biz/blob/main/Planungsarbeiten/Netzwerkplan.png)\
![](https://github.com/InCrafter/yihaaaaa.biz/blob/main/Planungsarbeiten/Physical.png)

Hierarchie:\
Wi-Fi: Router > Firewall > Switch1 > Access Point\
Kabel: Router > Firewall > Switch1 > Switch2/Switch3/Switch4 > Kabel

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

# Router
IP-Adresse: 172.16.0.1\
Benutzername: ubnt\
Passwort: ubnt

# Firewall
IP-Adresse: 172.16.0.2\
Benutzername: root\
Passwort: opnsense

# Switch
IP-Adresse: 172.16.0.3 - 172.16.0.6\
Passwort: password

# Access Point
IP-Adresse: 172.16.0.7\
Benutzername: admin\
Passwort: admin123\
Wi-Fi Passwort: 12345678
