* Name: SpeechRecognition
* Subject Area: speech recognition
* Type: in-browser demo software (Google Chrome only)
* Grade(s): all ages
* URL: [https://www.cs.cmu.edu/~dst/SpeechDemo](https://www.cs.cmu.edu/~dst/SpeechDemo)
* Creators: Dave Touretzky and Sarah Pam
* License: public domain

Description: this demo uses the Google Speech API to record audio from the computer's microphone and return strings indicating the best hypotheses for what the speaker said. These hypotheses are displayed in rank order, highest score first. There will usually be more than one hypothesis, and sometimes none of them are correct. The demo illustrates the current state of the art in speech recognition, including its limitations.

Note: this demo only works in Google Chrome because other browsers do not yet implement in-browser speech recognition. Also, the machine must have a microphone, and a working network connection in order to access the Google Speech recognition service.

Some things to consider:
* Longer utterances usually work better than one or two word utterances.
* Grammatical utterances are recognized much more easily than random strings of words.
* Careful enunciation improves the recognition rate.

Experiments you can try:
* Speaking a single word such as "break" or "night" or "led" will display all the homophones Google knows that match it.
* Homophones such as "which"/"witch" can often be disambiguated by context.  Try [these examples](https://examples.yourdictionary.com/examples-of-homophones.html) at yourdictionary.com.
* Common mispronunciations (or dialectical variants) may be corrected automatically to Standard American English. Try these examples:
* * _"Let me **ax** you a question."_
* * _"I love fruit, **exspecially** bananas."_
* * _"My hamster **exscaped** from his cage and is hiding under the bed."_
* Non-words can sometimes be corrected based on context. Try these examples, where the non-word 'brapes' is best interpreted as either 'grapes' or 'drapes' depending on the context:
* * _"Start your fruit salad by cutting up the **b**rapes"_
* * _"Brighten the room by drawing back the **b**rapes"_
* Common sayings are recognized as a whole, not word by word. Compare these examples:
* * _"Able was I ere I saw Elba"_ (a well known palindrome; Google recognizes it)
* * _"Able were you ere you saw Elba"_ (not a palindrome and not well known; Google has trouble with this one)
* Why does Google have problems with _"Able were you ere you saw Elba"_? Two reasons:
* * The syntax is unusual and slightly awkward.
* * The word "ere", which means "before", is archaic and not used in modern conversational English, so Google does its best to interpret this sound as some more common word, such as "ear", unless the context strongly points to "ere".
* Try this quote from _The Hobbit_. Does Google get it? Do you think Google's training corpus might include famous literature?
* * _"we must away, ere break of day"_
* Google tries really hard to hear famous quotes correctly. Try this example:
* * _"No man is an island"_ (John Donne, Meditation XVII)
* * _"No man is an eyelid"_ (unlikely to be in Google's training data)
* Sometimes the bias is so strong that Google refuses to recognize what you actually said:
* * _"Four blind mites"_ can be recognized with careful enunciation.
* * _"Three blind mites"_ cannot be recognized; Google always hears "Three blind mice" which matches the children's rhyme.
* Try the English word "Kalamazoo". Then switch the language model from English to Spanish and try "Kalamazoo" again.
* Switch the language model from English to Spanish and try speaking English to the Spanish model. It actually works pretty well. Now try switching the language model to Mandarin and try speaking English to that model.

Also see this Google demo page: [https://www.google.com/intl/en/chrome/demos/speech.html](https://www.google.com/intl/en/chrome/demos/speech.html)
