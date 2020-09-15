---
title: kesalahan Winsock 1554 10061
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
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698865"
---
# <a name="winsock-error-10061"></a>Kesalahan Winsock 10061

Kode kesalahan ini berarti Microsoft tidak dapat membuat soket TCP (koneksi) dengan host target. Kemungkinan penyebab kesalahan ini adalah masalah dengan konfigurasi firewall Anda. Untuk memperbaiki masalah tersebut, periksa pengaturan ini:

- Memverifikasi Konfigurasi firewall Anda dengan informasi dalam [URL dan rentang alamat IP Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Jika kesalahan tersebut khusus untuk Exchange Online Protection (EOP), Anda seharusnya telah diberitahu sebelumnya untuk mengubah [Alamat IP proteksi Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Verifikasi bahwa penyedia layanan internet (ISP) Anda tidak memblokir Port.

- Verifikasi pengaturan server Smart host dan target di konektor Anda.

Perhatikan bahwa Microsoft 365 tidak memblokir koneksi *masuk* dengan cara ini.
