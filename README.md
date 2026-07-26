# Integrated-Global-Development-Research-Database
Integrated Global Development Research Database (IGDRD): An open, reproducible platform integrating global economic, social, human capital, environmental, and governance data into harmonized panel datasets for development research, econometrics, and evidence-based policymaking.
Integrated_Global_Development_Research_Database/
│
├── README.md
├── LICENSE
├── requirements.txt
├── environment.yml
├── .gitignore
│
├── data/
│   ├── raw/
│   │   ├── world_bank/
│   │   ├── wgi/
│   │   ├── undp/
│   │   ├── ilo/
│   │   └── other_sources/
│   │
│   ├── interim/
│   │
│   ├── processed/
│   │   ├── IGDRD_economic_clean.csv
│   │   ├── IGDRD_social_inclusion_clean.csv
│   │   ├── IGDRD_human_capital_clean.csv
│   │   ├── IGDRD_resource_sustainability_clean.csv
│   │   └── IGDRD_master_panel.csv
│   │
│   └── metadata/
│       ├── indicator_dictionary.csv
│       ├── country_dictionary.csv
│       └── data_sources.csv
│
├── notebooks/
│   ├── 01_Data_Acquisition.ipynb
│   ├── 02_Data_Cleaning.ipynb
│   ├── 03_Master_Panel.ipynb
│   ├── 04_Exploratory_Analysis.ipynb
│   ├── 05_Index_Construction.ipynb
│   └── 06_Econometric_Models.ipynb
│
├── src/
│   ├── acquisition/
│   │   ├── worldbank_api.py
│   │   ├── governance_api.py
│   │   ├── undp_api.py
│   │   └── utils.py
│   │
│   ├── cleaning/
│   │   ├── economic_clean.py
│   │   ├── social_clean.py
│   │   ├── human_capital_clean.py
│   │   ├── resource_clean.py
│   │   └── validation.py
│   │
│   ├── integration/
│   │   ├── merge_modules.py
│   │   ├── harmonise_panel.py
│   │   └── construct_master_panel.py
│   │
│   ├── indices/
│   │   ├── pca_indices.py
│   │   ├── capdev.py
│   │   ├── hcdi.py
│   │   └── iegi.py
│   │
│   ├── econometrics/
│   │   ├── descriptive.py
│   │   ├── panel_models.py
│   │   ├── system_gmm.py
│   │   ├── diagnostics.py
│   │   └── robustness.py
│   │
│   └── visualisation/
│       ├── maps.py
│       ├── trends.py
│       ├── dashboards.py
│       └── figures.py
│
├── outputs/
│   ├── tables/
│   ├── figures/
│   ├── reports/
│   └── logs/
│
├── docs/
│   ├── methodology.md
│   ├── data_dictionary.md
│   ├── indicator_catalogue.md
│   ├── api_reference.md
│   └── user_guide.md
│
└── tests/
    ├── test_api.py
    ├── test_cleaning.py
    ├── test_merging.py
    └── test_indices.py
