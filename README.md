# Signal Processing Project

## About
This project involves signal processing tasks such as denoising and deblurring using Fourier transforms and convolution techniques. It explores methods to enhance signal clarity and recover original data from noisy or blurred signals.

## Problem Statement
The project aims to address two primary challenges:
1. **Denoising Signal y[n]**: Implementing a denoising function to remove noise from the original signal y[n] using convolution with a defined array.
2. **Deblurring Signal y[n]**: Applying deblurring techniques by dividing the Fourier transform of y[n] with that of an impulse response, followed by inverse Fourier transform to recover the signal.

## Implementation Details
- **Data Retrieval**: Signals are retrieved from an Excel file containing x[n] and y[n].
- **Functions**:
  - `hn(n)`: Defines the impulse response function.
  - `dtft_of_hn()`: Computes the Discrete-Time Fourier Transform (DTFT) of the impulse response.
  - `dtft(signal, array)`: Computes DTFT of any given signal.
  - `ift(signal, array)`: Computes the Inverse Fourier Transform (IFT) of a signal.
  - `denoise(signal)`: Denoises a signal using convolution with a predefined array.
- **Signal Processing**:
  - Denoises y[n] and plots the denoised signal.
  - Deblurs y[n] using Fourier transforms and recovers the signal.
- **Error Calculation**: Optionally calculates and visualizes the error between the original and recovered signals.

## Instructions for Use
1. Ensure Python and necessary libraries (Pandas, NumPy, Matplotlib) are installed.
2. Update `excel_file` variable to point to your data file.
3. Run each section of the script sequentially to perform denoising and deblurring operations.
4. Uncomment plotting sections to visualize denoised and recovered signals, and error calculations.

## Results
- The project outputs denoised and recovered signals, demonstrating the effectiveness of the implemented signal processing techniques.

