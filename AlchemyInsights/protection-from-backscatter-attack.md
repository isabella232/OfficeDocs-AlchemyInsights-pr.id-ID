---
title: Proteksi dari serangan Backscatter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036074"
---
# <a name="protection-from-backscatter-attack"></a>Proteksi dari serangan Backscatter

Backscatter adalah laporan tidak terkirim (juga dikenal sebagai NDR atau pesan pantulan) yang Anda terima untuk pesan yang tidak terkirim. Spammer menempa (spoof) Alamat **dari:** dari pesan mereka, dan mereka sering menggunakan alamat email nyata untuk meminjamkan kredibilitas pada pesan mereka. Jadi, saat spammer tidak mau mengirimkan pesan ke penerima yang tidak ada, server email tujuan pada dasarnya ditipu untuk mengembalikan pesan yang tidak terkirim dalam NDR ke pengirim yang ditempa di alamat **dari:** .

Informasi tambahan dapat ditemukan dalam [Backscatter di EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).

**Mengaktifkan proteksi Backscatter**

Untuk mengaktifkan proteksi Backscatter, ikuti jalur di bawah ini.

**protection.office.com > Threat Management > Policy > AntiSpam > memilih kebijakan filter spam dan mengedit kebijakan > properti spam > Tandai sebagai spam > NDR Backscatter > menetapkannya ke "aktif"**

Jika Anda yakin akun telah disalahgunakan, lihat yang berikut ini:

- [Membalas akun email yang dikompromikan](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [Menghapus pengguna yang diblokir dari portal pengguna terbatas di Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



