**Aim:**

To simulate solar powered DC/DC boost converter using MATLAB Simulation for the output voltage control using P-I Controller

**Software Tool used:**

MATLAB 2014 or above

**Modelling Parameters:**
1. Maximum voltage = 120V
2. Irradiance = 1000W/m2
3. Temperature at STC = 25 deg. C
4. Inductor, L = 100µH
5. Capacitor, C = 1000µF
6. Load Resistance = 350 W
7. Reference voltage = 100V to 300V
8. P constant = 0.01
9. I constant = 5
10. Time domain = Continuous
11. Switching frequency = 10kHz

**Circuit Diagram:**

<img width="501" height="272" alt="image" src="https://github.com/user-attachments/assets/7be7d64c-592e-42fa-af23-27e1c32a6a3a" />

**Simulation Diagram:**

<img width="1434" height="638" alt="image" src="https://github.com/user-attachments/assets/80b039b8-7164-4062-92e3-61b67aa79805" />

**Theory:**

Closed-loop proportional-integral (PI) control is a widely used technique for regulating the output voltage in a DC-DC boost converter. It helps maintain a stable and accurate output voltage despite variations in input voltage, load current, and other operating conditions. Here's a step-by-step explanation of how closed-loop PI control works in a boost converter:

**Components of the Control System:**

**Boost Converter:** This is the DC-DC converter responsible for increasing the output voltage.

**Reference Voltage (Vref):** This is the desired or setpoint output voltage that you want to achieve and maintain.

**Feedback System:** The feedback system measures the actual output voltage (Vout) using a voltage sensor or divider network and provides this information to the controller.

**Controller (PI Controller):** The controller calculates the error (the difference between the reference voltage and the measured output voltage) and generates a control signal based on this error. The PI controller has two components:

1. **Proportional (P) Component:** The proportional component generates a control signal proportional to the error. It helps reduce steady-state error and provides a quick response to changes in the error.

2. **Integral (I) Component:** The integral component accumulates the error over time and generates a control signal that eliminates any steady-state error. It helps in dealing with long-term deviations from the reference voltage.

By using a closed-loop PI control system, a boost converter can provide accurate and stable output voltage regulation, making it suitable for various applications, including power supplies and battery charging systems. The proportional and integral gains (Kp and Ki) need to be properly tuned to ensure good control system performance

**Procedure:**
1.	Open MATLAB
2.	From Simulink library browser, pick the following components
  a.	Solar Panel
  b.	Current and voltage measurement
  c.	MOSFET, Diode, Inductor and capacitor
  d.	RLC series load
  e.	Constant, subtract, PI controller and PWM generator
  f.	Slider, Scope, display
3.	Connect the Simulink library tools as shown in the circuit diagram.
4.	Connect the slider tool with the constant block used for the reference value.
5.	Set the parameters as per the required design.
6.	Simulate the work for the different reference voltage by sliding the slider. 
7.	Note the input and output side parameters and tabulate it.

**Tabulation:**

<img width="618" height="316" alt="image" src="https://github.com/user-attachments/assets/5ae83473-e300-4be8-8e78-c24fe8ddc4e7" />

**Formula:**

Input Power (W) = Input Voltage x Input Current

Output Power (W) = Output Voltage x Output Current

Efficiency (%) = (Output Power / Input Power) x 100

**Model Graph:**

<img width="616" height="241" alt="image" src="https://github.com/user-attachments/assets/3dbf5e60-8d2d-4c17-a592-7a1913d59081" />

**Result:**

Thus, the closed loop output voltage control of solar powered dc/dc boost converter using PI controller is simulated using MATLAB
