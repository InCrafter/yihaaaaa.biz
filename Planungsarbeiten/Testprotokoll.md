## Testprotokoll

#### Projekt:yihaaaaa.biz
#### Autor: Arlind, Cenis, Maximilian, Mustafa und Rilind
#### Letzte Änderung: 11.11.2022

### Übersicht
- Router, Switches, Access Point, Firewall, Workstations
- Sonstiges: Alle Manuals von den Geräten, die wir gebraucht haben
- Tester: Arlind, Cenis, Maximilian, Mustafa und Rilind
- Datum: 11.11.2022
#### Testfälle
1. Router DHCP Range konfiguriert
2. Router Routed aussherhalb vom Netzwerk
3. Firewall lässt Informationen von dem Router durch sich durch und filtert
4. Access Point hat die richtige IP und lässt Wi-Fi aus
5. Alle IP-Adressen die vergeben wurden stimmen überein mit unserer Subnetztabelle

### Testfall 1, DHCP Range

1. Erwartetes Ergebnis: Wenn man ein Gerät verbindet, sollte man eine IP zwischen 172.16.0.8 und 172.16.0.33 kriegen.

2. Tatsächliches Ergebnis: Wenn man ein Gerät verbindet, kriegt man eine IP zwischen 172.16.0.8 und 172.16.0.33.

3. Testergebnis Stimmt des tatsächliche Ergebnis mit dem erwarteten Ergebnis überein?: **Ja**

### Testfall 2, Netzwerk zugriff

1. Erwartetes Ergebnis: Wenn man eine Website aufruft sollte man auf die Website gelangen.

2. Tatsächliches Ergebnis: Wenn man eine Website aufruft landen man auch auf diese.

3. Testergebnis Stimmt des tatsächliche Ergebnis mit dem erwarteten Ergebnis überein?: **Ja**

### Testfall 3, Firewall filtert informationen

1. Erwartetes Ergebnis: Wenn ich etwas im Internet mache sollte es zuerst durch die Firewall und umgekehrt.

2. Tatsächliches Ergebnis: Wenn man etwas im Internet macht geht alles zuerst durch die Firewall und umgekehrt.

3. Testergebnis Stimmt des tatsächliche Ergebnis mit dem erwarteten Ergebnis überein?: **Ja**

### Testfall 4, Access Point gibt Wi-Fi aus und funktioniert mit DHCP

1. Erwartetes Ergebnis: Wenn ich mich mit dem Access-Point verbinde sollte ich automatisch eine IP-Adresse kriegen im DHCP Range.

2. Tatsächliches Ergebnis: Wenn ich mich mit dem Access-Point verbinde kirege ich eine IP-Adresse von der DHCP Range.

3. Testergebnis Stimmt des tatsächliche Ergebnis mit dem erwarteten Ergebnis überein?: **Ja**

### Testfall 5, Alle IP-Adressen die vergeben wurden stimmen überein mit unserer Subnetztabelle

1. Erwartetes Ergebnis: Alle IP-Adresse sollten übereinstimmen mit unserer Subnetztabelle.

2. Tatsächliches Ergebnis: Alle unsere IP-Adressen übereinstimmen mit unserer Subnetztabelle. Dies haben wir mach geschaut in dem wir alle Web-Guis geöffnet haben und ipconfig auf unseren Geräten ausgeführt haben.

3. Testergebnis Stimmt des tatsächliche Ergebnis mit dem erwarteten Ergebnis überein?: **Ja**
