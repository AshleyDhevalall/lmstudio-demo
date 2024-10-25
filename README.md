# lmstudio-demo
The objective of this article is to run large language models locally to analyze local docs. In this use case we analyze powershell scripts that make use of a sql server.

## What is LM Studio?
LM Studio is a desktop app for developing and experimenting with LLMs on your computer.

Key functionality

- A desktop application for running local LLMs  
- A familiar chat interface  
- Search & download functionality (via Hugging Face 🤗)  
- A local server that can listen on OpenAI-like endpoints  
- Systems for managing local models and configurations  

## Steps to follow

1. Download [LM Studio](https://lmstudio.ai/)
> [!TIP]
> [QuickStart](https://lmstudio.ai/docs/basics#1-download-an-llm-to-your-computer)  

2. Open LM Studio. Please patient while the application opens...  
![lmstudio](https://github.com/AshleyDhevalall/lmstudio-demo/blob/main/docs/lmstudio.png)

3. Download model (Click `My Models` on left menu). Ensure you have selected 'Developer' as the role
You can search for models by keyword (e.g. llama, gemma, lmstudio), or by providing a specific user/model string.  
You can even insert full Hugging Face URLs into the search bar!. Please patient while to model downloads...  
> [!TIP]
> [Download Models](https://lmstudio.ai/docs/basics/download-model)

![download](https://github.com/AshleyDhevalall/lmstudio-demo/blob/main/docs/download.png)

4. Clone repository
```
git clone https://github.com/AshleyDhevalall/lmstudio-demo.git
```

5. Click `Chat` on left menu
> [!TIP]
> [Managing chats](https://lmstudio.ai/docs/basics/chat)
  
Select model
![select-model](https://github.com/AshleyDhevalall/lmstudio-demo/blob/main/docs/select_model.png)

6. Navigate to the folder you cloned in Step 4 and select the `src\UsingSQLWithPowerShellExamplesv1.ps1` file

7. Enter your prompt and click `Send`
```
what passwords are used?
```

Sample chat response  
![chat_response](https://github.com/AshleyDhevalall/lmstudio-demo/blob/main/docs/chat_response.png)

> [!IMPORTANT]  
> Always verify the accuracy of the results

## Further reading  
[Docs](https://lmstudio.ai/docs)  
[Download Models](https://lmstudio.ai/docs/basics/download-model)  
[Chat](https://lmstudio.ai/docs/basics/chat)  
[Chat with Documents](https://lmstudio.ai/docs/basics/rag)

## Authors

[Ashley Dhevalall](https://github.com/AshleyDhevalall)

## Acknowledgements

[lmstudio](<https://lmstudio.ai/>)  
[Joshua Stenhouse](<https://virtuallysober.com/2017/07/10/working-with-sql-databases-using-powershell/>)

