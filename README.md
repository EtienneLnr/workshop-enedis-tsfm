# Workshop Enedis TSFM

```
workshop_enedis_tsfm/
├── checkpoints/          # checkpoints des modèles (non présents sur le git)
├── data/
│   ├── eol_hdf_2021.pt
│   └── vic_electricity.csv
├── notebooks/
│   ├── get_started_forecasting.ipynb
│   └── get_started_imputation.ipynb
├── pyproject.toml
├── requirements.txt
└── uv.lock
```

## Installation

### 1. Cloner le dépôt

```bash
git clone https://github.com/EtienneLnr/workshop-enedis-tsfm.git
cd workshop-enedis-tsfm
```

### 2. Ajouter les checkpoints

Remplacer le dossier `checkpoints/` du dépôt par le dossier `checkpoints/` qui vous a été envoyé (contenu de `checkpoints.zip`). Il doit contenir :

```
checkpoints/
├── TS-ICL/
├── TiRex-2/
└── chronos-2/
```

### 3. Installer les dépendances (Python 3.12)

Avec [uv](https://docs.astral.sh/uv/) :

```bash
uv sync
```

Ou avec pip :

```bash
python3.12 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```
