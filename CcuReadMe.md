# CCU microservice autotest framework.

CommercialCharacteristic Api retrieves history CCU, last history CCU and message types by dossierId.

CCU microservice autotest framework is a based on C# and NUnit library for testing of MasterData Api.
To create and clean test data in DB this framework uses Nuts.Autotests.CommercialCharacteristic.Sql.

## MasterData Api Swagers:
- [CommercialCharacteristic Api Test1](http://ccu.test1.nutsservices.local)
- [CommercialCharacteristic Api Acc1](http://ccu.acc1.nutsservices.local)
- [CommercialCharacteristic Api Acc3](http://ccu.acc3.nutsservices.local)

## Project's dependences:
- NUnit framework;
- Newtonsoft.Json;
- EntityFramework;
- Nuts.ApiClient;
- Nuts.CommercialCharacteristic.Contract;
- Nuts.Validation;
- Noksa.NUnit.Allure;
- Microsoft.VisualStudio.SlowCheetah.

## Project's structure:
![9](https://user-images.githubusercontent.com/45104581/58488444-07e1bc80-8172-11e9-9184-06cc703c0624.png)

* `ICcuComparer.cs`
> Public interface which contains a `Compare` method which implements in `CcuComparer.cs` class.
* `CcuComparer.cs`
> Public class which implements a `Compare` method to campare pattern with actual result.
* `NutsHttpClient.cs`
> Public class which realizes the http requests sending.
* `PatternMessage.cs`
> Public class which contains the error messages for checking.
* `CcuTestsBase.cs`
> Public abstract base class which creates test data if it need to be done and contains one help method to check CcuResponse.
* `GetCcuHistory.cs`
> Test class which contains test cases to test `GetCcuHistory` api method.
* `GetLastCcuHistory.cs`
> Test class which contains test cases to test `GetLastCcuHistory` api method.
* `GetMessageTypeByDossierId.cs`
> Test class which contains test cases to test `GetMessageTypeByDossierId` api method.
