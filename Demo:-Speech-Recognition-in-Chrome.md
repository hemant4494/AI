* Name: SpeechRecognition
* Subject Area: speech recognition
* Type: in-browser demo software (Google Chrome only)
* Grade(s): all ages
* URL: [https://www.cs.cmu.edu/~dst/SpeechRecognition](https://www.cs.cmu.edu/~dst/SpeechRecognition)
* Creators: Dave Touretzky and Sarah Pam
* License: public domain

Description: this demo uses the Google Speech API to record audio from the computer's microphone and return strings indicating the best hypotheses for what the speaker said. These hypotheses are displayed in rank order, highest score first. There will usually be more than one hypothesis, and sometimes none of them are correct. The demo illustrates the current state of the art in speech recognition, including its limitations.

Note: this demo only works in Google Chrome because other browsers do not yet implement in-browser speech recognition. Also, the machine must have a microphone, and a working network connection in order to access the Google Speech recognition service.

Some things to demonstrate:
* Longer utterances usually work better than one or two word utterances.
* Grammatical utterances are recognized much more easily than random strings of words.
* Careful enunciation improves the recognition rate.
