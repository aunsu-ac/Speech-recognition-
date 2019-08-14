**Requirements**
Python 2.6, 2.7, or 3.3+ (required)
PyAudio 0.2.11+ (required only if you need to use microphone input, Microphone)
Google API Client Library for Python (required only if you need to use the Google Cloud Speech API, recognizer_instance.recognize_google_cloud)
another requirements
On Python 2, and only on Python 2, some functions (like recognizer_instance.recognize_bing) will run slower if you do not have Monotonic for Python 2 installed.

**PYTHON** :
The first software requirement is Python 2.6, 2.7, or Python 3.3+. This is required to use the library.

**Pyaudio**
PyAudio is required if and only if you want to use microphone input (Microphone). PyAudio version 0.2.11+ is required, as earlier versions have known memory management bugs when recording from microphones in certain situations.

If not installed, everything in the library will still work, except attempting to instantiate a Microphone object will raise an AttributeError.

The installation instructions on the PyAudio website are quite good - for convenience, they are summarized below:

1. On Windows, install PyAudio using Pip: execute pip install pyaudio in a terminal.



