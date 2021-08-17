---
title: 1554 Kesalahan kemenangan 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083233"
---
# <a name="winsock-error-10061"></a>Kesalahanock kemenangan 10061

Kode kesalahan ini berarti bahwa Microsoft tidak dapat menetapkan soket TCP (koneksi) dengan host target. Kemungkinan besar penyebab kesalahan ini adalah masalah dengan konfigurasi firewall Anda. Untuk memperbaiki masalah, periksa pengaturan ini:

- Memverifikasi konfigurasi firewall Anda dengan informasi [Microsoft 365 URL dan rentang alamat IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Jika kesalahan ber spesifik untuk Exchange Online Protection (EOP), Anda harus diberi tahu sebelumnya bahwa ada perubahan pada [Exchange Online Protection IP eksternal.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- Verifikasi bahwa Penyedia Layanan Internet (ISP) Anda tidak memblokir port.

- Verifikasi pengaturan host cerdas dan server target di konektor Anda.

Perhatikan bahwa Microsoft 365 koneksi masuk *dengan* cara ini.
