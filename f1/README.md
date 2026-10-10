# Formula 1

I'm a big F1 fan, so I use the sport's telemetry to practise data science. Both notebooks use 2026 data loaded with [FastF1](https://github.com/theOehrly/Fast-F1).

| Notebook | What it does |
|---|---|
| [Qualifying: driver strengths by corner type](qualifying_corner_analysis.ipynb) | Splits every qualifying lap into 25 mini-sectors, classifies them as straights or fast, medium or slow corners, and rates each driver on each type. The ratings, combined with a circuit's mix of corners, predict qualifying pace on tracks the drivers haven't raced on yet. |
| [Race pace & tyre strategy simulator](race_strategy_simulator.ipynb) | Learns how lap time changes with tyre age and compound (XGBoost, fuel-corrected laps), then simulates one-stop strategies lap by lap to find the best pit lap. |

To run them: `pip install fastf1 xgboost scikit-learn seaborn`, then *Run All*. FastF1 downloads the data from the official F1 timing servers, which currently block requests from cloud notebooks like Colab, so run them on your own machine.

Each notebook ends with a short list of its limitations.
