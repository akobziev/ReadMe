# ApiTests

ApiTest is a based on C# and NUnit framwork library for testing of SaaS.Esign API.
Contains:
- NUnit;
- RestSharp;
- Newtonsoft.Json
- NLog;

## Esign API methods documentation
Navigate to [ESign documentation](https://stage-api-esign.sodapdf.com/swagger/ui/index#/) where you'll found all needed documentation;

## Deployment on local machine

1. Navigate to [ESign git repository](http://tfs.lulusoft.com:8080/tfs/WebCollection/_git/ESign);
2. Click "Clone" button in the top right corner;
3. Click "Clone into Visual Studio" button (Solution will be cloned on your local machine and VS will be opened.);
---
## Structure of the project:
![screenshot_1](https://user-images.githubusercontent.com/45104581/53341395-21c1f800-3914-11e9-8eb0-66b2cc5c06dc.png)

* `TestConfiguration.cs`
> Public class which contains a set of methods to post test data to the [Test] methods through [TestCaseSource] NUnit attribute.
* `Helper.cs`
> Public static class which contains a set of helper methods. 
* `DbQueries.cs`
> Public class which contains a method which gets a session Id data from DataBase.
* `Constants.cs`
> Public static class which contains a set of credentials, passwords, ids etc.
---
* `TestSuites` folder
> TestSuites folder contains:
> * `Account_Tests` folder with test of account api methods;
> * `Package_Tests` folder with test of package api methods;
> * `SignatureAppearance_Test` folder with test of signature appearance api methods.
> * `ApiPreconditions.cs` which contains pre\post-conditions methods for tests.
> ![screenshot_2](https://user-images.githubusercontent.com/45104581/53345095-d06a3680-391c-11e9-82e1-fbec1434ac25.png)

* `TestDocs` folder
> TestDocs folder contains test documents.

* `SignCeremony` folder
> SignCeremony folder contains classes which are taking a part in generating a SignSession json object.

* `Requests` folder
> Requests folder contains classes which are taking a part in sending of get\post\put\delete http request to Esign service.

* `JsonGenerator` folder
> JsonGenerator folder contains classes which are responsible for Esign elements (Signer, Acceptor etc.)

* `FilesToUpload` folder
> FilesToUpload folder contains files for uploading.

* `FilesToUpload` folder
> FilesToUpload folder contains files for uploading.

* `Enum` folder
> Enum folder contains AttachStatus\PackageStatus enums.
