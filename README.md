# IoT-ML
 
This project processes IoT sensor data and uses this data to train and test different models to detect malicious network traffic across these
sensors.
 
---
 
## Project Structure
 
```
my_ml_project/
│
├── README.md                     # Project documentation
├── requirements.txt              # Python dependencies
├── .gitignore
│
├── data/
│   ├── download_data.sh          # Fetches raw data from source
│   └── preprocess.py             # Cleans and prepares data for training
│
├── src/
│   ├── __init__.py
│   ├── models/                   # Model architecture definitions
│   ├── data/                     # Dataset classes and data loaders
│   ├── utils/                    # Shared helper functions
│   └── train.py                  # Main training entry point
│
├── scripts/
│   ├── train_baseline.sh         # SLURM job for baseline training run
│   └── hyperparameter_search.sh  # SLURM job for hyperparameter sweep
│
├── configs/
│   ├── default.yaml              # Default hyperparameters and settings
│   └── experiment1.yaml          # Overrides for a specific experiment
│
├── notebooks/                    # Exploratory analysis and prototyping
├── tests/                        # Unit and integration tests
├── logs/                         # Training logs (gitignored)
├── checkpoints/                  # Saved model weights (gitignored)
└── results/                      # Evaluation outputs and metrics (gitignored)
```
 
