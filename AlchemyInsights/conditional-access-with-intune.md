---
title: Akses bersyarat dengan Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931437"
---
# <a name="conditional-access-with-intune"></a>Akses bersyarat dengan Intune

Menggunakan **akses bersyarat** dengan Intune memerlukan 3 langkah:

- Buat **kebijakan kepatuhan** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [IOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) untuk menentukan pengaturan yang harus dipenuhi sebelum perangkat dianggap sesuai. Misalnya, perangkat harus memiliki PIN minimal 6 digit sebelum dianggap sesuai.
- Buat **kebijakan akses bersyarat** yang menentukan sumber daya apa yang dilindungi, dan kondisi apa yang perlu dipenuhi untuk mengakses sumber daya tersebut.  [Misalnya,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) perangkat harus kompatibel sebelum mengakses email perusahaan.
- Pastikan **kebijakan kepatuhan** dan **kebijakan akses bersyarat** ditargetkan ke grup pengguna yang diinginkan. Ini mungkin memerlukan membuat grup pengguna tertentu di Azure Active Directory.

**Link bermanfaat:**

[Ikhtisar kepatuhan perangkat](https://docs.microsoft.com/intune/device-compliance-get-started)

[Pemecahan masalah CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Kebijakan pemecahan masalah](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Untuk melindungi email (Exchange Online) dari akses oleh perangkat noncompliant, kedua dokumen harus diikuti:

1. [Melindungi akses email dari perangkat menggunakan EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Lindungi akses email dari perangkat yang menggunakan klien autentikasi modern seperti Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)