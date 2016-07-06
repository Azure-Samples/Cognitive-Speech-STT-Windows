# Microsoft Bing Speech API: Windows Speech-to-Text Sample
This repo contains the Windows client library & sample for using Speech-to-Text in the Microsoft Bing Speech API, an offering within [Microsoft Cognitive Services](https://www.microsoft.com/cognitive-services), formerly known as Project Oxford.
* [Learn about the Bing Speech API](https://www.microsoft.com/cognitive-services/en-us/speech-api)
* [Read the documentation](https://www.microsoft.com/cognitive-services/en-us/speech-api/documentation/overview)
* [Find more SDKs & Samples](https://www.microsoft.com/cognitive-services/en-us/SDK-Sample?api=bing%20speech)


## The Client Library
The Speech-to-Text client library is a thin C\# client wrapper for Bing Speech API. 

The easiest way to use this client library is to get microsoft.projectoxford.vision package from [nuget](<http://nuget.org>). There are two nuget packages. One is for x86 build, and one is for x64 build.
 * For x86 package, please go to [Speech Recognition API x86 Package in nuget](https://www.nuget.org/packages/Microsoft.ProjectOxford.SpeechRecognition-x86/) for more details.
 * For x64 package, please go to [Speech Recognition API x64 Package in nuget](https://www.nuget.org/packages/Microsoft.ProjectOxford.SpeechRecognition-x64/) for more details.


## The Sample
This sample is a Windows WPF application to demonstrate the use of Speech-to-Text in the Bing Speech API. It demonstrates the following features using a wav file or external microphone input:
 * Short-form recognition
 * Long-form dictation
 * Recognition with intent

### Build the sample
 1. Start Microsoft Visual Studio 2015 and select `File > Open >
    Project/Solution`.

 2. Starting in the folder where you clone the repository, go to `Speech > SpeechToText > Windows` Folder.

 3. Double-click the Visual Studio 2015 Solution (.sln) file
    SpeechToText-WPF-Sample.

 4. Choose the build flavor to be x64. This is important because the sample is using Microsoft.ProjectOxford.SpeechRecognition-x64 nuget package by default.

 5. Press Ctrl+Shift+B, or select `Build > Build Solution`.

For intent recognition to work, you need to sign up [Language Understanding Intelligent Service (LUIS)](<https://www.microsoft.com/cognitive-services/en-us/sign-up>). Please put your LUIS App ID and Subscription ID in app.config file. app.config file can be located from Solution Explorer.

<img src="SampleScreenshots/SampleRunning1.png" width="100%"/>

### Run the sample
After the build is complete, press F5 to run the sample.

First, you must obtain a Speech API subscription key by [following the instructions on our website](<https://www.microsoft.com/cognitive-services/en-us/sign-up>).

Locate the text edit box saying "Paste your subscription key here to start" on the top right corner. Paste your subscription key. You can choose to persist your subscription key in your machine by clicking "Save Key" button. When you want to delete the subscription key from the machine, click "Delete Key" to remove it from your machine.

Microsoft will receive the audio you upload and may use them to improve the Bing Speech API and related services. By submitting an audio, you confirm you have consent from everyone in it.

## Contributing
We welcome contributions. Feel free to file issues and pull requests on the repo and we'll address them as we can. Learn more about how you can help on our [Contribution Rules & Guidelines](</CONTRIBUTING.md>). 

You can reach out to us anytime with questions and suggestions using our communities below:
 - **Support questions:** [StackOverflow](<https://stackoverflow.com/questions/tagged/microsoft-cognitive>)
 - **Feedback & feature requests:** [Cognitive Services UserVoice Forum](<https://cognitive.uservoice.com>)

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.


## License
All Microsoft Cognitive Services SDKs and samples are licensed with the MIT License. For more details, see
[LICENSE](</LICENSE.md>).

Sample images are licensed separately, please refer to [LICENSE-IMAGE](</LICENSE-IMAGE.md>).


## Developer Code of Conduct
Developers using Cognitive Services, including this client library & sample, are expected to follow the “Developer Code of Conduct for Microsoft Cognitive Services”, found at [http://go.microsoft.com/fwlink/?LinkId=698895](http://go.microsoft.com/fwlink/?LinkId=698895).
