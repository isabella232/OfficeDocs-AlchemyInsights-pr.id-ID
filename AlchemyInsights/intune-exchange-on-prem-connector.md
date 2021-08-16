---
title: Konektor Exchange Lokal Intune
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
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013967"
---
# <a name="intune-exchange-on-premise-connector"></a>Konektor Exchange Lokal Intune

Untuk detail tentang menyiapkan konektor antara Intune dan Exchange yang dihosting secara lokal, silakan lihat dokumentasi berikut:

[Menyiapkan konektor Exchange lokal Intune di Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**FAQ:**

T: Saya melihat kesalahan seperti "Versi Exchange Connector tidak didukung" saat mencoba menyiapkan konektor Exchange. Apa penyebabnya?

A: Akun yang Anda gunakan memiliki lisensi yang tepat. Akun tersebut harus memiliki lisensi Intune aktif

T: Apakah mungkin memiliki beberapa Exchange konektor?

A: Anda hanya dapat menyiapkan satu konektor Exchange per penyewa Intune per Exchange organisasi. Konektor hanya bisa diinstal di satu server di organisasi pertukaran multi server.

Anda juga tidak bisa memiliki konektor yang dikonfigurasi untuk Exchange di tempat dan Exchange Online dikonfigurasi dalam penyewa yang sama.

T: Bisakah konektor menggunakan array CAS sebagai koneksinya ke Exchange?

A: Menentukan larik CAS bukanlah konfigurasi yang didukung dalam penyiapan konektor. Hanya server tunggal yang harus ditentukan dan harus memiliki kode keras dalam file konfigurasi konektor yang dapat ditemukan di

program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml

Temukan entri berikut ```<ExchangeWebServiceURL />``` ini dan ganti URL dengan server exchange.

**Contoh:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Silakan lihat dokumentasi berikut ini untuk pemecahan masalah [tambahan: Memecahkan masalah intune lokal Exchange konektor](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Mengaktifkan pembuatan log Verbose untuk Exchange konektor**

1. Buka Exchange connectortracing configuration file for editing.  
File berada di : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Contoh:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Temukan TraceSourceLine dengan kunci berikut ini: OnPremisesExchangeConnectorService  
  
3. Mengubah nilai node SourceLevel dari Penelusuran Aktivitas Informasi (default) ke Verbose ActivityTracing  

**Contoh:**
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
4. Mulai ulang Microsoft Intune Exchange Layanan  
5. Sinkronisasi penuh di Portal Intune hingga selesai, lalu ubah XML kembali ke "Penelusuran Aktivitas Informasi" dan mulai ulang Layanan Microsoft Intune Exchange Lanjut.  
6. Lokasi log adalah: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`