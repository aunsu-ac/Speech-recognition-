Requirements
------------

To use all of the functionality of the library, you should have:

* **Python** 2.6, 2.7, or 3.3+ (required)
* **PyAudio** 0.2.11+ (required only if you need to use microphone input, ``Microphone``)
* **PocketSphinx** (required only if you need to use the Sphinx recognizer, ``recognizer_instance.recognize_sphinx``)
* **Google API Client Library for Python** (required only if you need to use the Google Cloud Speech API, ``recognizer_instance.recognize_google_cloud``)   
Installing
----------

First, make sure you have all the requirements listed in the "Requirements" section. 

The easiest way to install this is using ``pip install SpeechRecognition``. 


**Quickstart:** ``pip install SpeechRecognition``. See the "Installing" section for more details.

To quickly try it out, run ``python -m speech_recognition`` after installing.

Project links:

-  `PyPI <https://pypi.python.org/pypi/SpeechRecognition/>`__


PYTHON
------

The first software requirement is Python 2.6, 2.7, or Python 3.3+. This is required to use the library.

PYAUDIO
-------


PyAudio is required if and only if you want to use microphone input (Microphone). PyAudio version 0.2.11+ is required, as earlier versions have known memory management bugs when recording from microphones in certain situations.

If not installed, everything in the library will still work, except attempting to instantiate a Microphone object will raise an AttributeError.

The installation instructions on the PyAudio website are quite good - for convenience, they are summarized below:


1. On Windows, install PyAudio using Pip: execute pip install pyaudio in a terminal.

2. On OS X, install PortAudio using Homebrew: brew install portaudio. Then, install PyAudio using Pip: pip install pyaudio.

3.PyAudio `wheel packages <https://pypi.python.org/pypi/wheel>`__ for common 64-bit Python versions on Windows and Linux are included for convenience, under the ``third-party/`` `directory <https://github.com/Uberi/speech_recognition/tree/master/third-party>`__ in the repository root. To install, simply run ``pip install wheel`` followed by ``pip install ./third-party/WHEEL_FILENAME`` (replace ``pip`` with ``pip3`` if using Python 3) in the repository `root directory

Google Cloud Speech Library for Python (for Google Cloud Speech API users)
--------------------------------------------------------------------------


Google Cloud Speech Library for Python (for Google Cloud Speech API users)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

`Google Cloud Speech library for Python <https://cloud.google.com/speech-to-text/docs/quickstart>`__ is required if and only if you want to use the Google Cloud Speech API (``recognizer_instance.recognize_google_cloud``).

If not installed, everything in the library will still work, except calling ``recognizer_instance.recognize_google_cloud`` will raise an ``RequestError``.

According to the `official installation instructions <https://cloud.google.com/speech-to-text/docs/quickstart>`__, the recommended way to install this is using `Pip <https://pip.readthedocs.org/>`__: execute ``pip install google-cloud-speech`` (replace ``pip`` with ``pip3`` if using Python 3).



