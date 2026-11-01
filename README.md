# AGRARPOLY – V2.10

## Änderung in V2.10
- Ereigniskarten-Popup bleibt bei jedem Spieler sichtbar, bis dieser Spieler selbst auf **KARTE SCHLIESSEN** klickt.
- Das Schließen ist lokal: Andere Spieler sehen ihr Popup weiterhin, bis sie es ebenfalls schließen.
- Das Popup erscheint nicht erneut bei jedem weiteren Server-State derselben Karte.
- Beim nächsten gezogenen Ereignis wird automatisch ein neues Popup geöffnet.
- Spielablauf, Kartenraster und Master-Steuerung bleiben unverändert.

## Render
1. Repository mit den Projektdateien verbinden.
2. Root Directory leer lassen, wenn `server.js`, `package.json` und `public/` im Repository-Hauptverzeichnis liegen.
3. Build Command: `npm install`
4. Start Command: `npm start`

## Lokal
```bash
npm install
npm start
```

Danach ist die Anwendung über den vom Server verwendeten Port erreichbar.

## Wichtig
- Nur diese `README.md` gehört zur ZIP.
- Der Spielcode wird vom Master erzeugt.
- Spieler öffnen den Spieler-Link mit dem enthaltenen Spielcode.
- Das OBS-Overlay verwendet den Overlay-Link mit dem Spielcode.
