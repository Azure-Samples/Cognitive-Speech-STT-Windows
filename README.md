Microsoft Cognitive Services Speech-to-Text API client SDK and samples
==================================================

This repo contains the client libraries that demonstrate Microsoft’s algorithms
to process spoken language. With these APIs, developers can easily include the
ability to add speech driven actions to their applications. In certain cases,
the APIs also allow for real-time interaction with the user as well. See the
tech in action on [our demo page](<https://www.microsoft.com/cognitive-services/en-us/speech-api>) or
learn more about the API with [our
documentation](<https://www.projectoxford.ai/doc/speech/overview>).

### Speech recognition

Convert spoken audio to text. The API can be directed to turn on and recognize
audio coming from the microphone in real-time, recognize audio coming from a
different real-time audio source, or to recognize audio from within a file. In
all cases, real-time streaming is available, so as the audio is being sent to
the server, partial recognition results are also being returned.

### Speech intent recognition

Convert spoken audio to intent. Similar to Speech Recognition, Speech Intent
Recognition -in addition to returning recognized text from audio input- returns
structured information about the incoming speech so that apps can easily parse
the intent of the speaker, and subsequently drive further action.

The sample
==========

This sample is a Windows WPF application to demonstrate the use of Microsoft Cognitive Services (formerly Project Oxford) Speech To Text API.

It demonstrates the following features using a wav file or external microphone input:

* Short-form recognition.
* Long-form dictation.
* Recognition with intent.

Build the sample
----------------

1.  Start Microsoft Visual Studio 2015 and select `File > Open >
    Project/Solution`.

2.  Starting in the folder where you clone the repository, go to `Speech > SpeechToText > Windows` Folder.

3.  Double-click the Visual Studio 2015 Solution (.sln) file
    SpeechToText-WPF-Sample.

4. Choose the build flavor to be x64. This is important because the sample is using Microsoft.ProjectOxford.SpeechRecognition-x64 nuget package by default.

5.  Press Ctrl+Shift+B, or select `Build > Build Solution`.

For intent recognition to work, you need to sign up [Language Understanding Intelligent Service (LUIS)](<https://www.microsoft.com/cognitive-services/en-us/sign-up>). Please put your LUIS App ID and Subscription ID in app.config file. app.config file can be located from Solution Explorer.

<img src="SampleScreenshots/SampleRunning1.png" width="100%"/>

Run the sample
--------------

After the build is complete, press F5 to run the sample.

First, you must obtain a Speech API subscription key by following instructions in [Microsoft Cognitive Services subscription](<https://www.microsoft.com/cognitive-services/en-us/sign-up>).

Locate the text edit box saying "Paste your subscription key here to start" on
the top right corner. Paste your subscription key. You can choose to persist
your subscription key in your machine by clicking "Save Key" button. When you
want to delete the subscription key from the machine, click "Delete Key" to
remove it from your machine.

Microsoft will receive the audio you upload and may use them to improve Speech
API and related services. By submitting an audio, you confirm you have consent
from everyone in it.

Contributing
============
We welcome contributions and are always looking for new SDKs, input, and
suggestions. Feel free to file issues on the repo and we'll address them as we can. You can also learn more about how you can help on the [Contribution
Rules & Guidelines](</CONTRIBUTING.md>).

For questions, feedback, or suggestions about Microsoft Cognitive Services, feel free to reach out to us directly.

-   [Cognitive Services UserVoice Forum](<https://cognitive.uservoice.com>)

License
=======

All Microsoft Cognitive Services SDKs and samples are licensed with the MIT License. For more details, see
[LICENSE](</LICENSE.md>).

Sample images are licensed separately, please refer to [LICENSE-IMAGE](</LICENSE-IMAGE.md>).
