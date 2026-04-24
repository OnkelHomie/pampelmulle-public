# 🍋 Pampelmulle — Discord Bot

> Level-System, Economy, Games und Moderation — alles über ein modernes Web-Panel verwaltet.

[![Discord](https://img.shields.io/badge/Discord-GameZoneOne-5865F2?logo=discord&logoColor=white)](https://discord.gg/szBd7ZD5Bq)
[![Issues](https://img.shields.io/github/issues/OnkelHomie/pampelmulle-public)](https://github.com/OnkelHomie/pampelmulle-public/issues)
[![Changelog](https://img.shields.io/badge/Changelog-ansehen-brightgreen)](https://github.com/OnkelHomie/pampelmulle-public/blob/main/CHANGELOG.md)

---

## ✨ Features

| Modul | Beschreibung |
|---|---|
| **Level-System** | XP durch Chatten und Voice-Aktivität, automatische Level-Rollen |
| **Economy** | Coins, Staking (0,2%/Tag), Kredit, Shop mit Items und Boosts |
| **Lotterie** | Wöchentliche Lotterie, Community-Pott, Investitionen |
| **Spiele** | Blackjack, Slots, Crash, Plinko, High-Low, Münzwurf, Duell, Pampelmusenwurf |
| **AutoMod** | Schimpfwortfilter, Invite-Blocker, Mention-Spam, Caps-Filter u.v.m. |
| **Moderation** | Warn-System, Tempban/-mute, Warn-Schwellen, Audit-Logging |
| **Willkommen** | Individuelle Begrüßungs- und Abschiedsnachrichten |
| **Reaction Roles** | Rollen per Emoji-Reaktion oder Buttons vergeben |
| **Prestige** | Level-Reset für permanente Boni (+Coins, +XP, +Glück) |
| **Web-Panel** | Vollständiges Dashboard unter `community.gamezoneone.de` |

---

## 🤖 Commands

### Alle User

| Command | Beschreibung |
|---|---|
| `!profil [@User]` | Profil, Level, XP, Coins und Achievements anzeigen |
| `!daily` | Tägliche Coins abholen (Streak-Bonus) |
| `!prestige` | Level-Reset für permanente Boni |
| `!challenge` | Tägliche Herausforderung |
| `!pay @User <Betrag>` | Coins überweisen (5% Steuer) |
| `!kredit <Betrag>` | Kredit aufnehmen (max. Level × 500) |
| `!stake / !unstake` | Coins staken für tägliche Zinsen |
| `!shop` | Shop öffnen |
| `!lotterie / !lottokauf` | Lotterie-Infos und Tickets kaufen |
| `!blackjack / !slot / !crash` | Spiele mit Coin-Einsatz |
| `!plinko / !highlow / !münzwurf / !duell` | Weitere Spiele |
| `/bugreport` | Bug oder Feature-Wunsch direkt als GitHub Issue melden |

### Moderatoren *(Discord: Mitglieder moderieren)*

| Command | Beschreibung |
|---|---|
| `/warn @User <Grund>` | Verwarnung + automatische Aktionen bei Schwellen |
| `/mute / /unmute @User` | Discord-Timeout setzen / aufheben |
| `/tempmute @User <Min>` | Temporärer Mute (persistent) |
| `/infractions @User` | Verwarnungs-Verlauf anzeigen |

### Moderation *(höhere Discord-Rechte)*

| Command | Recht | Beschreibung |
|---|---|---|
| `/kick @User` | Kick Members | User kicken |
| `/ban / /unban @User` | Ban Members | User bannen / entbannen |
| `/tempban @User <Min>` | Ban Members | Temporärer Ban (persistent in DB) |
| `/clear <Anzahl>` | Manage Messages | Nachrichten löschen |

### Bot-Admin *(via `/botadmin` vergeben)*

| Command | Beschreibung |
|---|---|
| `/setchannel <feature> <kanal>` | Feature-Kanal setzen (levelup, lottery, …) |
| `/setgamechannel <spiel> <kanal>` | Spiel auf einen Kanal beschränken |
| `/setwarnthreshold <count> <action>` | Automatische Aktion bei X Verwarnungen |
| `/setlevelrole <level> <rolle>` | Rolle ab einem Level automatisch vergeben |
| `/botadmin add/remove/list` | Bot-Admins verwalten |
| `/resetserver` | ⚠️ Alle Server-Daten zurücksetzen |

---

## 🐛 Bug melden

Du hast einen Fehler gefunden? Melde ihn direkt im Discord:

```
/bugreport kategorie:Bug titel:"..." beschreibung:"..."
```

Der Bot formatiert deinen Report automatisch und erstellt ein GitHub Issue — du bekommst sofort den Link.

Alternativ kannst du Issues direkt hier auf GitHub erstellen: [→ Neues Issue](https://github.com/OnkelHomie/pampelmulle-public/issues/new/choose)

---

## ⚙️ Web-Panel

Das Dashboard ist unter **[community.gamezoneone.de](https://community.gamezoneone.de)** erreichbar.

**Features:**
- Spielerverwaltung (Coins anpassen, verwarnen, kicken, bannen, Rollen vergeben)
- Leaderboard mit Discord-Avataren
- Lotterie- und Community-Pott-Übersicht
- AutoMod konfigurieren (Regeln, Schimpfwörter, Warn-Schwellen)
- Willkommen-System konfigurieren
- Reaction Roles verwalten
- Mod-Log einsehen
- Live-Console (Owner)
- Ankündigungen senden (Owner)

---

## 🔗 Links

- **Discord:** [discord.gg/szBd7ZD5Bq](https://discord.gg/szBd7ZD5Bq)
- **Dashboard:** [community.gamezoneone.de](https://community.gamezoneone.de)
- **Bug-Reports:** [GitHub Issues](https://github.com/OnkelHomie/pampelmulle-public/issues)

---

## 📋 Bug-Report Vorlage

Wenn du ein Issue direkt auf GitHub erstellen möchtest:

**Für Bugs:**
- Was hast du gemacht?
- Was hast du erwartet?
- Was ist stattdessen passiert?
- Welchen Command hast du genutzt?

**Für Feature-Wünsche:**
- Was soll der Bot können?
- Warum wäre das nützlich?

---

*Pampelmulle ist ein privater Discord-Bot von [GameZoneOne](https://discord.gg/szBd7ZD5Bq).*
