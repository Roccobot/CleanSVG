# Removed.md: le cose tolte da CleanSVG, e come si recuperano

> **Cos'è questo file.** L'archivio di quello che è uscito dalla pagina: per ogni cosa tolta, che
> cosa faceva, quando è stata tolta, e da quale commit si recupera. Si legge su richiesta, quando
> qualcuno vuole riportare indietro un elemento o capire dove viveva.
> ⚠️ **Nei file di regole resta solo la decisione** (che la cosa non c'è più, e perché): ogni
> appunto su come recuperarla vive qui, corto o lungo che sia (regola universale in
> `rules/Roccobot.md` di `Roccobot/tools`, § '🗄️ Le cose tolte vivono in Removed.md').
> Le voci vanno dalla più recente alla più vecchia.

## 📝 Il footer della pagina

- **Che cosa faceva**: una nota in fondo alla pagina, sotto le carte: *La pulizia è effettuata in
  locale: i file non lasciano mai il dispositivo di origine.*, seguita da una frase su SVGO e
  sulle rifiniture della pagina. Le note di allora lo descrivevano **poco visibile** (opacità
  0,6, per richiesta dell'utente) e **allineato al contenuto delle carte**, cioè rientrato quanto
  il bordo più il padding di una carta, per cadere sotto la riga della luminanza.
- **Tolto nella `1.40`** (istruzione dell'utente, 2026-08-26): la sua prima frase chiude adesso
  la riga del motore.
- **Si recupera dal commit `9cb35b4^`**, cioè il genitore del commit di `main` della `1.40` (il
  repo non ha tag). Dove viveva:
  - in `index.html`, l'elemento `<footer>` in fondo al guscio e le regole CSS `footer` e
    `footer a`, coi due commenti sul rientro e sulla visibilità ridotta;
  - le note che lo descrivevano, nel `CLAUDE.md` del progetto di allora (oggi `Rules.md`).
- Il comando che mostra la pagina di allora: `git show 9cb35b4^:index.html`.
