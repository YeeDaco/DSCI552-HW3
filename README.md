# DSCI 552 — Homework 3

Time-domain feature extraction on the UCI AReM (Activity Recognition system based on Multisensor data fusion) dataset, plus ISLR exercise 3.7.4.

## Structure

```
.
├── README.md
├── .gitignore
├── data
│   ├── AReM
│   │   ├── bending1/ bending2/ cycling/ lying/ sitting/ standing/ walking/   (dataset*.csv)
│   │   ├── bendingType.pdf
│   │   └── sensorsPlacement.pdf
│   └── arem_time_domain_features.csv   (written by the notebook; 88 instances x 42 features)
├── notebook
│   └── Lu_Yiming_HW3.ipynb
└── requirements.txt
```

## Run

```bash
pip install -r requirements.txt
cd notebook
jupyter notebook Lu_Yiming_HW3.ipynb   # then Kernel -> Restart & Run All
```

The notebook loads data with the relative path `../data/AReM/`. A few raw files have small format problems (space-separated values, trailing commas, one series with 479 rows); the notebook's parser handles them without changing the files.
