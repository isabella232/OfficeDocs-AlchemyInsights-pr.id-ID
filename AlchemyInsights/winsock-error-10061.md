---
title: 1554 Winsock kesalahan 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: f44ed42906b85e63f1f694813f54710906969904
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/22/2019
ms.locfileid: "30772445"
---
# <a name="winsock-error-10061"></a>Winsock kesalahan 10061

Kode kesalahan ini berarti bahwa Office 365 tidak bisa membangun soket TCP (koneksi) dengan target host. Kemungkinan penyebab kesalahan ini adalah masalah dengan konfigurasi firewall Anda. Untuk mengatasi masalah, periksa pengaturan ini:
  
- Memverifikasi Konfigurasi firewall Anda dengan informasi di [kantor 365 URL dan rentang alamat IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- Jika kesalahan tertentu untuk perlindungan Online pertukaran (EOP), Anda harus telah sebelumnya diberitahu untuk perubahan [Alamat IP perlindungan Online pertukaran](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- Pastikan bahwa Anda Internet Service Provider (ISP) tidak memblokir port.
    
- Pastikan pengaturan server host dan target cerdas dalam konektor Anda.
    
Perhatikan bahwa Office 365 tidak memblokir koneksi *masuk* dengan cara ini. 
  

