---
title: Konektor di tempat Exchange Intune
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807646"
---
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="2b8fe-102">Konektor di tempat Exchange Intune</span><span class="sxs-lookup"><span data-stu-id="2b8fe-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="2b8fe-103">Untuk detail menyetel konektor antara Intune dan Exchange yang dihosting di tempat, lihat dokumentasi berikut ini:</span><span class="sxs-lookup"><span data-stu-id="2b8fe-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="2b8fe-104">Menyiapkan konektor Exchange Intune lokal di Microsoft Intune Azure</span><span class="sxs-lookup"><span data-stu-id="2b8fe-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="2b8fe-105">**DITANYAKAN**</span><span class="sxs-lookup"><span data-stu-id="2b8fe-105">**FAQ:**</span></span>

<span data-ttu-id="2b8fe-106">P: saya melihat kesalahan seperti "versi konektor Exchange tidak didukung" ketika mencoba menyetel konektor Exchange.</span><span class="sxs-lookup"><span data-stu-id="2b8fe-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="2b8fe-107">Apa penyebabnya?</span><span class="sxs-lookup"><span data-stu-id="2b8fe-107">What could be the cause?</span></span>

<span data-ttu-id="2b8fe-108">J: akun yang Anda gunakan dilisensikan dengan benar-lisensi Intune harus aktif</span><span class="sxs-lookup"><span data-stu-id="2b8fe-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="2b8fe-109">P: Apakah ada beberapa konektor Exchange?</span><span class="sxs-lookup"><span data-stu-id="2b8fe-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="2b8fe-110">J: Anda hanya bisa menyetel satu konektor Exchange per Intune penyewa per Exchange Organization.</span><span class="sxs-lookup"><span data-stu-id="2b8fe-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="2b8fe-111">Konektor hanya dapat diinstal pada satu server dalam organisasi multi server Exchange.</span><span class="sxs-lookup"><span data-stu-id="2b8fe-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="2b8fe-112">Anda juga tidak dapat mengonfigurasi konektor untuk Exchange di tempat dan Exchange Online yang dikonfigurasi dalam penyewa yang sama.</span><span class="sxs-lookup"><span data-stu-id="2b8fe-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="2b8fe-113">P: Bisakah konektor menggunakan larik CAS sebagai hubungannya dengan Exchange?</span><span class="sxs-lookup"><span data-stu-id="2b8fe-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="2b8fe-114">A: menentukan larik CAS bukan konfigurasi yang didukung dalam penyetelan konektor.</span><span class="sxs-lookup"><span data-stu-id="2b8fe-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="2b8fe-115">Hanya satu server yang harus ditentukan dan harus dikode dalam file konfigurasi konektor yang bisa ditemukan di</span><span class="sxs-lookup"><span data-stu-id="2b8fe-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="2b8fe-116">program\microsoft\microsoft Intune di tempat konektor Exchange \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="2b8fe-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="2b8fe-117">Temukan entri berikut ini ```<ExchangeWebServiceURL />``` dan ganti URL dengan server Exchange.</span><span class="sxs-lookup"><span data-stu-id="2b8fe-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="2b8fe-118">**Misalnya**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="2b8fe-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="2b8fe-119">Silakan lihat dokumentasi berikut ini untuk pemecahan masalah tambahan: [memecahkan masalah konektor Exchange di tempat Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="2b8fe-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="2b8fe-120">**Mengaktifkan pembuatan log verbose untuk konektor Exchange**</span><span class="sxs-lookup"><span data-stu-id="2b8fe-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="2b8fe-121">Buka file konfigurasi pelacakan konektor Exchange untuk pengeditan.</span><span class="sxs-lookup"><span data-stu-id="2b8fe-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="2b8fe-122">File terletak di:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="2b8fe-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="2b8fe-123">**Misalnya**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="2b8fe-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="2b8fe-124">Temukan TraceSourceLine dengan tombol berikut ini: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="2b8fe-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="2b8fe-125">Mengubah nilai simpul SourceLevel dari informasi ActivityTracing (default) untuk Aktivitaspelacakan verbose</span><span class="sxs-lookup"><span data-stu-id="2b8fe-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="2b8fe-126">**Misalnya**</span><span class="sxs-lookup"><span data-stu-id="2b8fe-126">**Example:**</span></span>
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. <span data-ttu-id="2b8fe-127">Mulai ulang layanan Microsoft Intune Exchange</span><span class="sxs-lookup"><span data-stu-id="2b8fe-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="2b8fe-128">Sinkronisasi penuh di portal Intune hingga selesai, lalu mengubah kembali XML ke "Information ActivityTracing" dan memulai ulang layanan Microsoft Intune Exchange.</span><span class="sxs-lookup"><span data-stu-id="2b8fe-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="2b8fe-129">Lokasi log adalah: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="2b8fe-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>