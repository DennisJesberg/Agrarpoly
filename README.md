# AGRARPOLY V2.30 – Master-Würfel korrigiert

## Änderungen
- Würfelanzeige und Würfel-Button direkt in der Master-Ansicht ergänzt.
- Master kann selbst würfeln, wenn er beim Spielstart „Ja, ich spiele mit“ gewählt hat und an der Reihe ist.
- Würfelergebnis und Status werden in der Master-Ansicht angezeigt.
- Bei „Master spielt nicht mit“ bleibt der eigene Würfel-Button ausgeblendet; der Master gibt weiterhin die Würfel für Spieler frei.
- Neuer Header aus V2.28 bleibt erhalten.
- Bestehende Spiellogik, Ereigniskarten, Speicherplätze und Overlay bleiben erhalten.

## Render
ZIP entpacken und den vollständigen Inhalt in das GitHub-Repository übernehmen. Anschließend Render neu deployen. Das Projektverzeichnis enthält `server.js`, `package.json` und `public/`.


V2.30 Fehlerkorrektur: JavaScript-Syntaxfehler in der Master-Würfelstatusanzeige behoben. Dadurch werden die Client-Skripte wieder vollständig ausgeführt; insbesondere funktioniert die Spiel-Erstellung wieder.
