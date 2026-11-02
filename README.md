# AGRARPOLY V2.20

## Basis
Diese Version baut ausschließlich auf dem stabilen Stand **V2.16** auf.

## Neue Funktionen
- 💾 **3 SPEICHERSLOTS**: Jeder Spielcode hat drei getrennte Speicherplätze.
- 📂 **SPEICHERSTAND LADEN**: Speicherplatz 1, 2 oder 3 kann geladen werden.
- 🗑️ **SPEICHERSTAND LÖSCHEN**: Ein einzelner Speicherplatz kann vollständig gelöscht werden.
- 💾 **SPIEL SPEICHERN**: Der aktuelle Spielstand wird serverseitig als JSON unter `saves/<SPIELCODE>_slot1.json`, `_slot2.json` oder `_slot3.json` gespeichert.
- 📂 **SPIEL LADEN**: Ein gespeicherter Spielstand kann innerhalb eines laufenden Spiels geladen werden.
- 📂 **GESPEICHERTEN SPIELSTAND LADEN**: Auf der Startseite kann ein gespeicherter Spielstand über seinen Spielcode wieder als Master geöffnet werden.
- ♾️ **ENDLOSSPIEL**: Nach dem letzten Spieler beginnt der nächste Durchlauf automatisch. Die Rundenzahl wird erhöht.
- 🛑 **SPIEL BEENDEN**: Nur der Master kann das laufende Spiel beenden. Der Spielstand wird dabei automatisch gespeichert.

## Speicherplätze
- **Speicherplatz 1**
- **Speicherplatz 2**
- **Speicherplatz 3**
- Alte V2.19-Spielstände ohne Slot-Kennung werden beim Laden als Speicherplatz 1 erkannt.

## Wichtig
Die bestehende Würfel-, Ereigniskarten-, Popup- und Spielerlogik von V2.16 wurde nicht neu gestaltet.

Die Speicherung verwendet das Dateisystem des Node.js-Servers. Auf Hosting-Plattformen mit flüchtigem Dateisystem, z. B. bei einem neuen Render-Deployment, kann eine lokale Speicherdatei verloren gehen. Für dauerhaftes Speichern über Deployments hinweg wäre später eine externe Datenbank oder ein persistenter Speicher sinnvoll.

## Render
1. Dateien ins GitHub-Repository übernehmen.
2. Render Web Service verwenden.
3. Root Directory leer lassen, wenn `server.js` und `package.json` im Repository-Hauptverzeichnis liegen.
4. Build Command: `npm install`
5. Start Command: `npm start`

## Start lokal
```bash
npm install
npm start
```
Dann im Browser den lokalen Server öffnen.
