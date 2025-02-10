## YaGPT chatbot supporting user context 

### Summary
This YaGPT bot runs on the following components:
- [Yandex GPT](https://cloud.yandex.ru/services/yandexgpt)
- [Yandex GPT for Langchain](https://python.langchain.com/docs/integrations/chat/yandex)
- [Streamlit](https://streamlit.io/)
- [LangChain](https://python.langchain.com/)

### Repository structure and how to use the bot
- The ``.env`` file contains system variables (you can specify them as `secrets` when running in the cloud):
```
YAGPT_FOLDER_ID = 
YAGPT_API_KEY = 
```
- `requirements.txt` traditionally contains the list of dependencies to install using this command: 
```pip install -r requirements.txt ```
- The `images` folder stores the company logo to use in the `streamlit` GUI.
- `yagpt-chat-with-history-01.py`: File to run in `streamlit run yagpt-chat-with-history-01.py`. Adapted to run on local server or PC, requires filling in the `.env` file
- `yagpt-chat-with-history-02.py`: File to run. Adapted to run in [Streamlit Community Cloud](https://docs.streamlit.io/streamlit-community-cloud/get-started). Requires setting the system variables in `streamlit secrets` when deploying the application.
- `yagpt-chat-with-history-03.py`: File to run. Adapted to run in [Streamlit Community Cloud](https://docs.streamlit.io/streamlit-community-cloud/get-started). Does not require setting the system variables in `streamlit secrets` when deploying the application. You can set the system variables (see above) directly from the app web interface.

### Running in Streamlit Community Cloud
Follow [this guide](https://docs.streamlit.io/streamlit-community-cloud/get-started) to deploy this app using Streamlit Community Cloud.

