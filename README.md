# bachelorarbeit-3d-scan-pipeline

Quellcode zur Bachelorarbeit von Ben Nicolaus
Technische Hochschule Würzburg-Schweinfurt, 2026

## Voraussetzungen

Python 3.12 sowie folgende Bibliotheken:

pip install pyrealsense2 numpy opencv-python open3d scipy scikit-learn

## Programme und Ausführungsreihenfolge

1. drehachse_messen.py
   Kalibrierung der Drehachse — roten Referenzpunkt auf Tellermitte 
   positionieren, Programm starten, 's' drücken zum Speichern.
   Ausgabe: drehachse.json

2. scan_drehteller.py  
   Aufnahme der vier Scans — Objekt nach jedem Scan um 90° drehen,
   's' drücken zum Speichern, 'q' zum Beenden.
   Ausgabe: session_DATUM_UHRZEIT/

3. zusammenfuegen.py
   Session-Ordnernamen in Zeile 6 anpassen, dann starten.
   Ausgabe: linie_komplett.ply und linie_komplett.csv

4. pfad_generierung.py
   Dateipfad in Zeile 5 anpassen, dann starten.
   Ausgabe: roboterpfad.csv

## Hardware

Intel RealSense D435i, angeschlossen via USB 3.0
