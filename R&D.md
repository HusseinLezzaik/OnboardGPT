## Approahces
1. Finetuning OpenAssistant without messing it:
- it might not work for part of it
- maybe you just need some part of the neural network to fine tune. To do so you need to freeze weights, load GPT2, set grad to false, format data by scraping data from the web, autmate RLHF)

2. Finetung something like codex:
- first finetuning on your codebase, docs, internal tools
- make it a chatbot using RLHF
- might be able to use chatgpt itself to collect a dataset to finetune on

## Notes
- codeGen from Salesforce seemed working, after making it faster
- training from scratch after shipping something finetuned: collected data, knew what users want, etc
- they're using 2.8B param, sweet spot
- maybe do something close to the way ChatGPT for Robotics, instead just create a library that ChatGPT can use to write code or like ToolFormer