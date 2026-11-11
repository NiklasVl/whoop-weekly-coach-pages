# whoop-weekly-coach-pages

Zwei statische, unkritische HTML-Dateien für das private Projekt
[`whoop-weekly-coach`](https://github.com/NiklasVl/whoop-weekly-coach) (siehe
dort `CLAUDE.md`) — **kein Code, keine Secrets, keine Gesundheitsdaten**.

Dieses Repo ist nur öffentlich, weil GitHub Pages auf dem kostenlosen Plan
kein privates Repo hosten kann; der eigentliche Projekt-Code bleibt privat.

- `oauth-callback.html` — als Redirect-URL bei Whoop registriert (Whoop
  verlangt zwingend `https://`, ein lokaler Server allein reicht nicht).
  Leitet den Autorisierungscode per Top-Level-Navigation an
  `http://localhost:8000/oauth/callback` weiter, mit Fallback-Anzeige des
  Codes falls das lokale Backend nicht erreichbar ist.
- `privacy.html` — Pflichtfeld im Whoop-Developer-App-Formular.

Nach einem Push hier: GitHub Pages ggf. unter *Settings → Pages* aktivieren
(Branch `main`, Ordner `/`), damit die URLs live sind:
- `https://niklasvl.github.io/whoop-weekly-coach-pages/oauth-callback.html`
- `https://niklasvl.github.io/whoop-weekly-coach-pages/privacy.html`
