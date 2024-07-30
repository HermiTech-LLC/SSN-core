# **SSN-Core: Sensor and Servo Network Core Framework**

## **Overview**
The **SSN-Core** framework provides a robust and flexible foundation for developing applications that involve sensor data processing, natural language understanding (NLU), text-to-speech (TTS) capabilities, and servo control. This framework is designed for developers looking to create complex systems with integrated sensor and servo operations, alongside advanced NLU and TTS functionalities.

___

![img](https://github.com/HermiTech-LLC/SSN-core/blob/main/ssn-c.png)
___

## **Installation**

1. **Clone the repository:**
   ```sh
   git clone https://github.com/LoQiseaking69/SSN-core.git
   cd SSN-core
   ```

2. **Install required dependencies:**
   Ensure you have Python 3.8+ installed. Then, install the necessary Python packages:
   ```sh
   pip install -r requirements.txt
   ```

## **Usage**

1. **Configuration:**
   Configure the necessary settings in `core_framework.py`, `nlu_tts_modules.py`, and `servo_control_module.py` as per your application requirements.

2. **Running the application:**
   Execute the main script to start the application:
   ```sh
   python main.py
   ```

## **Files Description**

- **core_framework.py:** Contains the core functionalities and classes required for initializing and managing the sensor and servo network. This file is the backbone of the framework, ensuring smooth communication between different modules.

- **nlu_tts_modules.py:** Includes the modules responsible for natural language understanding and text-to-speech. This file contains methods for processing user input, understanding commands, and generating speech output.

- **servo_control_module.py:** Manages the control of servos. It provides functions to initialize servos, send control signals, and manage their states.

- **main.py:** The entry point of the application. This file integrates all modules and starts the execution of the framework.

## **Example**

The main script initializes the Multimodal SNN, sets the modules, trains the network, and handles various inputs:

1. **Sentiment Analysis**:
    ```python
    sentiment_result = snn.handle_input('nlu', 'Hello, how are you?', task='sentiment')
    ```

2. **Question Answering**:
    ```python
    qa_result = snn.handle_input('nlu', text='Who is the president of the United States?', task='qa', context='Joe Biden is the president of the United States.')
    ```

3. **Text-to-Speech**:
    ```python
    audio_data = snn.handle_input('tts', 'This is a test.', lang='en', slow=False)
    ```

4. **Servo Control**:
    ```python
    servo_response = snn.handle_input('servo', {'servo_1': 90, 'servo_2': 45})
    ```

## **License**

This project is licensed under the BSD 3-Clause License. See the LICENSE file for more details.
