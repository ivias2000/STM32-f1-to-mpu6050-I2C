# STM32-f1-to-mpu6050-I2C
How to connect STM32F103 to MPU6050 with I2C![download](https://github.com/ivias2000/STM32-f1-to-mpu6050-I2C/assets/125237611/842e1c80-b28b-4827-968c-5114d3bd5528)

This C code appears to be a template for a main program file targeting a microcontroller, likely an STM32 microcontroller, and using the MPU6050 accelerometer and gyroscope sensor. Let me explain the key components of the code:

Includes:
The code includes various header files representing different libraries used in the project. These headers provide access to functions and constants required for the peripherals and libraries used in the application.

Main Function:![Screenshot 2023-07-18 111147](https://github.com/ivias2000/STM32-f1-to-mpu6050-I2C/assets/125237611/32dc4743-80df-4520-8eeb-c054f1d49291)


The main function is the entry point of the program, where the microcontroller's peripherals and the MPU6050 sensor are initialized. The MPU6050 sensor readings are continuously read in a loop, and a delay of 100 milliseconds is added between each reading.

System Clock Configuration:
The function SystemClock_Config configures the system clock for the microcontroller. It initializes the oscillator, PLL (Phase-Locked Loop), and clock dividers to achieve the desired clock frequency.

Error Handling:
The Error_Handler function is a basic error handling routine, which is called in case of an error. In this implementation, it disables interrupts and enters an infinite loop, effectively halting the program.
![Screenshot 2023-07-18 110701](https://github.com/ivias2000/STM32-f1-to-mpu6050-I2C/assets/125237611/b8417a8e-2765-4199-aac7-909819c26124)
Assert Failed:
The assert_failed function is used when assertions are enabled (USE_FULL_ASSERT is defined). If an assertion fails, this function will be called to handle the error. In this implementation, it does not have any specific error handling and is left for the user to customize as needed.

To use this code on GitHub, follow the steps mentioned earlier to create a new repository and upload this C code as the main program file. Additionally, you may want to include a README.md file in your repository, providing a brief description of the project, instructions on how to set up the development environment, and how to use the code. This will make it easier for others to understand and work with your code.
