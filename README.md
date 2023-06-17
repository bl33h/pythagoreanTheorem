# pythagoreanTheorem
A CUDA program that calculates the Pythagorean theorem for a large number of elements using GPU parallel processing. It initializes input arrays, launches a CUDA kernel to perform the calculations in parallel on the GPU, and verifies the results. The code demonstrates the use of CUDA for accelerated mathematical computations on the GPU.

<p align="center">
  <br>
  <img src="https://upload.wikimedia.org/wikipedia/commons/7/70/Pythagoras-2a.gif" alt="pic" width="500">
  <br>
</p>
<p align="center" >
  <a href="#Files">Files</a> •
  <a href="#Features">Features</a> •
  <a href="#how-to-use">How To Use</a> 
</p>

## Files

- src: the file that implements de solution.

## Features
The main features of the application include:
- Parallel Processing: The code utilizes CUDA to perform calculations in parallel on the GPU, taking advantage of its parallel architecture to accelerate the computation of the Pythagorean theorem for a large number of elements.
- Memory Management: The code manages memory allocation and transfer between the host (CPU) and the device (GPU) using CUDA functions like cudaMalloc, cudaMemcpy, and cudaFree.
- Random Initialization: The code initializes input arrays with random values using the rand() function, providing variability to the input data.
- Error Handling: The code includes error handling mechanisms using cudaError_t and cudaGetErrorString to detect and report any errors that may occur during CUDA function calls.
- Result Verification: After the computation is performed on the GPU, the code verifies the correctness of the results by comparing them against the expected values, ensuring the accuracy of the Pythagorean theorem calculations.
- Performance Measurement: The code displays information about the number of blocks and threads used in the CUDA kernel launch, providing insights into the GPU's computational workload.
- Device Reset: The code calls cudaDeviceReset to deinitialize the GPU device after the computation is complete, ensuring proper cleanup and freeing of resources.

## How To Use
To clone and run this application, you'll need [Git](https://git-scm.com) installed on your computer. From your command line:

...
```bash
# Clone this repository
$ git clone https://github.com/bl33h/pythagoreanTheorem

# Open the folder
$ cd src

# Build the code
$ make

# Run the app
$ ./pythagoreanTheorem
```

Alternatively, you can run the code using Google Colab:
1. [Open Google Colab](https://colab.research.google.com) in your web browser.
2. Click on "File" in the top menu, then select "Open notebook".
3. In the "GitHub" tab, enter the repository URL: https://github.com/bl33h/pythagoreanTheorem
4. Choose the desired notebook file and click "Open".
5. Follow the instructions within the Colab notebook to execute the code.

Note: Running the code in Google Colab requires an internet connection and a Google account. It provides a convenient online environment for executing code without the need for local setup or dependencies.
