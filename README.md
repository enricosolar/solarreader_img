#solarreader_img


Meine erstes offizielles solarreader.img 

lauffähig ab Raspberry Pi2B+  , auch Grafana, dort mit USB-Wlan-Adapter oder LAN, 
Mit Hilfestellung ist auch Betrieb über USB möglich.

ab Pi3B+ ist Wlan  und USB-Start über OS integriert
komplett mit Apache2, php7, 
influx V.1.8.10, Grafana 9.3.2, MQTT
Browser Chromium & Mozilla Firefox ESR

6 InfluxDB
solaranzeige
steuerung
solarreader
solarreader1
solarreader2
solarreader3
alle angelegt und in Grafana bekannt gemacht.
Müssen nur in der Konfigurations-GUI aktiviert werden.

Alle Grafana-Stanbdard-Dashboards der solaranzeige enthalten.

Raspberry
user: pi            Passwort: solarreader

Grafana
user: admin     Passwort: solarreader
 
Einfache Automation(x) für 7 Tasmota-Relais mit 1 bis 4 Kontakten integriert
Kann auf Anfrage erweitert werden.

Download mit:

https://solarfanenrico.de/solarreader/solarreader_2022-12-30.img.zip

entpacken und auf microSD ein Laufwerksabbild erstellen
in den Pi stecken und starten
dann 

sudo raspi-config

6 Advanced Options    auswählen

danach

A1 Expanded Filesystem     wählen

dadurch bereitet sich der Pi auf die neue Laufwerksgröße vor.
Den Pi automatisch straten lassen

mit dem Befehl

df -h kann man den Erfolg kontrollieren

bei einer 15 GB SD sieht die erste Antwortzeile so aus
Dateisystem Größe Benutzt Verf. Verw% Eingehängt auf
/dev/root        15G    5,6G    8,1G   41%        /



