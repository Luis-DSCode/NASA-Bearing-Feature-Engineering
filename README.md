# NASA Bearing Dataset FFT-Analyse

In diesem Projekt wird eine explorative Datenanalyse mit Fast Fourier Transform implementiert. 
Es basiert auf dem NASA IMS Bearing Dataset und demonstriert, wie Features daraus extrahiert werden können, 
um Ausfälle mittels Vibrationsdaten zu erkennen.

Die verwendeten Daten stammen aus dem zweiten Test des Datensatzes. Hierin werden Vibrationsmessungen von vier Kugellagern erfasst, 
die konstant bis zu einem Ausfall betrieben wurden.

- 4 Lager
- 20 kHz Abtastrate
- Alle 10 Minuten für 1 Sekunde gemessen
- 984 Messdateien
- Bearing 1 fällt in diesem Test aus



## Verwendung von Fast Fourier Transform

FFT ist ein mathematisches Verfahren, welches ein Signal in einzelne Frequenzkomponenten zerlegen kann.
Für die Zustandsüberwachung von Maschinen kann dies verwendet werden, um Änderungen in Frequenzmustern frühzeitig zu erkennen.
Dies könnte beispielsweise eine Lockerung eines mechanischen Bauteils sein, welches die Vibrationen der Maschine verändert.
