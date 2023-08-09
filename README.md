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
