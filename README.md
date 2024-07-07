### Phi-3-mini-4k-instruct finetuning

This repo is using https://github.com/Azure/azureml-examples/tree/main/sdk/python/foundation-models/system/finetune/chat-completion as baseline.

Notes:
- Fine tunned model: Phi-3-mini-4k-instruct
- Fine tuning and inferencing has been done on Standard_NC24ads_A100_v4
- Tested with Python 3.12.4

Python libraries:
- Instead of using datasets==2.9.0, I am using datasets
  - v2.9.0 resulted in error visible in Notebook
  - After swapping v2.9.0 for latest version, I was able to run download-dataset.py
- I have created requirements_pip_freeze.txt that shows all libraries & versions
- Used requirements.txt instead of running Notebook cell with pip installs

Environment variables:
- Used .env to store all environment variables
- .env.example shows what environment variables are required. Rename it to .env and substitute values relevant to your environment
