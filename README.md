# Computational-Data-Analysis-on-Fluids
Background
Hot-wire anemometry is a measurement technique used to determine the velocity of fluids in the gas phase.
Hot-wire anemometry is commonly used in aerodynamics research and engineering applications such as
wind tunnel testing, combustion analysis, and HVAC system design. It involves the use of a small wire, typically
made of tungsten or platinum, which is heated to a high temperature using an electrical current; see Figure 1
for different probes. As the fluid flows passes the wire, the temperature of the wire drops, causing a change
in its resistance. This change in resistance can be measured and calibrated to calculate the velocity of the
fluid.
Figure 1: Samples of Hot-wire probes using different materials .
A TSI 1210-T1.5 hot-wire U-probe is used to measure the fluctuations in voltage of the probe due to the
turbulent air jet, see Figure 2. Velocity can be obtained from the measurements of voltage change and the
provided calibration curve; the data is available for sampling frequency of 10 [kHz].

TASKS 
For the given data (first column = time, and the second column = voltage change), accessible via Canvas
course shell under the corresponding assignment, do the following:
1. (10 points) Read the signal using your scripting language of choice, that is MATLAB, Python, or Julia,
and use the following calibration curve to convert the change in voltage to velocity.
(Voltage +1)2 = 0.3224 × u
0.46 + 0.5143
where u is the instantaneous velocity. Once the velocity is obtained, plot the record versus time.
2. (15 points) The signal is very long; in these situations, it is common to divide the signal in equal chunks
and create an ensemble. Create an ensemble of 1000 signals and plot the first three records versus
time.
3. (10 points) Calculate the ensemble mean velocity and visualize it against time.
4. Reynolds decomposition separates a turbulent velocity signal (u) into the mean (time-averaged) component (U) and the fluctuating component (u
′
). As a result, one can show the instantaneous velocity
as u(t) = U(t) + u
′
(t).
1. (15 points) For the first three records in the ensemble, calculate the empirical PDF of the u
′ and
visualize them.
2. (5 points) Are the obtained PDFs following the Gaussian distribution?
3. (10 points) For each record (realization) in the ensemble, calculate the power spectral density
(PSD) for the u
′
.
4. (10 points) Calculate the ensemble mean of the PSDs in part 4.3. and visualize it against the cyclic
frequency.
5. (25 points) Calculate and visualize the spectrogram of the velocity fluctuations u
′
for the entire
data (not the created ensemble in problem 2). Compare this with a spectrogram of a single
record from the ensemble, and discuss your observations from the localization of the time and
frequencies.
