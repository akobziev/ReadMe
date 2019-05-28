# MDU microservice autotest framework.

MasterData Api retrieves master data update history.

MDU microservice autotest framework is a based on C# and NUnit library for testing of MasterData Api.
To create test data in DB this framework uses Nuts.Autotests.MasterData.Cache instead of Sql requests.

## MasterData Api Swagers:
- [MasterData Api Test1](http://mdu.test1.nutsservices.local/index.html)
- [MasterData Api Acc1](http://mdu.acc1.nutsservices.local/index.html)
- [MasterData Api Acc3](http://mdu.acc3.nutsservices.local/index.html)

## Project's dependences:
- NUnit framework;
- Newtonsoft.Json;
- EntityFramework;
- Microsoft.EntityFrameworkCore (version: 2.1.8);
- Nuts.ApiClient;
- Nuts.MasterData.Contract;
- Nuts.Validation;
- Noksa.NUnit.Allure;
- Microsoft.VisualStudio.SlowCheetah.

## Project's structure:
![8](https://user-images.githubusercontent.com/45104581/58333753-cdf97900-7e46-11e9-88d2-ef77f27a8585.png)

* `IMduHistoryComparer.cs`
> Public interface which contains a `Compare` method which implements in `MduHistoryComparer.cs` class.
* `MduHistoryComparer.cs`
> Public class which implements a `Compare` method to campare pattern with actual result.
* `NutsHttpClient.cs`
> Public class which realizes the http requests sending.
* `PatternMessage.cs`
> Public class which contains the error messages for checking.
* `MduBaseTests.cs`
> Public abstract base class which creates test data if it need to be done and contains one help method to check MduResponse.
