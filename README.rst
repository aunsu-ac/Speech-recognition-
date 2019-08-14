**REQUIREMENTS**
Python 2.6, 2.7, or 3.3+ (required)
PyAudio 0.2.11+ (required only if you need to use microphone input, Microphone)
Google API Client Library for Python (required only if you need to use the Google Cloud Speech API, recognizer_instance.recognize_google_cloud)
another requirements
On Python 2, and only on Python 2, some functions (like recognizer_instance.recognize_bing) will run slower if you do not have Monotonic for Python 2 installed.

**PYTHON** :
The first software requirement is Python 2.6, 2.7, or Python 3.3+. This is required to use the library.

**PYAUDIO**:


PyAudio is required if and only if you want to use microphone input (Microphone). PyAudio version 0.2.11+ is required, as earlier versions have known memory management bugs when recording from microphones in certain situations.

If not installed, everything in the library will still work, except attempting to instantiate a Microphone object will raise an AttributeError.

The installation instructions on the PyAudio website are quite good - for convenience, they are summarized below:


1. On Windows, install PyAudio using Pip: execute pip install pyaudio in a terminal.
2. On OS X, install PortAudio using Homebrew: brew install portaudio. Then, install PyAudio using Pip: pip install pyaudio.
3.PyAudio wheel packages[https://pypi.org/project/wheel/] for common 64-bit Python versions on Windows and Linux are included for convenience, under the third-party/ directory in the repository root. To install, simply run pip install wheel followed by pip install ./third-party/WHEEL_FILENAME (replace pip with pip3 if using Python 3) in the repository root directory.


**Google Cloud Speech Library for Python (for Google Cloud Speech API users)**:


Google Cloud Speech library for Python is required if and only if you want to use the Google Cloud Speech API (recognizer_instance.recognize_google_cloud).

If not installed, everything in the library will still work, except calling recognizer_instance.recognize_google_cloud will raise an RequestError.

According to the official installation instructions, the recommended way to install this is using Pip: execute pip install google-cloud-speech (replace pip with pip3 if using Python 3).



