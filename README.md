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

3. Adding new model (Click `Models` on left menu) and then click `+ Add Model` button  
> [!TIP]
> [Models](https://docs.gpt4all.io/gpt4all_desktop/models.html)

![add_model](https://github.com/AshleyDhevalall/gpt4all-demo/blob/main/docs/add_model_1.png)

4. Search for `Llama 3.2 1B Instruct` and then click `Download`. Please patient while to model downloads...

![explore_models](https://github.com/AshleyDhevalall/gpt4all-demo/blob/main/docs/explore_models.png)

5. Clone repository
```
git clone https://github.com/AshleyDhevalall/gpt4all-demo.git
```

6. Configure settings
> [!TIP]
> [Settings](https://docs.gpt4all.io/gpt4all_desktop/settings.html)

7.1 Click `LocalDocs` on left menu. Provide a `Collection name` eg. `Sample Test`
> [!TIP]
> [LocalDocs](https://docs.gpt4all.io/gpt4all_desktop/localdocs.html)  

<img src="https://github.com/AshleyDhevalall/gpt4all-demo/blob/main/docs/add_document_collection.png" style='height: 70%; width: 70%;'>

7.2 Click `Browse`. Navigate to cloned repository folder above (Step 5) and then select the folder. Please patient while the embeddings complete...  

<img src="https://github.com/AshleyDhevalall/gpt4all-demo/blob/main/docs/embeddings.png" style='height: 70%; width: 70%;'>

8. Click `New chat` on left menu. Ensure you select the files from the `Local Docs` panel on the right side  
  
    Enter your prompt and click `Send`
```
what passwords are used?
```
> [!TIP]
> [Chat](https://docs.gpt4all.io/gpt4all_desktop/chats.html)

Sample chat response  
![chat](https://github.com/AshleyDhevalall/gpt4all-demo/blob/main/docs/chat.png)

> [!IMPORTANT]  
> Always verify the accuracy of the results  
> GTP4All has an option that allows you to view the source of the files in the Chat response

## Troubleshooting
#### Embedding taking too long
Uploading large files will result in an increased duration for the embedding to complete. Alternatively try a smaller subset of docs

#### Load Docs collection shows 0 files and 0 words

<img src="https://github.com/AshleyDhevalall/gpt4all-demo/blob/main/docs/troubleshooting.png" style='height: 70%; width: 70%;'>

Ensure that you have included the correct file extension
![allowed_file_extensions](https://github.com/AshleyDhevalall/gpt4all-demo/blob/main/docs/allowed_file_extensions.png)

> [!TIP]
> [Allowed File Extensions](https://github.com/nomic-ai/gpt4all/wiki/LocalDocs)

#### Chat window closes after selecting model -> try using a smaller model
This usually happens when using models that required more RAM than is available on your system. Try using a smaller model

<img src="https://github.com/AshleyDhevalall/gpt4all-demo/blob/main/docs/ram_required.png" style='height: 70%; width: 70%;'>

## Further reading  
[Docs](https://lmstudio.ai/docs)  
[Download Models](https://lmstudio.ai/docs/basics/download-model)  
[Chat](https://lmstudio.ai/docs/basics/chat)

## Authors

[Ashley Dhevalall](https://github.com/AshleyDhevalall)

## Acknowledgements

[lmstudio](<https://lmstudio.ai/>)  
[Joshua Stenhouse](<https://virtuallysober.com/2017/07/10/working-with-sql-databases-using-powershell/>)

