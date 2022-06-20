# SmokeHouse_1.1
 
Witam,

Zmiany w stosunku do wersji 1.0

1. Dodane PWM do wentylatora zadymiacza.
2. Dodany czujnik temperatury wyrobu.
3. Dodany pomiar temperatury dymu (MAX6675)
3. Zmiana GPIOS

- linia 108 - int LedGreen = 26; - dioda zielona - urządzenie włączone
- linia 109 - int LedRed = 25; - dioda czerwona - awaria
- linia 119 - int outputGPIOs[NUM_OUTPUTS] = {14, 18, 27, 40, 41}; - pin 14 - wentylator suszenia (12V poprzez mosfet) pozostałe nie używane.
- linia 127 - const int ledPin1 = 12; - PWM pod wentylator zadymiacza (5V przez mosfet)
- linia 194 - const byte RelayPin = 17; - SSR grzania;
- linia 224 - int SO = 23;
		int CS = 5;
		int sck = 19; - MAX6675 - temperatura dymu

- linia 260 - const int oneWireBus = 13; - linia DS18B20 - czujnik temperatrury
- linia 483 - ThermistorPin = 34; pin termistora temperatury wyrobu - termistor typu 10k

W interfejsie graficznym - wyłącznik zadymiacza nie działa - sterowanie tylko suwakiem PWM.



