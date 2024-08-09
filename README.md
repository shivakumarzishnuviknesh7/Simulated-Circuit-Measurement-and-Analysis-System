
### Project Title:
**Simulated Circuit Measurement and Analysis System**

## Project Overview
This project is a simulated measurement and analysis system for a simple electrical circuit. The system calculates and monitors voltage, current, and resistance over time, using virtual instruments like voltmeters, ammeters, ohmmeters, and a rolling average ohmmeter. The goal is to provide a dynamic simulation that can help in understanding the behavior of electrical components in a circuit.

## Features
- **Voltmeter**: Measures the voltage across a load resistor \( R_L \) over time.
- **Ammeter**: Measures the current through the load resistor \( R_L \).
- **Ohmmeter**: Calculates the resistance of \( R_L \) using the measured voltage and current.
- **Rolling Average Ohmmeter**: Computes a rolling average of the resistance to smooth out fluctuations and provide a more stable measurement over time.

## Circuit Diagram
The circuit under analysis consists of the following components:
- **Voltage Source \( V_S \)**
- **Resistors \( R_1 \), \( R_2 \), and \( R_L \)**
- **Voltmeter** connected across \( R_L \)
- **Ammeter** in series with \( R_L \)


## Usage
The simulation outputs the voltage, current, calculated resistance, and rolling average resistance at specific time intervals. These outputs can be used to analyze the circuit's behavior and verify theoretical calculations.

### Example Output
[Voltmeter] Time: 0.00s, Voltage: 2.31V
[Ammeter] Time: 0.00s, Current: 7.69e-05A
[Ohmmeter] Time: 0.00s, Calculated RL: 30000.00Ω
[RollingAverageOhmmeter] Time: 0.00s, Rolling Avg RL: 30000.00Ω

- **circuit_simulator.py**: Manages the simulation, handles timing, and updates instrument readings.
- **voltmeter.py**: Simulates the voltmeter and outputs voltage readings.
- **ammeter.py**: Simulates the ammeter and outputs current readings.
- **ohmmeter.py**: Calculates the resistance based on voltage and current.
- **rolling_average_ohmmeter.py**: Calculates a rolling average of the resistance.
- **main.py**: Entry point for the simulation. Initializes and runs the simulation.

## Installation
1. Clone the repository.
2. Ensure that you have Python 3.x installed.
3. Navigate to the project directory.
4. Install any required dependencies (if any) using `pip`:
   ```bash
   pip install -r requirements.txt

## Run the simulation
python src/circuit_simulation/main.py



## Requirements
- Python 3.x

## Acknowledgements
This project was developed to demonstrate basic circuit simulation techniques using Python. The circuit diagram and output analysis were essential for verifying the correctness of the simulation.

---

### Notes:
- The file paths in the structure should reflect the actual file structure of your project.
- The `requirements.txt` should list any third-party Python packages your project depends on. If you didn't use any, this step can be skipped.
- Replace the placeholder path to the circuit diagram image with the correct one, or include the image in the project folder.

