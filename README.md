# Machine Learning Projects

This repository contains machine-learning projects completed in 2023. The featured project is a Genetic Tetris Agent located in `Project_5`.

## Featured Project: Genetic Tetris Agent

The Genetic Tetris Agent is an individual project built around a preexisting Pygame Tetris simulator. I designed and implemented a genetic-algorithm training pipeline that evolved nine-feature board-evaluation weights through survivor selection, crossover, and mutation.

Fitness evaluation was parallelized for populations of 1,000 agents across 30 worker processes. The trained agent sustained gameplay for approximately 10 minutes, compared with the original 60-second project target.

## Technologies

- Python
- NumPy
- Pygame
- Python multiprocessing

## Project Files

- `Project_5/Project_5.ipynb` — training and evaluation workflow
- `Project_5/libraries/AI/genetic.py` — genetic-agent implementation
- `Project_5/libraries/AI/genetic_helpers.py` — board-feature calculations
- `Project_5/libraries/game.py` — simulator and gameplay logic
- `Project_5/deployment.py` — trained-agent deployment script

## Running the Genetic Tetris Agent

Clone the repository and enter the project directory:

```bash
git clone https://github.com/ProfessorSen0/machineLearning.git
cd machineLearning/Project_5
pip install -r requirements.txt
python deployment.py
```

The deployment script loads a saved genetic-agent checkpoint and launches the Pygame visualization.

## Note

This repository preserves the original 2023 course-project code and trained-model checkpoints. The deployment script currently loads a saved checkpoint from `Project_5/v1/5`.

