# New Relic Agent for Xamarin

## Description

A nuget package to use New Relic Agent on Xamarin projects for Xamarin.iOS and Xamarin.Android

## Agent version
 ###  Xamarin.iOS
The agent for Xamarin.iOS is currently using the version [7.3.6](https://download.newrelic.com/ios_agent/NewRelic_XCFramework_Agent_7.3.6.zip). 

 ###  Xamarin.Android
The agent for Xamarin.Android is currently using the version [6.7.0](https://download.newrelic.com/android_agent/ant/NewRelic_Android_Agent_6.7.0.zip). 

## Installation

The New Relic agent for Xamarin is available on a NuGet Package called [NewRelicAgentForXamarin](https://www.nuget.org/packages/NewRelicAgentForXamarin/). 

More details for using the agent on [wiki](https://github.com/GlobalsoftWigilabs/xamarin-newrelic-bridge/blob/main/README.md). 


## Working Features

| Name                  | iOS    | Android |
|-----------------------|--------|:-------:|
| App Launches          |   ✅   |   ✅    |          
| Crash report          |   ✅   |   ✅    |
| Custom Events         |   ✅   |   ✅    |
| Custom Attributes     |   ✅   |   ✅    |
| Breadcrumbs           |   ✅   |   ✅    |
| Handled Exceptions    |   ✅   |   ✅    |
| Stack traces          |   ✅   |   ✅    |
| User Interactions     |   ✅   |   ❌    |
| Performance metrics   |   ✅   |   ❌    |
| Http Request          |   ✅   |   ❌    |
| Distributed Tracing   |   ✅   |   ❌    |

### Blocker
The Android agent depends on a Gradle Plugin to make the instrumentation, so the all the features that use the instrumentation are not working yet.

### Blocker's potential solution
New Relic will provide the code and the knowledge on what the Gradle plugin does, so we try to replicate the behavior on the Visual Studio Build pipe.
