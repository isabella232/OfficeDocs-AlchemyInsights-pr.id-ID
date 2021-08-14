---
title: Menggunakan Akses Kondisional dengan Intune
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
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005777"
---
# <a name="using-conditional-access-with-intune"></a>Menggunakan Akses Kondisional dengan Intune

Memerlukan 3 langkah berikut ini untuk menggunakan Akses Kondisional dengan Intune:

- [Buat Kebijakan Kepatuhan untuk menetapkan pengaturan yang harus dipenuhi sebelum perangkat dianggap sesuai. Misalnya, perangkat harus memiliki pin yang minimal 6 digit sebelum dianggap sesuai.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Buat Kebijakan Akses Kondisional yang menentukan sumber daya mana yang dilindungi, dan syarat yang harus dipenuhi untuk mengakses sumber daya tersebut. Misalnya, perangkat harus memenuhi syarat sebelum mengakses email perusahaan.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Pastikan bahwa Kebijakan Kepatuhan dan Kebijakan Akses Kondisional ditargetkan ke kelompok pengguna yang diinginkan. Hal ini mungkin memerlukan pembuatan kelompok pengguna tertentu di Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Baca selengkapnya...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
