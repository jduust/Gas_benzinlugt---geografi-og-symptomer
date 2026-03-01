# 🏭 Benzinlugt Amager – Helbredsanalyse

Statistisk analyse af helbredspåvirkninger fra benzin/olie-lugt i Amager-området, baseret på spørgeskemadata indsamlet fra beboere i de berørte områder.

Appen er bygget i Python/Streamlit og hostet gratis via [Streamlit Community Cloud](https://gasbenzinlugt---geografi-og-symptomer-gjdx894vypyyqqdt2fawy8.streamlit.app/).

---

## 📊 Hvad appen viser

- **Dosis-respons-analyse** – symptomrate fordelt på eksponeringsgrad (ingen lugt → åbne vinduer → lukkede vinduer)
- **Relativ Risiko med 95% konfidensinterval** – hvor meget højere er risikoen for symptomer ved høj eksponering?
- **Symptomfordeling** – hvilke symptomer rapporteres, og hvor hyppigt?
- **Confounding-analyse** – resultater kontrolleret for præ-eksisterende luftvejssygdomme
- **Chi²-signifikanstest** – statistisk test med fuld gennemsigtighed

---

## 📁 Filer i dette repo

| Fil | Beskrivelse |
|-----|-------------|
| `app.py` | Streamlit-applikation |
| `benzinlugt - geografi og symptomer.csv` | Rå spørgeskemadata |
| `requirements.txt` | Python-afhængigheder |

---

## 🚀 Deploy på Streamlit Community Cloud (gratis)

1. **Fork eller upload** dette repo til din GitHub-konto
2. Gå til [share.streamlit.io](https://share.streamlit.io) og log ind med GitHub
3. Klik **"New app"** og vælg:
   - **Repository:** dit repo
   - **Branch:** `main`
   - **Main file path:** `app.py`
4. Klik **"Deploy"** — appen er live inden for ~1 minut

---

## 💻 Kør lokalt

```bash
pip install -r requirements.txt
streamlit run app.py
```

---

## ⚠️ Metodologisk note

Data er indsamlet via et selvvalgt spørgeskema, hvilket betyder at respondenter med stærke symptomer sandsynligvis er overrepræsenterede. Prævalenstal bør derfor ikke bruges som absolutte populationsestimater. Dosis-respons-mønstret og de statistiske tests er dog robuste overfor denne form for bias.

Analysen er udarbejdet med henblik på at informere myndigheder om behovet for en professionel epidemiologisk undersøgelse.

---

## 📦 Afhængigheder

```
streamlit
pandas
numpy
plotly
scipy
```

---

*Data indsamlet februar–marts 2026. Analysen må gerne deles og refereres til frit.*
