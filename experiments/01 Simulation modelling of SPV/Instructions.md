**Aim:**

To model and design a 1kW solar photovoltaic system using MATLAB Simulation to obtain the solar parameters and the solar PV characteristics curves.

**Software Tool Used:**

MATLAB 2021 or above

**Modelling Parameters:**

No. of solar cells = 216

No. of series cells per panel = 36

Short circuit current per panel = 2.54A

Open circuit voltage per cell = 21.80V

Irradiance = 1000 W/m2

Quality factor = 1.6

Cell resistance (series) = 5.10mΩ

Temperature at STC = 25 deg.C

Resistive load = 10Ω

**Theory:**

The theory of solar cells explains the process by which light energy in photons is converted into electric current when the photons strike a suitable semiconductor device. The theoretical studies are of practical use because they predict the fundamental limits of a solar cell, and give guidance on the phenomena that contribute to losses and solar cell efficiency. Photons in sunlight hit the solar panel and are absorbed by semi-conducting materials.
Electrons (negatively charged) are knocked loose from their atoms as they are excited. Due to their special structure and the materials in solar cells, the electrons are only allowed to move in a single direction. The electronic structure of the materials is very important for the process to work, and often silicon incorporating small amounts of boron or phosphorus is used in different layers. An array of solar cells converts solar energy into a usable amount of direct current (DC) electricity.

The photon can pass straight through the silicon — this (generally) happens for lower energy photons. The photon can reflect off the surface. The photon can be absorbed by the silicon if the photon energy is higher than the silicon band gap value. This generates an electron-hole pair and sometimes heat depending on the band structure.

**Circuit Diagram:**

<img width="927" height="587" alt="image" src="https://github.com/user-attachments/assets/d5c7af0d-e498-44ac-b8ea-9a7f931e3db4" />
**Simulation Model**

<img width="903" height="620" alt="image" src="https://github.com/user-attachments/assets/81802f68-c377-4936-a987-6c89673cb243" />
**Procedure: (Practice video: https://www.youtube.com/watch?v=n1dQzP6-H20**

1.	Open MATLAB
2.	From Simulink library browser, pick the following components
  a.	solar cell
  b.	constant
  c.	PS converter, S converter
  d.	Current sensor, voltage sensor
  e.	Variable resistor
  f.	Ramp
  g.	Scope, XY graph
3.	Connect the thirty-six solar cells in series with common irradiation and make it as a subsystem to form a panel.
4.	Form similar six panel and connect them in series to form an array with single irradiance input.
5.	Create a subsystem for the six panels.
6.	Connect the constant block with a value of 687 to the irradiance input through PS converter.
7.	From the output of the solar array connect a current sensor in series to the positive terminal and voltage sensor across the terminals.
8.	Connect a variable resistor across the solar pv array terminal.
9.	Connect a ramp signal to the variable resistor through the PS connector.
10.	 Using Simulink converter, connect the terminals of the current sensor and voltage sensor to the scope to record the graph.
11.	Use divide block and convert to multiplication operation and multiply the current and voltage outputs to get the power output.
12.	Set the minimum and maximum range in X-Y graph to obtain the IV and PV characteristics.
**Tabulation:**

<img width="913" height="201" alt="image" src="https://github.com/user-attachments/assets/3f9e372e-4039-4b5c-affb-bf34151c51fa" />
**Model Graph**

<img width="469" height="248" alt="image" src="https://github.com/user-attachments/assets/71ace438-7af3-4629-a219-0a884a1152f8" />
<img width="464" height="219" alt="image" src="https://github.com/user-attachments/assets/02cefcbc-69fe-4e12-b7fc-dcde369a89c8" />
**Result:**

Thus, the solar PV energy system is simulated using MATLAB and the I-V and P-V graphs are determined for the given panel rating.


