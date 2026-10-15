# AES Büroservice, Website

Einseitige Website für AES Büroservice. Alles steckt in einer Datei (`index.html`): Schrift, Bilder und Stile sind eingebettet, es werden keine externen Dienste geladen.

## Dateien

* `index.html`: die komplette Website
* `design/ui-kit-final.json`: das UI-Kit (Farben, Schrift, Abstände, Buttons, Animationen)
* `.nojekyll`: sorgt dafür, dass GitHub Pages die Datei unverändert ausliefert

## Lokal ansehen

`index.html` im Browser öffnen. Das Kontaktformular sendet nur auf Netlify.

## Veröffentlichen

**Variante 1, Netlify mit GitHub verbinden (empfohlen):**

* Repository bei Netlify als Projekt aus Git importieren. Jede Änderung auf GitHub wird dann automatisch veröffentlicht.
* Das Kontaktformular läuft über Netlify Forms. Die E-Mail-Benachrichtigung wird in Netlify eingerichtet (Project configuration, Notifications, Form submission notifications).
* Die Datenschutzerklärung nennt Netlify als Hoster. Das passt zu dieser Variante.

**Variante 2, GitHub Pages:**

* Repository auf GitHub, dann Settings, Pages, Source: Deploy from a branch, Branch: main, Ordner: / (root).
* GitHub Pages liefert nur statische Dateien aus. Netlify Forms funktioniert dort nicht, das Formular bräuchte einen anderen Dienst.
* Die Datenschutzerklärung müsste auf den neuen Hoster angepasst werden.
* Eine eigene Domain wird in Settings, Pages eingetragen. Dazu kommt eine Datei `CNAME` im Hauptordner und eine DNS-Änderung beim Domain-Anbieter.

## Vor dem Livegang

* Alle Stellen mit `BITTE PRÜFEN` ersetzen (Impressum, Datenschutz, Umsatzsteuer-Hinweis).
* In `index.html` die Zeile `<meta name="robots" content="noindex">` entfernen. Sie verhindert bis dahin, dass Suchmaschinen die Seite aufnehmen.
* Impressum und Datenschutzerklärung von einer dafür zuständigen Stelle prüfen lassen.
