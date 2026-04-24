## 🔧 Update — 24.04.2026 (4)

### ⚙️ Set-Commands konsolidiert
Alle Konfigurations-Commands sind jetzt unter einem einzigen `/set` Befehl zusammengefasst:

| Vorher | Jetzt |
|---|---|
| `/setchannel` | `/set channel` |
| `/setgamechannel` | `/set gamechannel` |
| `/setwarnthreshold` | `/set warnthreshold` |
| `/setlevelrole` | `/set levelrole` |
| `/sethelp` | `/set channel help` |
| `/setleaderboard` | `/set channel leaderboard` |

### 🃏 Blackjack-Kanal konfigurierbar
`/set gamechannel spiel:Blackjack` setzt den Kanal für `!blackjack`.

---

## 🐛 GitHub Bug-Tracker — 24.04.2026 (3)

Bugs und Feature-Wünsche könnt ihr jetzt direkt melden — automatisch als GitHub Issue!

**3 Wege:**
- Im **Bug-Kanal** einfach hinschreiben — der Bot analysiert automatisch und erstellt ein Issue
- `/bugreport` Slash-Command mit Kategorie, Titel und Beschreibung
- `!bugreport <text>` Prefix-Command

Der Bot erkennt auch mehrere Bugs in einer Nachricht und erstellt separate Issues.
Mods können zusätzlich mit 🐛 auf jede Nachricht reagieren um daraus ein Issue zu machen.
Kein Bug erkannt? Der Bot antwortet mit einem Hinweis (👀-Reaktion).

---

## 🌐 Dashboard-Ausbau — 24.04.2026 (2)

Das Community-Dashboard wurde massiv erweitert:

- **Einstellungen:** Prefix, Sprache, Embed-Farbe, alle Feature- und Spiel-Kanäle konfigurierbar (inkl. Blackjack)
- **AutoMod:** Warn-Schwellen jetzt im Dashboard editierbar (hinzufügen & entfernen)
- **Spielerverwaltung:** Kick-Button neben Ban, Rollen-Vergabe direkt im Panel
- **Owner — Server-Liste:** Alle Server mit Mitgliederzahl und Tracking-Stats
- **Owner — Bot-Logs:** Paginiert, filterbar nach Typ, durchsuchbar
- **Owner — Ankündigungen:** Nachricht oder Embed an beliebigen Kanal senden
- **Owner — Bot-Config:** Anti-Spam, Immune-Rollen, Slash-Commands an/aus
- **Hilfe & Setup:** Interaktive Checkliste, 7-Schritte-Guide, vollständige Befehlsreferenz mit Permissions

---

## 🌐 Community Dashboard — 24.04.2026

Neues Web-Dashboard unter **[community.gamezoneone.de](https://community.gamezoneone.de)**

- Discord OAuth2 Login
- Server-Übersicht mit Modul-Toggles (Welcome, AutoMod)
- Spielerverwaltung (Suche, User-Detail, Coins anpassen, Verwarnen, Kicken, Bannen, Rollen)
- Leaderboard mit Discord-Avataren
- Mod-Log mit Usernamen statt IDs
- Lotterie- und Community-Pott-Übersicht
- Reaction Roles verwalten
- Willkommen-System konfigurieren
- Owner-Bereich: Economy, Live-Console, Ankündigungen

---

## 🎮 Neue Features — 24.04.2026

### 🃏 Blackjack
Neues Kartenspiel! `!blackjack <einsatz>` — Spiele gegen den Dealer.
Hit, Stand oder Double Down per Button. Blackjack zahlt 1,5x, Dealer zieht bis 17.

### 📊 Level-Rollen
User erhalten jetzt automatisch eine Discord-Rolle, wenn sie ein bestimmtes Level erreichen.
Admins konfigurieren das mit `/set levelrole set <level> <rolle>`.

### ⚠️ Automatische Warn-Schwellen
Nach X Verwarnungen greift der Bot automatisch ein (Mute/Kick/Ban).
Konfiguration per `/set warnthreshold set <anzahl> <aktion>`.

### 🔊 Voice-XP
User verdienen jetzt XP für Zeit in Voice-Channels (3 XP/Minute).
Level-Ups werden im konfigurierten Levelup-Channel angekündigt.

### 💸 5% Coin-Steuer bei `!pay`
Bei `!pay @user 1.000` werden dem Sender **1.050** abgezogen — 50 Coins werden vernichtet.
Verhindert Coin-Farming unter Freunden.

---

## 🔧 Update — 24.04.2026 (2)

### 🛠️ Staking-Datenmigration
Staking-Daten haben jetzt eine eigene Datenbank-Collection. Alle bestehenden Stakes wurden migriert.
Für euch ändert sich nichts — `!stake`, `!unstake`, `!mystake` laufen wie gewohnt.

---

## 🔧 Update — 24.04.2026

### ❌ Crypto-Trading entfernt
Das Kryptowährungs-System wurde entfernt.
**Staking bleibt:** `!stake`, `!unstake`, `!mystake` laufen weiter wie gewohnt.

### 🛡️ Temporäre Bans jetzt neustart-sicher
Temp-Bans (`/tempban`) werden in der Datenbank gespeichert und überleben Bot-Neustarts.

### 🔇 Temporäre Mutes auf Discord-Timeout umgestellt
`/tempmute` nutzt jetzt Discords eingebautes Timeout-System — kein Bot-Neustart beeinflusst sie mehr.
