# MDU microservice autotest framework.

MasterData Api retrieves master data update history.

MDU microservice autotest framework is a based on C# and NUnit library for testing of MasterData Api.

## MasterData Api Swagers:
- [MasterData Api Test1](http://mdu.test1.nutsservices.local/index.html)
- [MasterData Api Acc1](http://mdu.acc1.nutsservices.local/index.html)
- [MasterData Api Acc3](http://mdu.acc3.nutsservices.local/index.html)

## Project's dependences:
- NUnit framework;
- Newtonsoft.Json;
- EntityFramework;
- Nuts.ApiClient;
- Nuts.MasterData.Contract;
- Nuts.Validation;
- Noksa.NUnit.Allure;
- Microsoft.VisualStudio.SlowCheetah.

## Project's structure:
![8](https://user-images.githubusercontent.com/45104581/58333753-cdf97900-7e46-11e9-88d2-ef77f27a8585.png)

* `IMduHistoryComparer.cs`
> Public interface which contains a `Compare` method which implements in `MduHistoryComparer.cs` class.
* `IMduHistoryComparer.cs`
> Public interface which contains a `Compare` method which implements in `MduHistoryComparer.cs` class.
