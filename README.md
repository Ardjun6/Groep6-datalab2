# FC Barcelona Data-analyse - Datalab Groep 6

## Over het project

Dit project is gemaakt voor **Datalab** door **Groep 6**.  
In dit project analyseren we voetbaldata over **FC Barcelona** met behulp van **Python**, **SQL** en een **Jupyter Notebook**.

De analyse maakt gebruik van een **SQLite-database** met voetbaldata. We onderzoeken wedstrijden, competities, teamstatistieken, ranglijsten, spelergegevens en voorspellende modellen. Het doel van het project is om meer inzicht te krijgen in de prestaties van FC Barcelona en om te onderzoeken of data gebruikt kan worden om wedstrijdresultaten beter te begrijpen en te voorspellen.

## Onderzoek en analyse

In de notebook worden onder andere de volgende onderdelen behandeld:

- Verbinding maken met de SQLite-database
- Het vinden van de `team_api_id` van FC Barcelona
- Wedstrijden van FC Barcelona ophalen uit de database
- De competitie van FC Barcelona bepalen
- Relaties tussen tabellen uitleggen
- Ranglijsten maken op basis van punten
- Wedstrijden per seizoen analyseren
- Punten per team per seizoen berekenen
- Teamstatistieken koppelen aan prestaties
- Visualisaties maken van teamstatistieken
- Spelergegevens voorbereiden en analyseren
- Gemiddelde spelerattributen berekenen
- Features selecteren voor een voorspelmodel
- Data schalen met `StandardScaler`
- Modellen trainen met Logistic Regression en Random Forest
- Hyperparameters testen met GridSearchCV
- Modelprestaties vergelijken
- Bookmakerkansen van Bet365 omrekenen naar voorspellingen
- Het model vergelijken met bookmakerverwachtingen

## Belangrijke gegevens

| Onderdeel | Waarde |
|---|---|
| Team | FC Barcelona |
| `team_api_id` | `8634` |
| Competitie | Spain LIGA BBVA |
| `league_id` / `country_id` | `21518` |
| Seizoen voor ranglijstvoorbeeld | 2015/2016 |
| Bookmaker voor vergelijking | Bet365 |

## Gebruikte technieken

Voor dit project zijn de volgende technieken en libraries gebruikt:

- **Python**
- **Jupyter Notebook**
- **SQLite**
- **SQL**
- **pandas**
- **matplotlib**
- **seaborn**
- **scikit-learn**

## Machine learning

In Sprint 5 is een voorspellend model gemaakt om wedstrijdresultaten te voorspellen.  
Het doel is om te voorspellen of een wedstrijd eindigt in:

- winst
- verlies
- gelijkspel

Hiervoor zijn spelerseigenschappen en teameigenschappen gebruikt als features. De data is geschaald met `StandardScaler` en daarna zijn twee modellen getest:

1. **Logistic Regression**
2. **Random Forest**

Met behulp van `GridSearchCV` zijn verschillende instellingen getest om het beste model te bepalen.

## Resultaten

Uit de analyse blijkt dat **Logistic Regression** het beste model was binnen deze vergelijking.

| Model / voorspeller | Accuracy |
|---|---:|
| Logistic Regression | 51,6% |
| Random Forest | 50,7% |
| Bet365 bookmaker | 53,3% |

De bookmaker Bet365 presteerde in deze vergelijking iets beter dan het model. Het verschil was ongeveer **1,7 procentpunt**.  
Dit betekent dat het model redelijk dichtbij de bookmaker zit, maar nog niet beter presteert dan de marktverwachting.

## Projectstructuur

```text
Groep6-datalab-sprint_2/
|
|-- assets/
|   `-- database.sqlite              # SQLite-database met voetbaldata
|
|-- fc_barcelona_analysis.ipynb      # Notebook met de volledige analyse
|
`-- README.md                        # Documentatie van het project
```

## Installatie

Clone eerst de repository:

```bash
git clone https://github.com/Ardjun6/Groep6-datalab-sprint_2.git
cd Groep6-datalab-sprint_2
```

Installeer daarna de benodigde Python-libraries:

```bash
pip install pandas matplotlib seaborn scikit-learn notebook
```

> Let op: `sqlite3` hoeft normaal gesproken niet apart geïnstalleerd te worden, omdat deze standaard bij Python zit.

## Gebruik

Open de Jupyter Notebook met:

```bash
jupyter notebook fc_barcelona_analysis.ipynb
```

Zorg ervoor dat de database op de juiste plek staat:

```text
assets/database.sqlite
```

De notebook maakt standaard verbinding met dit pad:

```python
./assets/database.sqlite
```

Voer daarna de cellen in de notebook stap voor stap uit.

## Contributors

- **Ardjun Debi - Tewarie** - 25032895
- **Azfar Mohab Ali** - 25026356
- **Tesja Kartomo** - 25035193
- **Shelby Gibbs** - 18005055

## Licentie

Dit project valt onder de **MIT License**.

## Opmerking

Dit project is gemaakt voor **educatieve doeleinden** als onderdeel van een **Datalab-opdracht**.
