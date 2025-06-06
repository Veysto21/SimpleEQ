# 🎛️ SimpleEQ – Real-Time Audio Equalizer Plugin

**SimpleEQ** is a real-time audio equalizer plugin built with the JUCE framework. It features customizable frequency bands, interactive GUI elements, and a live response curve to give users precise tonal control within any DAW that supports VST or AU plugins.

---

## ✨ Features

- 🎚️ Peak, Low-Cut, and High-Cut EQ bands
- 🔗 Real-time parameter control via sliders
- 🎨 Custom-drawn response curve with grid overlay
- 📊 Real-time spectrum analyzer
- 🚫 Per-band bypass functionality
- 🧱 Modular DSP structure using JUCE's `ProcessorChain`
- 🎛️ Clean, customizable user interface
- 🔌 VST3 and AU plugin support (via JUCE)

---

## 📖 Project Overview

This project is based on a tutoraial (https://www.youtube.com/watch?v=i_Iq4_Kd7Rc&list=WL&index=6&t=1790s) and a fully functional audio equalizer plugin built using the JUCE framework, following a modular and DSP-focused development approach. It begins with setting up a new JUCE project and configuring it to support real-time audio processing. Once the foundational setup is complete, audio parameters are created to control various aspects of the EQ, such as peak frequency, gain, and Q values, as well as low-cut and high-cut filter controls.

The next step involves integrating the digital signal processing (DSP) components, which includes designing and implementing IIR filters using JUCE's `ProcessorChain` and `Filter` classes. These filters are used to shape the sound by adjusting frequency content based on the user’s input. Audio parameters are then connected to these filters to ensure the plugin responds dynamically to user input from the interface.

Once the DSP is functioning, a custom graphical user interface (GUI) is developed to enhance usability. This includes adding interactive sliders for all filter parameters, allowing users to tweak EQ settings in real-time. A custom-drawn response curve is implemented to visually represent the EQ curve, helping users see how the audio signal is being shaped. To improve visual clarity and feedback, a grid overlay and spectrum analyzer are added, enabling users to observe both the static EQ curve and the real-time frequency spectrum of the audio input.

Further enhancements include the creation of bypass buttons, allowing each filter band or section to be disabled independently for A/B comparisons or tonal control. The sliders are visually customized for a professional and intuitive experience, and the response curve is built as a reusable component to maintain modularity and ease of future expansion.

This EQ app combines real-time DSP, audio parameter management, and interactive visualization to deliver a responsive and polished equalizer plugin that can be integrated into digital audio workstations (DAWs) via VST or AU formats.

---

## 🔧 Build Instructions 

> Requires: JUCE 7, C++17, and a DAW (or JUCE AudioPluginHost)

1. Clone the repo  
2. Open the `.jucer` file in Projucer or open the Visual Studio project  
3. Build the plugin using the selected exporter (e.g., VST3)  
4. Load into a DAW or JUCE’s AudioPluginHost to test


