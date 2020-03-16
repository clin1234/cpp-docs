---
title: "AnalysisControl enum class"
description: "The C++ Build Insights SDK AnalysisControl enum reference."
ms.date: "02/12/2020"
helpviewer_keywords: ["C++ Build Insights", "C++ Build Insights SDK", "AnalysisControl", "throughput analysis", "build time analysis", "vcperf.exe"]
---
# AnalysisControl enum class

::: moniker range="<=vs-2015"

The C++ Build Insights SDK is compatible with Visual Studio 2017 and above. To see the documentation for these versions, set the Visual Studio version selector control for this article to Visual Studio 2017 or Visual Studio 2019.

::: moniker-end
::: moniker range=">=vs-2017"

The `AnalysisControl` enum class is used control the flow of an analysis or relogging session. Return an `AnalysisControl` code from an [IAnalyzer](ianalyzer-class.md) or [IRelogger](irelogger-class.md) member function to control what should happen next.

## Members

|  |  |
|--|--|
| `BLOCK` | Prevents the current event from propagating further in the analyzer or relogger group. |
| `CANCEL` | Cancel the current analysis or relogging session. |
| `CONTINUE` | Continue the current analysis or relogging session normally. Propagate the current event to the next analyzer or relogger group member. |
| `FAILURE` | Cancel the current analysis or relogging session and signal an error. |

::: moniker-end