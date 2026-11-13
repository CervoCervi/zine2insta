# Zine A7 → carosello Instagram

Web app che prende il PDF A4 di una zine pieghevole da 8 pagine A7 e genera un JPEG 4:5 per ogni pagina, pronto per un carosello Instagram.

**Usala qui:** https://cervocervi.github.io/zine2insta/

## Cosa fa

- Divide il foglio A4 orizzontale in 8 pagine A7 (griglia 4×2); se il foglio è verticale lo ruota.
- Ordine fisso: si parte dalla copertina (riga in basso, seconda da sinistra) e si procede in senso antiorario. La riga in alto viene raddrizzata.

  ```
  alto (capovolte):  7  6  5  4
  basso:             8  1  2  3
  ```

- Rimuove le linee di taglio e i crocini lungo i bordi di ogni pagina (lascia intatti i lati con immagini al vivo). C'è anche un "rifilo extra" in mm.
- Centra ogni pagina, mantenendo le proporzioni, su un fondo 4:5 (1080×1350, 1440×1800 o 2160×2700) con cornice bianca o del colore che scegli.
- Scarica le singole immagini o tutte insieme in uno ZIP (`nome_01.jpg` … `nome_08.jpg`).
- Accetta anche PDF con le 8 pagine già separate.

Tutto avviene nel browser: il PDF non viene caricato da nessuna parte.

## Uso in locale

Apri `index.html` in un browser moderno (serve la connessione per caricare pdf.js e JSZip da cdnjs).
