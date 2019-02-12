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
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903102"
---
# <a name="winsock-error-10061"></a>Winsock kesalahan 10061

Kode kesalahan ini berarti bahwa Office 365 tidak bisa membangun soket TCP (koneksi) dengan target host. Kemungkinan penyebab kesalahan ini adalah masalah dengan konfigurasi firewall Anda. Untuk mengatasi masalah, periksa pengaturan ini:
  
- Memverifikasi Konfigurasi firewall Anda dengan informasi di [kantor 365 URL dan rentang alamat IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- Jika kesalahan tertentu untuk perlindungan Online pertukaran (EOP), Anda harus telah sebelumnya diberitahu untuk perubahan [Alamat IP perlindungan Online pertukaran](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- Pastikan bahwa Anda Internet Service Provider (ISP) tidak memblokir port.
    
- Pastikan pengaturan server host dan target cerdas dalam konektor Anda.
    
Perhatikan bahwa Office 365 tidak memblokir koneksi *masuk* dengan cara ini. 
  

