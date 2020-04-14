# Welcome to Voice User Interface!

- A VUI is a speech platform that enables humans to communicate with machine by voice.
- VUI used to be the stuff of science fiction.
  - These there parts constitute a general pipeline for building an end to end voice enabled application. Each part employs some aspects of AI.
    1. Audio sound waves from voice must be converted into language texts using machine learning algorithms and probabilistic models.
    2. The resulting text must be reasoned-over using AI logic to determine the meaning and formulate a response.
    3. Finally, the response text must be converted back into understandable speech again with machine learning tools.

---

- VUI Overview
- ![VUI Stages](/img/vui_overview.png)
  - voice to text: speech recognition,
    1. as person speaks into a microphone, sound vibrations are converted to an audio signal. This signal can be sampled at some rate and converted into vectors of component frequencies, these vectors represent features of sound in a data set. so this step is feature extraction.
    2. next step is to decode or recognize the series of vectors as a word or a sentence. Do that by **probabilistic models** that work well with time series data for the sound pattern which is the **acoustic model**.
    3. decoding a vector with an acoustic model will give us a best guess as to what the words are. but that not enough the could not recognize 'hello world' or 'how a word' not like us! We have **Language** model in our brains trained from years of experience and that sth we need to add to our decoder.
    4. An **accent model** may be needed for the same reason.
    5. if these models are well trained on lots of representative examples, we have a higher probability of producing the correct text
  - ![speech recog models](/img/sr_models.png)
  - **Probabilistic Models**:
    1. We built **Hidden Markov Models (HMMs)** to decode a series of gestures.
    2. We used **Recurrent Neural Networks (RNNs)** to train time series data.
  - both of these models have been used successfully in speech recognition.
  - Once we have speech in form of text, it's time to do the thinking part
  ***
  - text input reasoned to text output: thinking part of our voice application, the reasoning logic.
  - [reasoning logic example](/img/rlogic_ex.png)
  ***
  - Once we have a text response, remaining task is to convert that text to speech. this is the speech synthesis or text to speech (TTS).

---

- VUI Application
  - Can be found on cars!
  - Dictation application
  - Translation application
  - Conversational AI technology
    - Apple's Siri
    - Microsoft Cortana
    - Google Home
    - Amazon Alexa on Eco
