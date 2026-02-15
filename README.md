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
 
### Vibrationsdaten aller 4 Lager
![](1.png)

## Verwendung von Fast Fourier Transform

FFT ist ein mathematisches Verfahren, welches ein Signal in einzelne Frequenzkomponenten zerlegen kann.
Für die Zustandsüberwachung von Maschinen kann dies verwendet werden, um Änderungen in Frequenzmustern frühzeitig zu erkennen.
Dies könnte beispielsweise eine Lockerung eines mechanischen Bauteils sein, welches die Vibrationen der Maschine verändert.

Betrachten wir beispielsweise die aufgeteilten Frequenzen von Lager 1 zu beginn des Tests, können wir eine gleichmäßige Verteilung mit einer dominanten Grundfrequenz erkennen: 

Diese Frequenz bei 985.40 Hz mit einer Amplitude von 428.21 ist möglicherweise eine grundlegende Vibration des gesamten Versuchaufbaus.
<img width="1392" height="749" alt="Screenshot 2026-02-16 002741" src="https://github.com/user-attachments/assets/8f5b8121-ea0f-430a-93f2-8f4c86d13a8e" />

  
4 Tage nach dieser Aufnahme verändern sich diese Frequenzen:  
Weitere Frequenzen steigen in ihrer Amplitude und die Vibrationen werden Chaotischer.
<img width="1744" height="900" alt="grafik" src="https://github.com/user-attachments/assets/e7c5ca7b-f7df-4adf-bf65-758685ada462" />

  
Kurz vor dem Ausfall des Lagers steigen diese Frequenzen weiter an:

<img width="1692" height="889" alt="grafik" src="https://github.com/user-attachments/assets/17d5440d-b9e0-4423-98a2-8154fdbbb6fb" />

Durch diese Messungen können die Veränderungen der dominanten Frequenzen und Amplituden als Erkennungsmerkmal eines degradierenden Systems verwendet werden.

## Weitere Features
Neben FFT gibt es noch weitere messbare Veränderungen in den Vibrationsdaten.

### Root Mean Square

### Peak to Peak

### Crest Factor

### Kurtosis

# Labeling

# Feature Verteilung nach Label

# Feature Korrelation

