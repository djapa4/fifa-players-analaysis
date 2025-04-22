# 🏟️ Football Players Data Analysis

Ovaj projekat predstavlja analizu fudbalskih igrača korišćenjem Pandas i Matplotlib biblioteka u Pythonu. Korišćen je dataset sa [Kaggle](https://www.kaggle.com/datasets/maso0dahmed/football-players-data), koji sadrži podatke o profesionalnim igračima u FIFI — uključujući njihove fizičke karakteristike, tržišnu vrednost, pozicije, zemlje porekla i više.

## 📊 Korišćeni alati

- Python
- Jupyter Notebook
- Pandas
- Matplotlib

## 📁 Dataset

Dataset sadrži sledeće kolone (neke od najvažnijih):

- `name`, `full_name`
- `age`
- `height_cm`, `weight_kg`
- `nationality`, `national_team`, `national_rating`
- `positions`
- `value_euro`, `wage_euro`

## 🧹 Čišćenje podataka

- Popunjene `NaN` vrednosti u kolonama `wage_euro`, `value_euro` i 'release_clause_euro' sa prosečnim vrednostima.
- Popunjene 'NaN' vrednosti u kolonama 'national_rating' i 'national_jersey_number' sa vrednosti 0.
- Popunjene 'NaN' vrednosti u kolonama 'national_team' i 'national_team_position sa 'not-called'.
- Kreirane nove kolone kao npr. `is_top_player` (ako je value_euro > 40 miliona).
- Droppovana kolona koju sam slucajno napravio (nationa_team_position).

## 📈 Analize i vizualizacije

- Distribucija visine i težine – Histogrami
- Boxplot: Plata po godinama
- Scatter plot: Visina vs Težina po godinama
- Pie chart: Top 10 drzava po broju igraca
- Prosečna tržišna vrednost po godinama
- Top 10 drzava sa najskupljim igracima u proseku
- Top 10 plata po naciji
- Broj mladih igrača (< 22 god) po poziciji
- Broj igrača koji su viši od 185cm i vrede više od 20M
- Top 5 najskupljih igrača po zadatoj zemlji (funkcija)
