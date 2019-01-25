---
title: 1554 Winsock kesalahan 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 96a9cfd11941158ddf13655c74974e3eb800e570
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/24/2019
ms.locfileid: "29474809"
---
# <a name="winsock-error-10061"></a>Winsock kesalahan 10061

Kode kesalahan ini berarti bahwa Office 365 tidak bisa membangun soket TCP (koneksi) dengan target host. Kemungkinan penyebab kesalahan ini adalah masalah dengan konfigurasi firewall Anda. Untuk mengatasi masalah, periksa pengaturan ini:
  
- Memverifikasi Konfigurasi firewall Anda dengan informasi di [kantor 365 URL dan rentang alamat IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- Jika kesalahan tertentu untuk perlindungan Online pertukaran (EOP), Anda harus telah sebelumnya diberitahu untuk perubahan [Alamat IP perlindungan Online pertukaran](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- Pastikan bahwa Anda Internet Service Provider (ISP) tidak memblokir port.
    
- Pastikan pengaturan server host dan target cerdas dalam konektor Anda.
    
Perhatikan bahwa Office 365 tidak memblokir koneksi *masuk* dengan cara ini. 
  

