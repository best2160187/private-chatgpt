# private-chatgpt
This page describes how to interact with the Llama 2 large language model (LLM) locally using Python, without requiring internet, registration, or API keys. We will deliver prompts to the model and get AI-generated chat responses using the llama-cpp-python package.

Step 1: Download a Large Language Model
The Llama 2 model can be downloaded in GGML format from Hugging Face:

Model I’m using: llama-2-7b-chat.ggmlv3.q8_0.bin (7 GB)

All models: Llama-2-7B-Chat-GGML/tree/main

Model descriptions: Readme

The model I’m using here is the largest and slowest one currently available. It is 7 GB in size and requires 10 GB of ram to run. Developers should experiment with different models, as simpler models may run faster and produce similar results for less complex tasks.

Step 2: Prepare the Python Environment
Install the latest version of Python from python.org

Create a virtual environment: python -m venv .venv

Activate the virtual environment: .venv/Scripts/activate

Install the llama-cpp-python package: pip install llama-cpp-python

Installation will fail if a C++ compiler cannot be located. To get one:

Windows: Install Visual Studio Community with the “Desktop development with C++” workload. It is free for individuals an open-source developers. See the C++ installation guide for more information.

Linux: apt install python3-dev

MacOS: brew install python3-dev
