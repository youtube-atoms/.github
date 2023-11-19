# Welcome to the Youtube Atoms Project 

## 🙋‍♀️ A short introduction - what is your organization all about?
Du'an Lightfoot inspired us with his amazing [Youtube Analysis Assistant](https://github.com/labeveryday/youtube-analysis-assistant): it works, and is really well done, so use that. 

This might be good some day, too.

## Anatomy of the System 

In order to acheive anythign close to the success of Du'an's project, we need access to:

 * voice to speach (transcription)
 * generative AI chat
 * image generation

The [`youtube-assistant-client`](https://github.com/youtube-assistant-client) provides a simple autoconfigured client that supports those three usecases. 

For transcription, we integrated [Whisper AI](https://openai.com/research/whisper). Whisper AI is an opensource Python-based AI from OpenAI to support Transcription. It's been caged and containerized in a small Python-based  microservice called [`whisper-transcription-service`](https://github.com/youtube-atoms/whisper-transcription-service) that's accessible from RabbitMQ. Use the `youtube-assistant-client`'s `YaAiClient` to talk to it via the `YaAiClient#transcribe(Resource audioFile)`  method. 

<!--

**Here are some ideas to get you started:**


🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
