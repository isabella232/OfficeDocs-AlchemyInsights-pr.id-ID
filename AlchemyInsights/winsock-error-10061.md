---
title: 1554 Winsock galat 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766172"
---
# <a name="winsock-error-10061"></a>Winsock galat 10061

Kode galat ini berarti bahwa Microsoft tidak dapat membuat soket TCP (sambungan) dengan target host. Kemungkinan penyebab kesalahan ini adalah masalah dengan konfigurasi firewall Anda. Untuk memperbaiki masalah, periksa pengaturan ini:

- Verifikasi Konfigurasi firewall Anda dengan informasi di [Microsoft 365 URL dan kisaran alamat IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Jika galat khusus untuk Exchange Online Protection (EOP), Anda harus telah diberitahu sebelumnya untuk mengubah [Alamat IP perlindungan Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Verifikasi bahwa Internet Service Provider (ISP) tidak memblokir Port.

- Verifikasi host cerdas dan pengaturan server target di konektor Anda.

Perhatikan bahwa Microsoft 365 tidak memblokir koneksi *masuk* dengan cara ini.
