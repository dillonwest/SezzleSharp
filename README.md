# SezzleSharp
A Sezzle C# SDK

[![Build status](https://ci.appveyor.com/api/projects/status/5yixr8hm3n33ej67?svg=true)](https://ci.appveyor.com/project/StephenPAdams/sezzlesharp)
[![NuGet Version](https://img.shields.io/nuget/v/SixFourThree.SezzleSharp.svg?style=flat-square)](https://www.nuget.org/packages/SixFourThree.SezzleSharp)

This library is still in development. This SDK will wire up the following endpoints and features from the Sezzle Pay API:

* Authentication POST https://gateway.sezzle.com/v1/authentication - DONE
* Configuration POST https://gateway.sezzle.com/v1/configuration - DONE
* Checkouts (Create) POST https://gateway.sezzle.com/v1/checkouts - DONE*
* Checkouts (Complete) POST https://gateway.sezzle.com/v1/checkouts/{order_reference_id}/complete - DONE*
* Orders (Details) GET https://gateway.sezzle.com/v1/orders/{order_reference_id} - PENDING TESTS
* Orders (Refund) POST https://gateway.sezzle.com/v1/orders/{order_reference_id}/refund - PENDING TESTS
* Order Webhook modeling - PENDING TESTS

*Pending Sezzle developer support giving information regarding why the shipping address isn't being populated on the Orders (Details) call. Need to ensure it's being saved on checkout create appropriately.

# Sandbox
For more information about the Sezzle sandbox, please see documentation located here: https://docs.sezzle.com/#sandbox