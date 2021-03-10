---
title: Menggunakan akses bersyarat dengan Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693578"
---
# <a name="using-conditional-access-with-intune"></a>Menggunakan akses bersyarat dengan Intune

Menggunakan akses bersyarat dengan Intune memerlukan 3 langkah:

- [Buat kebijakan kepatuhan untuk menentukan pengaturan yang harus dipenuhi sebelum perangkat dianggap patuh. Misalnya, perangkat harus memiliki PIN minimal 6 digit sebelum dianggap patuh.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Buat kebijakan akses bersyarat yang menentukan sumber daya yang sedang diproteksi, dan kondisi apa yang harus dipenuhi untuk mengakses sumber daya tersebut. Misalnya, perangkat harus memenuhi syarat sebelum mengakses email korporat.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Pastikan kebijakan kepatuhan dan kebijakan akses bersyarat ditargetkan ke grup pengguna yang diinginkan. Ini mungkin mengharuskan pembuatan grup pengguna tertentu di Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Baca selengkapnya...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
