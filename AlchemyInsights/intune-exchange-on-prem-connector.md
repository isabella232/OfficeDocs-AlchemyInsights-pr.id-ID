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
# <a name="intune-exchange-on-premise-connector"></a>Konektor di tempat Exchange Intune

Untuk detail menyetel konektor antara Intune dan Exchange yang dihosting di tempat, lihat dokumentasi berikut ini:

[Menyiapkan konektor Exchange Intune lokal di Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**DITANYAKAN**

P: saya melihat kesalahan seperti "versi konektor Exchange tidak didukung" ketika mencoba menyetel konektor Exchange. Apa penyebabnya?

J: akun yang Anda gunakan dilisensikan dengan benar-lisensi Intune harus aktif

P: Apakah ada beberapa konektor Exchange?

J: Anda hanya bisa menyetel satu konektor Exchange per Intune penyewa per Exchange Organization. Konektor hanya dapat diinstal pada satu server dalam organisasi multi server Exchange.

Anda juga tidak dapat mengonfigurasi konektor untuk Exchange di tempat dan Exchange Online yang dikonfigurasi dalam penyewa yang sama.

P: Bisakah konektor menggunakan larik CAS sebagai hubungannya dengan Exchange?

A: menentukan larik CAS bukan konfigurasi yang didukung dalam penyetelan konektor. Hanya satu server yang harus ditentukan dan harus dikode dalam file konfigurasi konektor yang bisa ditemukan di

program\microsoft\microsoft Intune di tempat konektor Exchange \ OnpremiseExchangeConnectorServiceConfiguration.xml

Temukan entri berikut ini ```<ExchangeWebServiceURL />``` dan ganti URL dengan server Exchange.

**Misalnya**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Silakan lihat dokumentasi berikut ini untuk pemecahan masalah tambahan: [memecahkan masalah konektor Exchange di tempat Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Mengaktifkan pembuatan log verbose untuk konektor Exchange**

1. Buka file konfigurasi pelacakan konektor Exchange untuk pengeditan.  
File terletak di:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Misalnya**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Temukan TraceSourceLine dengan tombol berikut ini: OnPremisesExchangeConnectorService  
  
3. Mengubah nilai simpul SourceLevel dari informasi ActivityTracing (default) untuk Aktivitaspelacakan verbose  

**Misalnya**
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
4. Mulai ulang layanan Microsoft Intune Exchange  
5. Sinkronisasi penuh di portal Intune hingga selesai, lalu mengubah kembali XML ke "Information ActivityTracing" dan memulai ulang layanan Microsoft Intune Exchange.  
6. Lokasi log adalah: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`