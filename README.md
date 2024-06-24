## Project Description

This project involves generating analog pulse modulated signals from an arbitrary message signal  m(t). The goal is to create a GUI application that allows users to input specific parameters and visualize the results. The GUI application includes the following features:

### Inputs
- **Message signal m(t)**: Provided in the form of two vectors, \( t \) and \( m \).
- **Sampling Time \( T_s \)**: The time interval between samples.

### Options
- **Type of modulation**: Selectable from:
  1. Pulse Amplitude Modulation (PAM)
  2. Flat-top PAM
  3. Pulse Width Modulation (PWM)
  4. Pulse Position Modulation (PPM)
- **Value of \( T \)**: For PAM, flat-top PAM, and PPM.
- **Value of \( A \)**: For PWM and PPM.

### Outputs
- A figure with four vertically aligned subplots showing:
  1. The original message signal m(t)
  2. The pulse signal p(t)
  3. The modulated signal
  4. The demodulated signal

### Test Cases
The GUI and code are tested with the following cases to ensure accuracy and functionality:

#### Test Case 1:
- **Message signal**:
   ```math
       m(t) = 3 \cos(4\pi t) 
   ```
    where \( t = 0:0.001:1 \)
- **Sampling Time \( T_s \)**: 1/8 sec
- **Modulation Types**:
  - PAM and flat-top PAM with \( T = 0.25T_s \)
  - PWM with \( A = 2 \)
  - PPM with \( A = 2 \) and \( T = 0.1T_s \)

#### Test Case 2:

  - **Message signal**: m(t) defined as
  
  ```math
  m(t) = 
  \begin{cases} 
  2t & \text{for } 0 \le t \le 4 \\
  16 - 2t & \text{for } 4 \le t \le 8 
  \end{cases}
  ```
  where \( t = 0:0.01:8 \)

- **Sampling Time \( T_s \)**: 0.4 sec
- **Modulation Types**:
  - PAM with \( T = 0.1 \) sec
  - Flat-top PAM with \( T = 0.4 \) sec
  - PWM with \( A = 2 \)
  - PPM with \( A = 2 \) and \( T = 0.05 \) sec

This project provides a comprehensive tool for visualizing various analog pulse modulation techniques, ensuring a clear understanding of the modulation and demodulation processes through interactive and graphical representation.

