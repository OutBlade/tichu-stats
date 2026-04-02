# Tichu Statistik - Referenzseite für erfahrene Spieler

**Live Demo:** [https://outblade.github.io/tichu-stats/](https://outblade.github.io/tichu-stats/)

Eine interaktive Statistik-Referenzseite für Tichu-Spieler, basierend auf einem gefilterten Datensatz von ~400.000 Runden erfahrener BSW-Spieler (>100 Partien, ≥55% Winrate). Alle Daten stammen aus der Analyse von [fabianvdw.github.io](https://fabianvdw.github.io/).

**Keywords:** Tichu Strategie, Tichu Statistiken, Tichu BSW, Bomben Wahrscheinlichkeit, Großes Tichu, Schupfkarten, Tichu Referenz

## Features

- **5 Themen-Tabs**: Bomben, Großes Tichu, GT bei Rückstand, Schupfkarten, Straßen
- **Gefilterter Datensatz**: ~400K Runden vs. ~21M Gesamtrunden — beide Werte immer vergleichbar
- **Opportunitätskosten-Analyse**: Wann lohnt GT wirklich? Nicht nur Erfolgsrate, sondern Erwartungswert
- **Schupfstrategie-Vergleich**: Gerade/Ungerade vs. Klein/Groß vs. keine Strategie
- **Bomben-Korrelationen**: Drillinge, Tichu-Ansagen und Gegner-Bombenrisiko
- **Straßen-Risikotabellen**: Überbietungswahrscheinlichkeit nach Länge, 4er-Vervollständigung
- **Keine Dependencies**: Reines HTML/CSS/JS — sofort offline nutzbar

## Live Demo

**Jetzt öffnen:** [Tichu Statistik Referenz](https://outblade.github.io/tichu-stats/)

**Was du findest:**
- Bombenwahrscheinlichkeiten in jeder Spielsituation
- GT-Entscheidungsrahmen nach 80 Handklassen (Asse × Sonderkarten)
- Ab welchem Rückstand GT mit welcher Hand sinnvoll ist
- Hund und Mahjong: Erwartungswerte beim Schupfen
- Straßenlänge vs. Überbietungsrisiko

## Datenbasis

| Datensatz | Runden | Beschreibung |
|-----------|--------|-------------|
| `(*)` Alle Spiele | ~21.000.000 | Gesamter BSW-Datensatz |
| `(**)` Gefiltert | ~400.000 | Spieler mit >100 Partien & ≥55% Winrate |

Quelle: [fabianvdw.github.io](https://fabianvdw.github.io/) — 8-teilige Analyse-Reihe (Pt.0–Pt.4 + Changelog)

## Technologie

- **Frontend:** Vanilla HTML5, CSS3, JavaScript (ES6+)
- **Design:** Dark-Mode-Terminal-Ästhetik, Monospace-Typografie
- **Deployment:** GitHub Pages
- **Bundle:** Einzelne HTML-Datei, keine externen Abhängigkeiten

## Inhalt

### 💣 Bomben (Pt.1)
Wahrscheinlichkeiten nach Spielsituation, Drillinge-Korrelation, Bombenwert (Erwarteter Rundengewinn: 90.7 Pkt.), Schupfstrategie-Vergleich zur Bombenreduktion.

### 🎯 Großes Tichu (Pt.2)
Ansagerate & Erfolgsquoten nach 80 Handklassen. Opportunitätskosten-Modell: Warum 50% Erfolgsrate nicht ausreicht. Erfahrene Spieler sagen GT nur bei 3.57–7.69% aller Hände an.

### 📉 GT bei Rückstand (Pt.2.2)
Ab −305 Punkten lohnt GT mit jeder Hand. Schwellenwerte nach Handklasse: von ausgeglichenem Stand (beste Hände) bis Verzweiflungs-GT (schwache Hände).

### 🃏 Schupfkarten (Pt.4)
Hund an GT-Ansager schupfen: +40–53 Punkte Erwartungswert. Hund an Gegner: −25.65 Punkte. Ass-Korrelationen: Wenn Ass einzige Hochkarte → Partner schupft es in 59.9% der Fälle.

### 📏 Straßen (Pt.3)
5er-Straße wird in 36.4% der Fälle überboten. 3-4-5-6 → 59.3% Vervollständigung. J-Q-K-A → nur 12.7%.

## Lokale Nutzung

```bash
# Repository klonen
git clone https://github.com/OutBlade/tichu-stats.git
cd tichu-stats

# Direkt im Browser öffnen — keine Installation nötig
open index.html
```

## Referenzen

- Originale Analyse: [fabianvdw.github.io](https://fabianvdw.github.io/)
- Datensatz: BrettSpielWelt (BSW)
- Kontakt Analyst: [fabianvonderwarth@gmail.com](mailto:fabianvonderwarth@gmail.com)
