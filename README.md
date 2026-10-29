# JARVIS AI Assistant — Custom Enhancements

This package contains modifications to D3v0ps/JARVIS.

## Features

- GPT-OSS 120B Cloud as the primary AI model
- Automatic fallback to local Qwen3:4B
- Automatic cloud retry after 60 seconds
- Windows GUI and voice interaction
- File management and application control
- Website creation through available tools

## Requirements

- Windows 10/11
- Python 3.13
- Git
- Ollama
- Microphone and speakers
- Internet access for cloud AI

## Installation

1. Clone the original project:

   git clone https://github.com/D3v0ps/JARVIS.git
   cd JARVIS

2. Check out the tested base commit:

   git checkout b747b0041ea8d0025699b7c7de89ff27a7cdb897

3. Download the files from this enhancement package.

4. Apply the patch from the JARVIS project folder:

   git apply --check path\to\jarvis-changes.patch
   git apply path\to\jarvis-changes.patch

5. Copy config.example.yaml into the JARVIS folder and rename the copy to config.yaml.

6. Create a Python virtual environment:

   py -3.13 -m venv .venv

7. Install dependencies:

   .\.venv\Scripts\python.exe -m pip install -r requirements-cpu.txt

   Additional dependencies or model assets may be required by the original project.

8. Install Ollama and download the local model:

   ollama pull qwen3:4b

9. Sign in to Ollama Cloud with your own account and confirm access to gpt-oss:120b-cloud.

10. Launch JARVIS:

    .\.venv\Scripts\python.exe -m jarvis --window

## Notes

- The original JARVIS source code is not included in this enhancement package.
- Each user must configure their own Ollama Cloud access.
- Model assets and voice files are not included.
- Some hardware-specific settings may require adjustment.
- Only the patch application has been verified on a clean checkout; a complete fresh installation has not yet been tested.

## Credits

Original project: https://github.com/D3v0ps/JARVIS

Enhancements: https://github.com/wajahat59-code/JARVIS-AI-Assistant

This package does not claim ownership of the original project.
