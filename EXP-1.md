# GENERATION OF STANDARD DISCRETE-TIME SIGNALS
# AIM:
To generate and plot standard discrete-time signals using MATLAB.
# APPARATUS REQUIRED:
•	Computer / Laptop
•	MATLAB software
# THEORY:
Discrete-time signals are signals defined only at integer values of time (n).
These signals are basic building blocks in Digital Signal Processing (DSP) and are used for system analysis, filtering, and signal modeling.
Standard discrete-time signals include:
	Unit Impulse
	Unit Step
	Ramp
	Exponential
	Sinusoidal
	Damped Sinusoidal
In MATLAB, discrete-time signals are represented using vectors and plotted using the stem() command.
 Standard Discrete-Time Signals
 
🔹 1. Unit Impulse Signal
δ(n)={(1,n=0
       0,n≠0)}

🔹 2. Unit Step Signal
u(n)={(1,n≥0
       0,&n<0)}

🔹 3. Ramp Signal
r(n)=n⋅u(n)

🔹 4. Exponential Signal
x(n)=a^n

🔹 5. Sinusoidal Signal
x(n)=sin⁡(ωn)

🔹 6. Damped Sinusoidal Signal
x(n)=a^n sin⁡(ωn)

# ALGORITHM:
1.	Start the program
2.	Define the sample index n
3.	Generate each standard discrete-time signal
4.	Plot the signal using stem()
5.	Label the axes and title
6.	Stop the program

# MATLAB CODE:
~~~
% GENERATION OF STANDARD DISCRETE-TIME SIGNALS

clc;
clear;
close all;

%% Sample index
n = -10:10;

%% 1. Unit Impulse Signal
x1 = (n == 0);
figure;
stem(n, x1, 'filled');
title('Unit Impulse Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 2. Unit Step Signal
x2 = (n >= 0);
figure;
stem(n, x2, 'filled');
title('Unit Step Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 3. Ramp Signal
n1 = 0:10;
x3 = n1;
figure;
stem(n1, x3, 'filled');
title('Ramp Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 4. Exponential Signal
a = 0.8;
x4 = a.^n1;
figure;
stem(n1, x4, 'filled');
title('Exponential Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 5. Sinusoidal Signal
x5 = sin(0.3*pi*n1);
figure;
stem(n1, x5, 'filled');
title('Sinusoidal Signal');
xlabel('n'); ylabel('Amplitude');
grid on;

%% 6. Damped Sinusoidal Signal
x6 = (0.9.^n1).*sin(0.4*pi*n1);
figure;
stem(n1, x6, 'filled');
title('Damped Sinusoidal Signal');
xlabel('n'); ylabel('Amplitude');
grid on;
~~~

# OUTPUT GRAPH:
# 1. Unit Impulse Signal
<img width="905" height="442" alt="Screenshot 2026-03-28 155751" src="https://github.com/user-attachments/assets/6aa1ecdb-823f-4f25-bb50-3772db49994a" />

# 2. Unit Step Signal
<img width="933" height="441" alt="Screenshot 2026-03-28 155850" src="https://github.com/user-attachments/assets/96ad609c-9f60-4107-ac88-5e13e3447ec6" />

# 3. Ramp Signal
<img width="914" height="442" alt="Screenshot 2026-03-28 155933" src="https://github.com/user-attachments/assets/51879dcb-328f-4f54-9a48-1dd3cf4156a6" />

# 4. Exponential Signal
<img width="916" height="446" alt="Screenshot 2026-03-28 160019" src="https://github.com/user-attachments/assets/2ed1b4bd-8e28-4627-9433-44f9f800330c" />

# 5. Sinusoidal Signal
<img width="936" height="445" alt="Screenshot 2026-03-28 160048" src="https://github.com/user-attachments/assets/9100a59e-b86b-4f4c-88b6-8ee8b0f25751" />

# 6. Damped Sinusoidal Signal
<img width="937" height="450" alt="Screenshot 2026-03-28 160112" src="https://github.com/user-attachments/assets/19d26bac-11ba-40ea-ab12-c1b52eaa4eff" />

# Result :
Thus, standard discrete-time signals were successfully generated and plotted using MATLAB.


