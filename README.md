## RachelChat
Rachel is a voice assistant chatbot that can be configured to speak different languages using ChatGPT, OpenAI and ElevenLabs AI. This project is created with React and Python FastAPI where API keys are added from different user accounts.
### Frontend 
- React js and Tailwindcss
### Backend
Steps used to create API routes
- Save an audio input `online-voice-recorder.com`
- Convert audio to text `OpenAI Whisper`.
- Get chatbot response from `OpenAI ChatGPT`
- Add chat to history
- Covert text to speech `ElevenLabs AI`
#### Dependencies 
NOTE: Run the packages in a virtual environment.
- python3 -m venv NAME_OF_YOUR_ENVIRONMENT
- Activate the environment: for mac `source venv/bin/activate` and windows `venv/Script/activate`.
- Install this in your environment `pip3 install -r requirements.txt`.
```
pip3 install openai==0.27.0
pip3 install python-decouple==3.8
pip3 install python-multipart==0.0.6 
pip3 install requests==2.28.2 
pip3 install fastapi==0.92.0
pip3 install "uvicorn[standard]"

```
- Running the backend `uvicorn main:app --reload` for development and production `uvicorn main:app`