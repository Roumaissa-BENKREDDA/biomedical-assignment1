# biomedical-assignment1
<div align="center">
  <a href="https://your-university-link.com/">
    <img src="img/logounige.jpg" width="20%" height="20%" title="University of Genoa" alt="University of Genoa">
  </a>
</div>

<h1 align="center"> Biomedical Robotics - EMG Assignment </h1>

> **Authors:**
> - *Roumaissa Benkredda*  
> - *Karim Triki*  
> - *Ines Haouala*  
>
> **Professor:**
> - *Maura Casadio*
>
> **Submission Date:** November 9th, 2023

## Table of Contents

1. [Introduction](#introduction)
2. [Exercise 1: MATLAB](#exercise-1-matlab)
    * [Methodology](#methodology)
    * [Question A: Down-Sampling and Envelope Computation](#question-a)
    * [Question B: Temporal Relationship Between Muscle Activation and Movement](#question-b)
3. [Exercise 2: MATLAB Simulink](#exercise-2-matlab-simulink)
    * [Case 1: Reaching Horizontal and Vertical Target Points](#case-1)
    * [Case 2: Reaching Diagonal Target Points](#case-2)
    * [Case 3: Reaching the 8 Target Points](#case-3)
    * [Further Methods](#further-methods)
4. [Conclusion](#conclusion)
5. [References](#references)
6. [Appendices](#appendices)

---

<a name="introduction"></a>

## Introduction

This repository contains the work done for the first assignment in the Biomedical Robotics course, focusing on Electromyography (EMG) signal processing and control systems using MATLAB and Simulink. The project explores the preprocessing of EMG signals and their application in controlling a cursor to reach target points in a virtual environment. The work is divided into two main exercises: signal processing using MATLAB and system simulation using Simulink.

---

<a name="exercise-1-matlab"></a>

## Exercise 1: MATLAB

This exercise focuses on the preprocessing of EMG signals, a crucial step in developing EMG-based control systems. The signals are derived from muscle activities and are processed to enhance accuracy and reliability in control applications.

<a name="methodology"></a>

### Methodology

The preprocessing of EMG signals involves the following steps:

1. **Band-Pass Filtering**: Filters the signal to retain frequencies between 30-450 Hz, removing noise and irrelevant components.
2. **Rectification**: Converts the signal to a full-wave signal by taking the absolute value.
3. **Envelope Computation**: Smooths the signal using a low-pass filter with a 5 Hz cutoff frequency.
4. **Downsampling**: Reduces the data size by a factor of 4 to improve efficiency.

<a name="question-a"></a>

### Question A: Down-Sampling and Envelope Computation

Down-sampling is performed after envelope computation because the envelope contains lower-frequency components, making it more efficient to downsample without losing critical information.

<a name="question-b"></a>

### Question B: Temporal Relationship Between Muscle Activation and Movement

To understand the temporal relationship between muscle activation and movement, synchronization of the EMG signal and motion data is required. By comparing the onset times of muscle activation and movement, the temporal dynamics of muscle control can be analyzed.

---

<a name="exercise-2-matlab-simulink"></a>

## Exercise 2: MATLAB Simulink

This exercise involves controlling a cursor in a virtual environment using EMG signals processed in Simulink. The cursor must reach target points based on the intensity of muscle activations.

<a name="case-1"></a>

### Case 1: Reaching Horizontal and Vertical Target Points

The cursor is controlled to reach horizontal and vertical targets using EMG data. The data is processed through filtering, rectification, and thresholding to trigger cursor movements.

<a name="case-2"></a>

### Case 2: Reaching Diagonal Target Points

Similar to Case 1, but the cursor's objective is to reach diagonal target points. This involves combining signals from two muscles to control the diagonal movements.

<a name="case-3"></a>

### Case 3: Reaching the 8 Target Points

The cursor is controlled to reach all 8 target points in a virtual space. A step block is used to create sudden changes in the signal to model dynamic transitions in the system.

<a name="further-methods"></a>

### Further Methods

Alternative methods for mapping EMG signals to control cursor movements, such as linear mapping to X and Y coordinates or velocity control, are discussed. These methods offer different trade-offs in terms of implementation complexity and precision.

---

<a name="conclusion"></a>

## Conclusion

This project demonstrated the use of EMG signals in controlling a virtual cursor, emphasizing the importance of signal preprocessing and the potential applications in assistive technologies. The exercises provided a practical understanding of how EMG signals can be leveraged for control purposes in biomedical robotics.

---

<a name="references"></a>

## References

1. Relevant literature and tools used in the project (e.g., MATLAB documentation, Simulink references).

---

<a name="appendices"></a>

## Appendices

Additional materials, such as code snippets, simulation results, and extended explanations, can be found in the appendices.

