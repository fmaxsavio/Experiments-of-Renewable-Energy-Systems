**Aim:**

To simulate solar powered DC/DC boost converter using MATLAB Simulation and obtain the I-V and P-V characteristics by changing the duty cycle.

**Software Tool Used:**

MATLAB 2021 or above

**Modelling Parameters:**
Maximum voltage = 120 V
Temperature at STC = 25 deg. C
Inductor, L = 100µH
Capacitor, C = 1000µF
Switching frequency = 25kHz
Load Resistance = 350 W
Duty cycle = 10% to 80%

**Circuit Diagram**

<img width="927" height="428" alt="image" src="https://github.com/user-attachments/assets/9763f3b3-22cf-4b81-ad6c-cee461464d2e" />


**Simulation Model:**

<img width="1434" height="638" alt="image" src="https://github.com/user-attachments/assets/1b9bc082-cf3f-4e04-8d4c-9112cd67dd37" />

**Theory:**

DC-DC boost converters play a crucial role in solar power systems by efficiently increasing the voltage output of solar panels to match the requirements of the load or energy storage system. A boost converter, also known as a step-up converter, is a type of DC-DC converter that increases the output voltage level compared to the input voltage. It operates by storing energy in an inductor and then releasing it to the output at a higher voltage.

Input Voltage (Vin): The input voltage is the voltage supplied to the boost converter, typically coming from a source like a battery or a solar panel.

Switch (S): The switch is a semiconductor device, often a transistor or a MOSFET, that alternately connects and disconnects the input voltage to the rest of the circuit. It operates in a switching mode, where it is either fully ON (conducting) or fully OFF (non-conducting).

Inductor (L): The inductor is a coil of wire wound around a core. It stores energy in its magnetic field when the switch is ON and releases this energy to the output when the switch is OFF. The inductor plays a crucial role in boosting the voltage.

Diode (D): A diode is connected in parallel with the load (output) and allows current to flow in one direction only. It prevents backflow of current from the output to the input when the switch is OFF.

Output Voltage (Vout): The output voltage is the higher voltage level that you want to achieve.

The boost converter operates in two main modes: the ON mode (when the switch is closed) and the OFF mode (when the switch is open). Here's how it works step by step:

ON Mode (Switch Closed): When the switch (S) is closed (ON), current flows from the input voltage (Vin) through the inductor (L) and into the switch. As current flows through the inductor, it stores energy in its magnetic field, causing the inductor's current to increase gradually.

Transition to OFF Mode (Switch Opening): After a certain period (determined by the switching frequency), the switch is opened (turned OFF). When the switch opens, the inductor wants to maintain the current flow, and this is where the boost action occurs.

OFF Mode (Switch Open): With the switch open, the inductor's stored energy is released. The diode (D) provides a path for the current to flow in a loop, and it forces the current to pass through the load (output).
As the inductor releases energy, it effectively adds to the input voltage, creating a higher voltage at the output (Vout).

Output Voltage Regulation: The duty cycle of the switch (the ratio of ON time to total switching period) is controlled by a feedback mechanism to regulate the output voltage. By adjusting the duty cycle, the boost converter can maintain a stable output voltage even when the input voltage varies or when the load changes. The boost converter's output voltage (Vout) is typically higher than the input voltage (Vin) and is determined by the duty cycle, the inductance of the inductor, and the input voltage.

In summary, a boost converter is a DC-DC converter that increases the output voltage by storing energy in an inductor during the ON state and releasing it to the output during the OFF state, thereby providing a higher output voltage level than the input voltage.

**Procedure:**
1.	Open MATLAB
2.	From Simulink library browser, pick the following components
  a.	Solar Panel
  b.	Current and voltage measurement
  c.	MOSFET, Diode, Inductor and capacitor
  d.	RLC series load
  e.	Scope, display
3.	Connect the Simulink library tools as shown in the circuit diagram.
4.	Set the parameters as per the required design.
5.	Simulate the work for the duty cycles from 10% to 80%.
6.	Note the input and output side parameters and tabulate it.
7.	Plot the I-V, P-V graph for the values obtained

**Tabulation:**
<img width="692" height="464" alt="image" src="https://github.com/user-attachments/assets/ce7a1281-3c0c-4d99-89db-9af88595ad42" />

**Model Graph**

<img width="1305" height="357" alt="image" src="https://github.com/user-attachments/assets/e8d178be-4a0f-4934-a920-0e81dc97db31" />

**Result:**
Thus, the solar powered dc/dc boost converter is simulated using MATLAB and the I-V and P-V graphs are plotted for various values of duty cycles.
