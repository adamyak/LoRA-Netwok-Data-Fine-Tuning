
```markdown
# LoRA-Netwok-Data-Fine-Tuning

Train the **TinyLlama-1.1B-Chat-v1.0** model for analyzing IoT network logs using Low-Rank Adaptation (LoRA).

## Overview

This project focuses on fine-tuning the `TinyLlama-1.1B-Chat-v1.0` model to classify and analyze network traffic logs from IoT devices. The aim is to detect anomalies and perform intrusion detection by leveraging machine learning techniques tailored for natural language processing tasks.

## Data Used

The dataset used for this project is sourced from [Kaggle](https://www.kaggle.com/datasets/speedwall10/iot-device-network-logs/data).
It has been preprocessed specifically for the task of network-based intrusion detection in IoT environments.

### Dataset Classes

0: "Normal traffic between IoT devices.",
1: "Misconfiguration detected. Possibly a device sending out-of-spec data.",
2: "DDoS attack detected. High volume of traffic to a specific target.",
3: "Data type probing. Strange payloads (e.g., strings) sent to devices expecting specific types.",
4: "Network scan identified. The source is likely scanning for active devices or open ports.",
5: "Man-in-the-Middle attack detected. Suspicious interception between source and destination."
```
## Environment Setup

To set up a Python virtual environment for the project, follow these steps:

1. **Create a Virtual Environment:**

   ```bash
   python3 -m venv my_ntk_finetuning_env
   ```

2. **Activate the Virtual Environment:**

   ```bash
   source my_ntk_finetuning_env/bin/activate
   ```

3. **Deactivate the Virtual Environment:**

   To exit the environment, simply run:

   ```bash
   deactivate
   ```

## Training Configuration

- The model is configured to utilize Apple's MPS (Metal Performance Shaders) for efficient computation on Apple Silicon.
- Training relies on LoRA (Low-Rank Adaptation) to perform parameter-efficient fine-tuning.

## Project Goals

- **Achieve effective anomaly detection** in IoT device logs.
- **Optimize training performance** using device-specific accelerations.

## Contact

For questions or collaboration, feel free to reach out or submit issues and pull requests to contribute to the project.

