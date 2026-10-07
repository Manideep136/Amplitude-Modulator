# Amplitude-Modulator

📌 Project Overview

This project is an Amplitude Modulator (AM) circuit designed and implemented as a PCB using KiCad.

Amplitude modulation is a technique used in communication systems where the amplitude of a high-frequency carrier signal is varied according to the amplitude of a lower-frequency message signal.

The purpose of this project is to understand the basic concept of AM and implement a simple amplitude modulation circuit using electronic components.

🎯 Objectives
Understand the basic concept of amplitude modulation.
Generate a carrier signal and message signal.
Combine the signals to produce an AM waveform.
Design the AM circuit schematic in KiCad.
Assign appropriate footprints to components.
Create a PCB layout.
Route the PCB tracks.
Perform ERC and DRC checks.
Visualize the completed PCB using KiCad 3D Viewer.
📡 What is Amplitude Modulation?

Amplitude Modulation (AM) is a modulation technique in which the amplitude of a carrier signal is changed according to the message signal, while the carrier frequency remains constant.

In simple terms:

Message Signal + Carrier Signal
              │
              ▼
       AM Modulator Circuit
              │
              ▼
          AM Output

The message signal contains the information, while the carrier signal is a higher-frequency signal used to carry that information.

⚙️ Working Principle

The amplitude modulator takes two input signals:

Message signal – the information signal.
Carrier signal – a high-frequency signal.

The modulator combines these signals and produces an amplitude-modulated output.

The basic AM equation is:

s(t) = Ac [1 + μ cos(ωm t)] cos(ωc t)

Where:

Ac = Carrier amplitude
μ = Modulation index
ωm = Message signal angular frequency
ωc = Carrier signal angular frequency

The frequency of the carrier remains constant, while its amplitude changes according to the message signal.


🧩 Components Used

The exact components depend on the circuit implementation. A typical AM modulator PCB may contain:

Reference	Component	Quantity
Q1	Transistor / Modulator Device	1
R1–R4	Resistors	As required
C1–C3	Capacitors	As required
J1	Message Signal Input	1
J2	Carrier Signal Input	1
J3	AM Output	1
VCC	DC Power Supply	1

Component values should be selected according to the actual schematic used in the project.

🔌 Inputs and Outputs
Message Input

The low-frequency information signal is connected to the message input.

Message Signal
      │
      ▼
   AM Circuit
Carrier Input

The high-frequency carrier signal is supplied to the carrier input.

Carrier Signal
      │
      ▼
   AM Circuit
AM Output

The resulting amplitude-modulated signal is available at the output connector.

Message + Carrier
       │
       ▼
 AM Modulator
       │
       ▼
   AM Output
🖥️ KiCad Design

The complete circuit was designed using KiCad.

Design Process
Create a new KiCad project.
Create the AM modulator schematic.
Add the required components.
Connect the components according to the circuit.
Add power connections.
Assign footprints.
Transfer the schematic to PCB Editor.
Place the components.
Route the PCB tracks.
Check the design using ERC.
Check the PCB using DRC.
View the final PCB using the 3D Viewer.

🔍 PCB Design Considerations

When designing the AM PCB, special attention should be given to:

Short signal paths.
Proper grounding.
Correct component placement.
Avoiding unnecessary long tracks.
Keeping the carrier signal path clean.
Proper separation of input and output signals.
Correct footprint selection.
Appropriate PCB track widths.

Since AM circuits can work with relatively higher-frequency signals, good PCB layout practices help reduce unwanted noise and interference.

🧪 Testing

After completing the PCB:

Check all component values.
Verify component orientation.
Check transistor pin configuration if a transistor is used.
Check capacitor polarity for polarized capacitors.
Verify the power supply connections.
Run ERC in KiCad.
Run DRC in KiCad.
Check the PCB for shorts.
Apply the required DC supply.
Connect the message signal.
Connect the carrier signal.
Observe the output using an oscilloscope.

The oscilloscope should show an AM waveform whose envelope follows the message signal.

📈 Modulation Index

The modulation index indicates how strongly the carrier is being modulated.

It can be calculated from the AM waveform as:

μ = (Vmax - Vmin) / (Vmax + Vmin)

Where:

Vmax = Maximum envelope amplitude
Vmin = Minimum envelope amplitude

For normal AM operation:

0 ≤ μ ≤ 1

If the modulation index becomes greater than 1, over-modulation can occur, which causes distortion.

✅ Advantages
Simple concept and easy to understand.
Useful for learning communication-system fundamentals.
Easy to observe using an oscilloscope.
Demonstrates the relationship between message and carrier signals.
Can be extended into a complete communication system.
⚠️ Limitations
AM is less power-efficient than some modern modulation techniques.
A significant amount of power can be present in the carrier.
It is susceptible to noise.
Over-modulation can cause distortion.
Practical performance depends on the circuit design and component selection.
🚀 Future Improvements

The project can be improved by adding:

Adjustable modulation depth.
Variable carrier frequency.
Signal amplification stage.
RF output stage.
LC filtering.
Audio input connector.
Oscilloscope test points.
Demodulator circuit.
Complete AM transmitter and receiver.
📚 Learning Outcomes

Through this project, I learned:

Basic principles of amplitude modulation.
Difference between message and carrier signals.
AM waveform generation.
Modulation index.
Schematic design using KiCad.
Component and footprint selection.
PCB component placement.
PCB routing.
ERC and DRC checking.
PCB testing using an oscilloscope.
🛠️ Software Used

KiCad 9.0

⚠️ Safety Notice

This project should be operated using the specified low-voltage supply and signal levels for the circuit.

Do not connect the circuit directly to mains voltage or unauthorized RF equipment. Use appropriate laboratory equipment and follow the ratings of all components.

📄 License

This project is created for educational purposes. You may modify, improve, and use the design for learning and personal electronics projects.
