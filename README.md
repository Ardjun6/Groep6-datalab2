# FC Barcelona Data-analyse - Datalab Groep 6

## Over het project

Dit project is gemaakt voor **Datalab** door **Groep 6**.  
In dit project analyseren we data over **FC Barcelona** met behulp van **Python**, **SQL** en **.ipynb - vscode**.

De analyse maakt gebruik van een SQLite-database met voetbaldata. We onderzoeken onder andere wedstrijden, competities, teamstatistieken, ranglijsten en spelergegevens. Het doel is om meer inzicht te krijgen in de prestaties van FC Barcelona en andere teams binnen de dataset.

## Inhoud van de analyse

In de notebook worden onder andere de volgende onderdelen behandeld:

- Verbinding maken met de SQLite-database
- Het vinden van de `team_api_id` van FC Barcelona
- Wedstrijden van FC Barcelona ophalen uit de database
- De competitie van FC Barcelona bepalen
- Relaties tussen tabellen uitleggen
- Ranglijsten maken op basis van punten
- Wedstrijden per seizoen analyseren
- Punten per team per seizoen berekenen
- Visualisaties maken van teamstatistieken
- Spelergegevens voorbereiden en analyseren

## Gebruikte technieken

Voor dit project zijn de volgende technieken en libraries gebruikt:

- **Python**
- **Jupyter Notebook**
- **SQLite**
- **pandas**
- **matplotlib**
- **seaborn**

## Projectstructuur

```text
Groep6-datalab-sprint_2/
│
├── assets/
│   └── database.sqlite              # SQLite-database met voetbaldata
│
├── fc_barcelona_analysis.ipynb      # Notebook met de volledige analyse
│
└── README.md                        # Documentatie van het project
```

## Installatie

Clone eerst de repository:

```bash
git clone https://github.com/Ardjun6/Groep6-datalab-sprint_2.git
cd Groep6-datalab-sprint_2
```

Installeer daarna de benodigde Python-libraries:

```bash
pip install pandas matplotlib seaborn notebook
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

## Contributors

- **Ardjun Debi - Tewarie** — 25032895
- **Azfar Mohab Ali** — 25026356
- **Tesja Kartomo** — 25035193
- **Shelby Gibbs** — 18005055

## Licentie

Dit project valt onder de **MIT License**.

## Opmerking

Dit project is gemaakt voor **educatieve doeleinden** als onderdeel van een **Datalab opdracht**.

