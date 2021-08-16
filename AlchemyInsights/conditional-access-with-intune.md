---
title: Akses Bersyarat dengan Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069715"
---
# <a name="conditional-access-with-intune"></a>Akses Bersyarat dengan Intune

Memerlukan  3 langkah berikut ini untuk menggunakan Akses Kondisional dengan Intune:

- Buat Kebijakan **Kepatuhan** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) untuk menetapkan pengaturan yang harus dipenuhi sebelum perangkat dianggap sesuai. Misalnya, perangkat harus memiliki pin yang minimal 6 digit sebelum dianggap sesuai.
- Buat Kebijakan **Akses Kondisional**  yang menentukan sumber daya mana yang dilindungi, dan syarat yang harus dipenuhi untuk mengakses sumber daya tersebut.  [Misalnya, perangkat](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  harus memenuhi syarat sebelum mengakses email perusahaan.
- Pastikan bahwa **Kebijakan Kepatuhan**  dan Kebijakan  **Akses Kondisional**  ditargetkan ke kelompok pengguna yang diinginkan. Hal ini mungkin memerlukan pembuatan kelompok pengguna tertentu di Azure Active Directory.

**Tautan yang berguna:**

[Gambaran umum kepatuhan perangkat](https://docs.microsoft.com/intune/device-compliance-get-started)

[Memecahkan masalah CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Kebijakan pemecahan masalah](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Untuk melindungi Email (Exchange online) dari akses dengan perangkat nonkompilasi, kedua dokumen harus diikuti:

1. [Melindungi akses email dari perangkat menggunakan EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Melindungi akses email dari perangkat yang menggunakan klien autentikasi modern seperti Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)