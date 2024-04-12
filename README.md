Σταθμοί περιβαλλοντικών μετρήσεων χαμηλού κόστους - Δυτική Μακεδονία
https://maps.sensor.community/?nowind&nolabs#9/40.6045/21.6168

Το μοντέλο του κιτ που θα διερευνηθεί είναι: 
https://nettigo.eu/products/nettigo-air-monitor-kit-bme-0-3-3-std-soldered-build-your-own-smog-sensor

Λίγο προσοχή στον αισθητήρα, και στη σφράγιση της οπής με θερμοσιλικονη  
https://docs.nettigo.pl/en/nam/033/nam-bme280-033

Οδηγίες συναρμολόγησης του kit:
https://docs.nettigo.pl/en/nam/033/nam-033-std-fa

Εάν ο μικροελεγκτής ESP8266: 
+ **Δεν** συνδεθεί στο καθορισμένο WiFi μετά από 20 δευτερόλεπτα, ενεργοποιείται ένα A.P. με default password: **nettigo.pl** και SSID: (**NAM-XXXXXX** το XXXXXX είναι το ChipID του ESP8266). Μετά τη σύνδεση σε αυτό το σημείο πρόσβασης. Διεύθυνση παραμετροποίησης:  http://192.168.4.1/
+ **Συνδεθεί** στο καθορισμένο WiFi. Η διεύθυνση παραμετροποίησης (με σύνδεση στο ίδιο τοπικό δίκτυο) είναι: http://**NAM-XXXXXX**.local/ (Το XXXXXX είναι το ChipID του ESP8266 - Είναι τυπωμένο σε λευκό αυτοκόλλητο πάνω στον αισθητήρα SDS011 και αναφέρεται ως **SensorID** - Είναι πιθανό το firewall των windows 11 να μην επιτρέπει την πρόσβαση στην ιστοσελίδα παραμετροποίησης nam-xxxxxxxxxx.local)

##Ρυθμίση της θέσης του αισθητήρα λεπτής σκόνης, και άλλων παραμέτρων:
https://devices.sensor.community/

##Αισθητήρας θερμοκρασίας υγρασίας και πίεσης  
Στη σελίδα https://devices.sensor.community/sensors επιλέγουμε ρυθμίσεις στον αισθητήρα που θέλουμε να παραμετροποίσουμε (ρυθμίσεις του κόμβου), στη διαμόρφωση υλικού επιλέγουμε σωστό τύπο του αισθητήρα που είναι ο **ΒΜΕ280**
![Ρύθμιση στο https://devices.sensor.community/sensors](https://github.com/chzarafidis/pm/blob/main/bme280.png) 

##Watchdog Settings  
Η διεύθυνση παραμετροποίησης (με σύνδεση στο ίδιο τοπικό δίκτυο) είναι: http://**NAM-XXXXXX**.local/config  
![watchdog settings](https://github.com/chzarafidis/pm/blob/main/watchdog.png)  
