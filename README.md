# BB84 Quantum Key Distribution Visual Simulator

---

### Description

A Python-based application that provides an interactive and educational tool for understanding the BB84 Quantum Key Distribution (QKD) protocol. The simulator allows you to visualize the key exchange process, analyze results, and explore different backends, including real quantum hardware.

---

### 🔧 Features

* **Interactive Controls:** Easily adjust simulation parameters like the number of qubits, Eve's intercept probability, and channel noise.

* **Multiple Backends:** Run simulations on a **classical mathematical model**, Qiskit's **Aer Simulator**, or a real **IBM Quantum device**.

* **Animated Visualization:** See qubits travel from Alice to Bob in an animated flow, highlighting how Eve's interception affects the process.

* **Post-processing:** Simulate **error correction (EC)** and **privacy amplification (PA)** to see how keys are secured.

* **Detailed Metrics:** Get key insights with metrics such as sifted key length, QBER, and final key length.

* **Comprehensive Logs:** A log panel tracks each step of the protocol for full transparency.

---

### 🛠️ Tech Stack

| Tool / Library | Purpose |
| :--- | :--- |
| **Python 3.11** | Core programming language |
| **Streamlit** | Building the interactive web application |
| **NumPy** | Numerical operations and array handling |
| **Pandas** | Data manipulation for tables and metrics |
| **Plotly** | Creating interactive graphs and animations |
| **Qiskit** | Building quantum circuits and running on backends |
| **Qiskit Aer** | Simulating quantum circuits with noise models |
| **Qiskit IBM Runtime** | Connecting to and running on IBM's real quantum hardware |

---

### 🚀 How to Run

1.  Clone the repository or save the `app.py`, `bb84_backend.py`, and `requirements.txt` files into a single directory.

2.  Open your terminal and navigate to the project directory.

3.  Install the required libraries:

    ```bash
    pip install -r requirements.txt
    ```

4.  Run the Streamlit application:

    ```bash
    streamlit run app.py
    ```

    The application will open automatically in your web browser.

---

### 📝 Usage

Once the application is running, you can use the sidebar to control the simulation:

* **Scenario Presets:** Quickly load predefined scenarios like "Clean Fiber" or "Aggressive Eve."

* **Simulation Controls:** Manually fine-tune parameters for a custom simulation.

* **Backend Selection:** Switch between the classical simulator, Aer simulator, and a real quantum device.

* **Run Simulation:** Click the button to start the protocol and watch the animation unfold.
