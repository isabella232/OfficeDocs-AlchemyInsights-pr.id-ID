---
title: Akses bersyarat dengan Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704789"
---
# <a name="conditional-access-with-intune"></a>Akses bersyarat dengan Intune

Menggunakan  **akses bersyarat**  dengan Intune memerlukan 3 langkah:

- Membuat  **kebijakan kepatuhan**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [IOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) untuk menentukan pengaturan yang harus dipenuhi sebelum perangkat dianggap patuh. Misalnya, perangkat harus memiliki PIN minimal 6 digit sebelum dianggap patuh.
- Buat **kebijakan akses bersyarat**  yang menentukan sumber daya yang sedang diproteksi, dan kondisi apa yang harus dipenuhi untuk mengakses sumber daya tersebut.  [Misalnya,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  perangkat harus memenuhi syarat sebelum mengakses email korporat.
- Pastikan kebijakan **kepatuhan**  dan  **kebijakan akses bersyarat**  ditargetkan ke grup pengguna yang diinginkan. Ini mungkin mengharuskan pembuatan grup pengguna tertentu di Azure Active Directory.

**Link yang berguna:**

[Gambaran umum kepatuhan perangkat](https://docs.microsoft.com/intune/device-compliance-get-started)

[Pemecahan masalah CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Kebijakan pemecahan masalah](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Untuk melindungi email (Exchange Online) dari akses dengan perangkat yang tidak patuh, kedua dokumen harus diikuti:

1. [Proteksi akses email dari perangkat menggunakan EA](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Proteksi akses email dari perangkat menggunakan klien autentikasi modern seperti Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)