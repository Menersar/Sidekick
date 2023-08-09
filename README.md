# Sidekick

<h2 id="embedding">Einbettung</h2>

Einbettung über das iframe-HTML-Element:

```HTML
<iframe src="https://scratch.mit.edu/projects/[ID]/embed" width="499" height="416" allowtransparency="true" frameborder="0" scrolling="no" allowfullscreen></iframe>
```

- `[ID]` bestimmt die ID des einzubettenden Projektes (ersetzen).
- `width` und `height` bestimmen die Dimensionen des iframe-HTML-Elememts.
  - Die Größe des Players wird dabei automatisch angepasst.
  - Beispiel: Bei `width="499" height="416"` des iframe-Elements rendert die Bühne unverzerrt mit 480 x 360 Pixeln Größe.

<h2 id="unshared-projects">Nicht öffentlich geteilte Scratch-Projekte</h2>

Ungeteilte Scratch-Projekte sind nicht mehr öffentlich sicht- und einsehbar.

Um ein Projekts von der Scratch-API herunterzuladen, ist ein Projekt-Token erforderlich. Auf den Token hat, bei nicht freigegebenen Projekten, nur der Projekt-Eigentümer Zugriff. Sidekick kann deshalb ebenso nicht auf ungeteilte Scratch-Projekte zugreifen. Token werden zusätzlich regelmäßig und in kurzen Zeitabschnitten erneuert – vorherige Token werden damit unbrauchbar.
Scratch-Projekte werden wie folgt heruntergeladen:
- Den Projekt-Token über das project_token-Feld der URL https://api.scratch.mit.edu/projects/[ID] abgreifen.
- Mit der Information die URL https://projects.scratch.mit.edu/ID?token=[Projekt-Token] aufrufen.
