# Microsoft Azure Service Fabric 11.5 Release Notes

This release will only be available through Auto upgrades. Clusters set to automatic upgrades will receive this release. For how to configure upgrades, please see [classic](https://docs.microsoft.com/azure/service-fabric/service-fabric-cluster-upgrade) or [managed](https://docs.microsoft.com/azure/service-fabric/how-to-managed-cluster-configuration) documentation.

## Contents
* [Service Fabric Packages and Versions](#service-fabric-packages-and-versions)
* [Service Fabric Feature and Bug Fixes](#service-fabric-feature-and-bug-fixes)

## Service Fabric Packages and Versions

The following packages and versions are part of this release:

| **Service** | **Platform** | **Version** |
|---|---|---|
| Service Fabric Runtime | Windows <br> Windows ARM64 <br> Azure Linux | 11.5.111.1 <br> 11.5.111.2 <br> 11.5.115.5 |
| Service Fabric for Windows Server | Service Fabric Standalone Installer Package | 11.5.111.1 |
| .NET SDK | Windows .NET SDK <br> Microsoft.ServiceFabric <br> Reliable Services and Reliable Actors <br> ASP.NET Core Service Fabric integration | 8.5.111 <br> 11.5.111.1 <br> 8.5.111 <br> 8.5.111 |
| Java SDK | Java for Linux SDK | 1.0.6 |
| Service Fabric PowerShell and CLI | AzureRM PowerShell Module<br>SFCTL | 0.3.15 <br> 11.0.1 |

## Service Fabric Feature and Bug Fixes

Due to an issue with the production rollout of Service Fabric runtime version 11.5.111, we recommend you move to version [11.5.116](Service_Fabric_ReleaseNotes_115_Hotfix.md).
