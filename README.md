# 🎂 Bday – Geburtstags-App

Eine dunkle, schnelle Android-App, damit du nie wieder einen Geburtstag vergisst.
Gebaut mit Kotlin, Jetpack Compose (Material 3) und Glance-Widgets.

## Features

**Kalender**
- Monatsansicht mit Wischen zwischen den Monaten, alle Tage auf einen Blick
- Tage mit Geburtstag sind markiert (farbige Punkte pro Person), heute ist umrandet
- Tag antippen → Geburtstage an dem Tag sehen, **lange drücken → direkt eintragen**
- Jahresübersicht mit allen 12 Monaten als Mini-Kalender

**Start**
- Große Karte für den nächsten Geburtstag mit Countdown
- Spezielle „Heute“-Karte mit „Gratulieren“- und „Anrufen“-Knopf
- Gruppiert nach „Nächste 7 Tage“, „Nächste 30 Tage“ und „Später“
- Suche (Name, Monat, Notiz) und Filter (Favoriten, Familie, Freunde, Arbeit, …)

**Personen**
- Name, Tag, Monat, optional Geburtsjahr (→ Alter, „wird 30“, runde Geburtstage 🏆)
- Gruppe, Farbe, Telefonnummer, Notiz, Favorit, Erinnerung an/aus
- Geschenkideen-Liste zum Abhaken
- Sternzeichen, aktuelles Alter, Lebenstage
- Gratulieren per Teilen-Menü (WhatsApp, Telegram, …), Anrufen oder SMS
- Löschen mit „Rückgängig“
- 29. Februar wird in Nicht-Schaltjahren am 28. gefeiert

**Benachrichtigungen**
- Am Geburtstag zur eingestellten Uhrzeit
- Vorab-Erinnerungen (1, 2, 3, 7, 14 oder 30 Tage vorher – beliebig kombinierbar)
- Direkt aus der Benachrichtigung gratulieren oder anrufen
- Funktioniert auch nach Neustart; verpasste Erinnerungen werden nachgeholt

**Widgets**
- „Nächste Geburtstage“: Countdown + Liste, skaliert mit der Größe, „+“ zum schnellen Hinzufügen
- „Geburtstags-Kalender“: aktueller Monat mit markierten Tagen

**Statistik**
- Geburtstage pro Monat, Gruppen, Wochentage, Sternzeichen
- Runde Geburtstage der nächsten 12 Monate, älteste/jüngste Person

**Einstellungen**
- Erinnerungen an/aus, Uhrzeit, Vorab-Tage, Test-Benachrichtigung
- 8 Akzentfarben, AMOLED-Schwarz, Wochenstart Mo/So, Alter & Sternzeichen ein/aus
- Eigene Glückwunsch-Vorlage mit Platzhaltern `{name}`, `{vollname}`, `{alter}`
- Import aus Kontakten, Backup exportieren/importieren (JSON), alles löschen
- Widgets direkt aus der App zum Startbildschirm hinzufügen

## Installieren

Jeder Push baut die App automatisch über GitHub Actions:

1. Im Repo auf **Actions** → neuester Lauf von **Android Build** gehen
2. Unten bei **Artifacts** `bday-apk` herunterladen und entpacken
3. `app-release.apk` aufs Handy kopieren und installieren
   (ggf. „Installation aus unbekannten Quellen“ erlauben)

Oder selbst bauen: Projekt in Android Studio öffnen und auf ▶ drücken, bzw.

```bash
./gradlew assembleRelease
```

Mindestens Android 8.0 (API 26).
