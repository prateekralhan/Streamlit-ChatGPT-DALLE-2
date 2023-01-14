# ✨ Streamlit based ChatGPT/DALLE-2 [![Project Status: Active](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active) [![](https://img.shields.io/badge/Prateek-Ralhan-brightgreen.svg?colorB=ff0000)](https://prateekralhan.github.io/)
A simple streamlit based webapp using OpenAI APIs empowered with text generation and image generation functionalities

![demo_txt](https://user-images.githubusercontent.com/29462447/212479457-f3a11c26-f889-4f33-9569-ea154c95f091.gif)

![demo_img](https://user-images.githubusercontent.com/29462447/212479452-3d59ed7b-cbc3-43f1-bdb9-5e9d3b37dadc.gif)

## Installation:
* Simply run the command ***pip install -r requirements.txt*** to install the dependencies.

## Usage:
1. Clone this repository and install the dependencies as mentioned above.
2. Navigate to the [OpenAI API section](https://beta.openai.com/account/api-keys) to login and generate your API Key. Ensure you save this API Key as **"OpenAI_API_Key"*** in the form of a system environment variable which shall be used by the webapp. ***( I am only using the Free Trial version which provides 18$ of credits. )***
2. Simply run the command: 
```
streamlit run app.py
```
3. Navigate to http://localhost:8501 in your web-browser.


## Results:

![1](https://user-images.githubusercontent.com/29462447/212479438-b2774381-122c-40b3-8380-5a7fa1336483.png)

![2](https://user-images.githubusercontent.com/29462447/212479439-6e6ce078-e61b-4430-9eba-0931b1b199d5.png)

### Running the Dockerized App
1. Ensure you have Docker Installed and Setup in your OS (Windows/Mac/Linux). For detailed Instructions, please refer [this.](https://docs.docker.com/engine/install/)
2. Navigate to the folder where you have cloned this repository ( where the ***Dockerfile*** is present ).
3. Build the Docker Image (don't forget the dot!! :smile: ): 
```
docker build -f Dockerfile -t app:latest .
```
4. Run the docker:
```
docker run -p 8501:8501 app:latest
```

This will launch the dockerized app. Navigate to ***http://localhost:8501/*** in your browser to have a look at your application. You can check the status of your all available running dockers by:
```
docker ps
```
