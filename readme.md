# RoastLearner
#### Machine learning audio classification engine for Artisan

RoastLearner is a collection of scripts to record audio samples during the coffee roasting process and to classify the recorded sounds into user-defined classes like "firstcrack" or "environment".  This data can be presented to the [Artisan Roaster Scope](https://github.com/artisan-roaster-scope/artisan) software to be graphed or to help control the roast in response to audible events.

RoastLearner also includes tools to train classification engines against data recorded from previous roasts.

RoastLearner acts as a "shell" for the excellent [PyAudioAnalysis](https://github.com/tyiannak/pyAudioAnalysis) audio classification toolkit.  The RoastLearner distribution also includes compiled binaries for [SoX](http://sox.sourceforge.net/) to record audio from your default microphone.

### Requirements
* RoastLearner currently supports Windows installations only.
* [Artisan](https://github.com/artisan-roaster-scope/artisan) 1.0 or above
* Python 2.7 for Windows and a pile of additional modules.  [Read here](documentation/Deploy_Python27.md) for detailed installation instructions on setting up the Python environment.
* A microphone positioned somewhere where it can pick up the sounds from your roaster.  This was developed with a cheap $7 USB microphone, so nothing fancy is required here.  The microphone must be set as the default recording device in Windows.

### Getting Started
1. [Install Artisan](https://github.com/artisan-roaster-scope/artisan/blob/master/wiki/Installation.md) to the default location.
2. [Install Python27, our required modules, and the PyAudioAnalysis libraries](documentation/Deploy_Python27.md).
3. [Install RoastLearner](documentation/Install_RoastLearner.md).
4. [Configure Artisan to run RoastLearner](documentation/Install_RoastLearner.md#Artisan-device-configuration).
5. Run one or more roasts to collect some initial recordings of the sounds your machine makes during the roast process.
6. [Manually classify your recordings and train the RoastLearner classifier(s)](documentation/Train_RoastLearner.md).
