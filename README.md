# BB84
A Python application built with Streamlit that provides an interactive and educational tool for understanding the BB84 Quantum Key Distribution protocol. Simulate key exchange, visualize qubit flow, and analyze key metrics like the Quantum Bit Error Rate (QBER).


# BB84 Quantum Key Distribution Visual Simulator

# Description
The BB84 Visual Simulator is a Python application built with Streamlit that provides an interactive and educational tool for understanding the BB84 Quantum Key Distribution (QKD) protocol. It allows you to simulate the key exchange process, visualize the flow of qubits between Alice, Eve, and Bob, and analyze the results, including the Quantum Bit Error Rate (QBER).

The simulator features multiple backends, including a classical mathematical model, Qiskit's Aer simulator, and a path for running on real IBM Quantum hardware. It also includes post-processing steps such as error correction and privacy amplification.

# Key Features
Interactive Simulation: Adjust parameters like the number of qubits, Eve's intercept probability, and channel noise in a real-time environment.

Multiple Backends: Run the simulation on a classical math simulator, Qiskit's Aer Simulator with noise models, or on an IBM Quantum device.

Animated Visualization: Watch the qubits travel from Alice to Bob, with a detailed view of how Eve's interception affects the process.

Key Post-processing: Simulate Cascade-lite error correction (EC) and BLAKE2s privacy amplification (PA) to see how keys are refined after the initial exchange.

Detailed Metrics: View key metrics such as sifted key length, QBER, and the final key length after post-processing.

Comprehensive Logs: A log panel tracks each step of the protocol, from preparation to key reconciliation.


# Getting Started
To run this application, you will need Python 3.11 and the required libraries.

Clone this repository or save the app.py, bb84_backend.py, and requirements.txt files to a single directory on your computer.

Open your terminal or command prompt and navigate to the project directory.

Install the required Python libraries by running the following command:

# pip install -r requirements.txt

This will install streamlit, numpy, pandas, plotly, qiskit, qiskit-aer, and qiskit-ibm-runtime.

# Run the application using Streamlit:

streamlit run app.py

The application will open in your web browser.


# Usage
Once the application is running, you can use the sidebar to control the simulation:

Scenario Presets: Choose from predefined scenarios like "Clean Fiber" or "Aggressive Eve" to quickly load settings.

Simulation Controls: Manually adjust the number of qubits, Eve's intercept probability, and other parameters.

Backend Selection: Switch between the classical simulator, Aer simulator, and a real quantum device.

Run Simulation: Click the ▶ Run Simulation button to start the protocol and watch the animation.


# Dependencies
The dependencies for this project are listed in the requirements.txt file and include popular libraries for data science, visualization, and quantum computing.

streamlit
numpy
pandas
plotly
qiskit
qiskit-aer
qiskit-ibm-runtime
