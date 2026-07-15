# Microsoft Azure Service Fabric 11.6 Release Notes

This release will only be available through Auto upgrades. Clusters set to automatic upgrades will receive this release. For how to configure upgrades, please see [classic](https://docs.microsoft.com/azure/service-fabric/service-fabric-cluster-upgrade) or [managed](https://docs.microsoft.com/azure/service-fabric/how-to-managed-cluster-configuration) documentation.

## Contents
* [Service Fabric Packages and Versions](#service-fabric-packages-and-versions)
* [Service Fabric Feature and Bug Fixes](#service-fabric-feature-and-bug-fixes)
* [Retirement and Deprecation Path Callouts](#retirement-and-deprecation-path-callouts)
* [Repositories and Download Links](#repositories-and-download-links)

## Service Fabric Packages and Versions

Packages and versions are listed with the most recent version listed first.

The following packages and versions are part of this release:

### Service Fabric 11.6.235

| **Service** | **Platform** | **Version** |
|---|---|---|
| [Service Fabric Runtime](https://download.microsoft.com/download/b/8/a/b8a2fb98-0ec1-41e5-be98-9d8b5abf7856/MicrosoftServiceFabric.11.6.235.1.exe) | Windows <br> Windows ARM64 <br> Ubuntu 22 | 11.6.235.1 <br> 11.6.235.2 <br> 11.6.235.4 |
| [Service Fabric for Windows Server](https://download.microsoft.com/download/8/3/6/836e3e99-a300-4714-8278-96bc3e8b5528/11.6.235.1/Microsoft.Azure.ServiceFabric.WindowsServer.11.6.235.1.zip) | Service Fabric Standalone Installer Package | 11.6.235.1 |
| [.NET SDK](https://download.microsoft.com/download/b/8/a/b8a2fb98-0ec1-41e5-be98-9d8b5abf7856/MicrosoftServiceFabricSDK.8.6.235.msi) | Windows .NET SDK <br> Microsoft.ServiceFabric <br> Reliable Services and Reliable Actors <br> ASP.NET Core Service Fabric integration | 8.6.235 <br> 11.6.235.1 <br> 8.6.235 <br> 8.6.235 |

## Key Announcements

* Service Fabric 11.6 improves runtime stability by addressing multiple crash and fail-fast conditions across core runtime components.

## Breaking Changes

* Legacy SMB-based image-store file sharing is no longer supported on Linux. Linux clusters must use the secure non-SMB image-store transfer mode. Review configurations that explicitly depend on SMB-based transfers before upgrading.

## Service Fabric Feature and Bug Fixes

Features and bug fixes are listed by the version in which they were introduced, with the most recent version listed first.

The following features and bug fixes are part of this release:

### Service Fabric 11.6.235 Features and Bug Fixes

| **Type** | **Description** | **Resolution** |
|---|---|---|


## Retirement and Deprecation Path Callouts

* Service Fabric runtime will discontinue support for the Java SDK soon. For a smooth transition, we strongly recommend users to shift to Azure Service Fabric .NET SDK. If your current setup is based on the Service Fabric Java SDK, we suggest starting migration plans to smoothly switch to the Azure Service Fabric .NET SDK. Although applications using the Java SDK will continue to work, we highly recommend adopting the Service Fabric .NET SDK for optimal outcomes.

* Service Fabric runtime will soon be archiving and removing Service Fabric runtime versions less than 7.2 and older, as well as the corresponding SDK version 4.2 packages and older from the package Download Center. Archiving and removing will affect application scaling and re-imaging of virtual machines in a Service Fabric cluster running on unsupported versions. After older versions are removed/archived, this may cause rollback failures when an in-progress upgrade has errors.
  * To prevent disruption of workloads, create a new cluster using the following steps:
    * [Create a Service Fabric cluster using ARM template](https://learn.microsoft.com/azure/service-fabric/quickstart-cluster-template)
    * [Create a Standalone cluster](https://learn.microsoft.com/azure/service-fabric/service-fabric-cluster-creation-for-windows-server)
    * Install the supported version of Service Fabric SDK based on the runtime version installed on the cluster.

## Repositories and Download Links

The list below is an overview of the direct links to the packages associated with this release, with the links for the most recent version listed first.

Follow this guidance for setting up your developer environment: 
* [Getting Started with Linux](https://docs.microsoft.com/azure/service-fabric/service-fabric-get-started-linux)
* [Getting Started with Mac](https://docs.microsoft.com/azure/service-fabric/service-fabric-get-started-mac)
* [Getting Started with Windows](https://docs.microsoft.com/azure/service-fabric/service-fabric-get-started)

### Service Fabric 11.6.235 Repositories and Download Links

Runtime:
https://download.microsoft.com/download/b/8/a/b8a2fb98-0ec1-41e5-be98-9d8b5abf7856/MicrosoftServiceFabric.11.6.235.1.exe

SDK:
https://download.microsoft.com/download/b/8/a/b8a2fb98-0ec1-41e5-be98-9d8b5abf7856/MicrosoftServiceFabricSDK.8.6.235.msi

Cab:
https://download.microsoft.com/download/b/0/b/b0bccac5-65aa-4be3-ab13-d5ff5890f4b5/11.5.116.1/MicrosoftServiceFabric.11.6.235.1.cab

Package:
https://download.microsoft.com/download/8/3/6/836e3e99-a300-4714-8278-96bc3e8b5528/11.6.235.1/Microsoft.Azure.ServiceFabric.WindowsServer.11.6.235.1.zip
 
Goalstate:
https://download.microsoft.com/download/7/d/1/7d1d1511-59a4-4933-8187-40c20065aa29/11.6.235.1/goalstate.11.6.235.1.json
