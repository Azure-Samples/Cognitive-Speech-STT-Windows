# Samples for Microsoft C# speech client library

This repository contains samples for transcribing speech to text using Microsoft Speech Service, an offering within [Microsoft Cognitive Services](https://azure.microsoft.com/services/cognitive-services/), formerly known as Project Oxford.

* [Learn about Microsoft Speech Service](https://azure.microsoft.com/services/cognitive-services/speech/)
* [Read the documentation](https://docs.microsoft.com/azure/cognitive-services/speech/home)
* [Find more SDKs & samples](https://docs.microsoft.com/azure/cognitive-services/speech/getstarted/getstartedclientlibraries)

## The C# client library

The C# client library is provided as Nuget packages. There are two NuGet packages available at [nuget.org](<http://nuget.org>).

* [Microsoft.ProjectOxford.SpeechRecognition-x86](https://www.nuget.org/packages/Microsoft.ProjectOxford.SpeechRecognition-x86/) for x86 build.
* [Microsoft.ProjectOxford.SpeechRecognition-x64](https://www.nuget.org/packages/Microsoft.ProjectOxford.SpeechRecognition-x64/) for x64 build.

## The sample

This sample is a Windows WPF application to demonstrate the use of Speech-to-Text with Microsoft Speech API. It demonstrates the following features using a wav file or external microphone input:

* Short-form recognition
* Long-form dictation
* Recognition with intent

### Build the sample

1. Start Microsoft Visual Studio 2015 and select File > Open > Project/Solution.
2. Navigate to the folder where you cloned the repository.
3. Double-click the Visual Studio 2015 Solution file `SpeechToText-WPF-Sample.sln`.
4. There are 2 projects in the solution. One is for the x86 platform, and the other is for the x64 platform. Choose the build platform (x86 or x64) and configuration (Debug or Release) of your preference, and build the project.
5. For intent recognition to work, you need to sign up to the [Language Understanding Intelligent Service (LUIS)](https://azure.microsoft.com/services/cognitive-services/language-understanding-intelligent-service/). Please put the endpoint URL of your LUIS app in `app.config` file in the `samples/SpeechRecognitionServiceExample` folder. For more infomraiton on the endpoint URL of LUIS app, see [Publish LUIS App](https://docs.microsoft.com/azure/cognitive-services/luis/luis-get-started-create-app#publish-your-app). You must replace the character `&` in the LUIS endpoint URL with `&amp;` to ensure that the URL is correctly interpreted by the XML parser.

### Run the sample

Before running the sample, you must first have a [subscription key](https://azure.microsoft.com/try/cognitive-services/). You can get free trial subscription keys from the [Cognitive Services Subscription](https://azure.microsoft.com/try/cognitive-services/) page. After you select the Speech API, click Get API Key to get the key. It returns a primary and secondary key. Both keys are tied to the same quota, so you may use either key.

Paste your subscription key to the text edit box saying "Paste your subscription key here to start" on the top right corner. You can choose to persist your subscription key in your machine by clicking "Save Key" button. When you want to delete the subscription key from the machine, click "Delete Key" to remove it from your machine.

<img src="SampleScreenshots/SampleRunning1.png" width="100%"/>

Microsoft will receive the audio you upload and may use them to improve the speech API and related services. By submitting an audio, you confirm you have consent from everyone in it.

## Contributing

We welcome contributions. Feel free to file issues and pull requests on this repository and we'll address them as we can. Learn more about how you can help on our [Contribution Rules & Guidelines](</CONTRIBUTING.md>).

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## License

All Microsoft Cognitive Services SDKs and samples are licensed with the MIT License. For more details, see [LICENSE](</LICENSE.md>).

Sample images are licensed separately, please refer to [LICENSE-IMAGE](</LICENSE-IMAGE.md>).

## Developer Code of Conduct

Developers using Cognitive Services, including this client library and sample, are expected to follow the "Developer Code of Conduct for Microsoft Cognitive Services", found at [http://go.microsoft.com/fwlink/?LinkId=698895](http://go.microsoft.com/fwlink/?LinkId=698895).
