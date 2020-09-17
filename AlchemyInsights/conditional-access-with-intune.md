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
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807662"
---
# <a name="conditional-access-with-intune"></a>Akses bersyarat dengan Intune

Menggunakan  **akses bersyarat**  dengan Intune memerlukan 3 langkah:

- Membuat  **kebijakan kepatuhan**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [IOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) untuk menentukan pengaturan yang harus dipenuhi sebelum perangkat dianggap patuh. Misalnya, perangkat harus memiliki PIN minimal 6 digit sebelum dianggap patuh.
- Buat **kebijakan akses bersyarat**  yang menentukan sumber daya yang sedang diproteksi, dan kondisi apa yang harus dipenuhi untuk mengakses sumber daya tersebut.  [Misalnya,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  perangkat harus memenuhi syarat sebelum mengakses email korporat.
- Pastikan kebijakan **kepatuhan**  dan  **kebijakan akses bersyarat**  ditargetkan ke grup pengguna yang diinginkan. Ini mungkin mengharuskan pembuatan grup pengguna tertentu di Azure Active Directory.

**Link yang berguna:**

[Gambaran umum kepatuhan perangkat](https://docs.microsoft.com/intune/device-compliance-get-started)

[Pemecahan masalah CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Kebijakan pemecahan masalah](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Untuk melindungi email (Exchange Online) dari akses dengan perangkat yang tidak patuh, kedua dokumen harus diikuti:

1. [Proteksi akses email dari perangkat menggunakan EA](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Proteksi akses email dari perangkat menggunakan klien autentikasi modern seperti Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)