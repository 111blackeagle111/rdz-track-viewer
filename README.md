# 🎈 rdz-track-viewer

Visualizzatore offline per tracce radiosonde meteo con analisi avanzata del volo, predizione touchdown e export KML.

[![HTML5](https://img.shields.io/badge/HTML5-ES6-orange.svg)](https://www.w3.org/TR/html5/)
[![Leaflet](https://img.shields.io/badge/Maps-Leaflet-green.svg)](https://leafletjs.com/)

![Screenshot interfaccia](screenshot.png)

## ✨ Caratteristiche

- **📍 Visualizzazione mappa interattiva** (Leaflet) con heatmap altimetrica
- **🎯 Predizione Touchdown** calcolata in tempo reale su base velocità e vario
- **💨 Rilevamento Wind Shear** - analizza automaticamente variazioni di velocità del vento tra strati atmosferici
- **🏠 Calcolo distanza QTH** - inserisci le tue coordinate e calcola distanza, tempo di arrivo e bearing
- **🌍 Export KML** per Google Earth con traccia 3D, punto di atterraggio stimato e marker QTH
- **📊 Grafici avanzati** (Chart.js) con profilo altimetrico e dinamica di volo (velocità vs vario)
- **🔓 100% Offline** - Funziona in locale senza server, dati salvati in memoria

## 🚀 Utilizzo

1. Scarica il file `index.html`
2. Apri con qualsiasi browser moderno (Chrome, Firefox, Edge)
3. Carica il tuo file `.csv` contenente i dati della radiosonda
4. Inserisci le coordinate del tuo QTH (opzionale)
5. Esplora la traccia e scarica il KML per Google Earth

Nessuna installazione richiesta. Funziona su Windows, macOS, Linux e persino Raspberry Pi.

## 📋 Formato Dati Supportato

Il file CSV deve contenere colonne separate da virgola nel formato:

```csv
tipo,id,flag,lat,lon,alt,vario,speed,dir,sats,rssi,timestamp,frame
1,X1812309,0,41.528618,13.303823,18487.494,-16.343,19.330,80.112,9,127,1770987159,8163
