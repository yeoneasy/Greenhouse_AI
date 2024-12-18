# SmartGreenhouseAI

SmartGreenhouseAI is a project focused on developing AI-based prediction and visualization techniques for smart greenhouse environments. The goal is to maintain optimal conditions for plant growth by leveraging advanced machine learning models and data visualization tools.

## Features
- **Data-Driven Insights**: Analyze time-series data from greenhouse sensors.
- **AI Predictions**: Predict internal temperature and control values using LSTM and reinforcement learning.
- **Visualization**: Generate interactive graphs and dashboards for monitoring greenhouse conditions.
- **Control Optimization**: Adjust actuators dynamically based on AI predictions.

## Data Description
The project uses real-world greenhouse data, including:
- **External Data**: Temperature, wind direction, wind speed, solar radiation, rainfall, etc.
- **Internal Data**: Temperature, humidity.
- **Control Data**: Heating and ventilation setpoints.
- **Actuator Data**: Opening percentages of windows, curtains, and valve positions.

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/SmartGreenhouseAI.git
    cd SmartGreenhouseAI
    ```
2. Create and activate a virtual environment:
    ```bash
    python -m venv env
    source env/bin/activate  # On Windows: env\Scripts\activate
    ```
3. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
4. Ensure all required datasets are available in the `data/` directory.

## Usage
### Training the Model
Run the following command to train the LSTM model:
```bash
python train_lstm.py
```

### Reinforcement Learning
Use the `train_rl.py` script to train the RL model:
```bash
python train_rl.py
```

### Visualization
Launch the visualization dashboard:
```bash
python visualize.py
```

## Directory Structure
```
SmartGreenhouseAI/
├── data/
│   ├── raw/               # Raw greenhouse datasets
│   ├── processed/         # Preprocessed datasets
├── models/                # Trained model files
├── notebooks/             # Jupyter notebooks for analysis
├── src/                   # Source code
│   ├── data_processing/   # Scripts for preprocessing data
│   ├── models/            # Model architectures
│   ├── rl/                # Reinforcement learning modules
├── requirements.txt       # Required Python packages
├── train_lstm.py          # Script for training LSTM model
├── train_rl.py            # Script for training RL model
├── visualize.py           # Script for data visualization
```

## Requirements
- Python 3.8+
- TensorFlow or PyTorch
- Matplotlib
- Pandas
- NumPy

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

## Contact
For any inquiries or collaboration opportunities, please reach out to:
- **Your Name**: your.email@example.com
- **GitHub**: [yourusername](https://github.com/yourusername)

---
Thank you for using SmartGreenhouseAI! Together, we can optimize agricultural efficiency through technology.
