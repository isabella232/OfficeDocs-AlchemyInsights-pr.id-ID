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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746030"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="e1732-102">Menggunakan akses bersyarat dengan Intune</span><span class="sxs-lookup"><span data-stu-id="e1732-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="e1732-103">Menggunakan akses bersyarat dengan Intune memerlukan 3 langkah:</span><span class="sxs-lookup"><span data-stu-id="e1732-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="e1732-104">Buat kebijakan kepatuhan untuk menentukan pengaturan yang harus dipenuhi sebelum perangkat dianggap patuh. Misalnya, perangkat harus memiliki PIN minimal 6 digit sebelum dianggap patuh.</span><span class="sxs-lookup"><span data-stu-id="e1732-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="e1732-105">Buat kebijakan akses bersyarat yang menentukan sumber daya yang sedang diproteksi, dan kondisi apa yang harus dipenuhi untuk mengakses sumber daya tersebut. Misalnya, perangkat harus memenuhi syarat sebelum mengakses email korporat.</span><span class="sxs-lookup"><span data-stu-id="e1732-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="e1732-106">Pastikan kebijakan kepatuhan dan kebijakan akses bersyarat ditargetkan ke grup pengguna yang diinginkan. Ini mungkin mengharuskan pembuatan grup pengguna tertentu di Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e1732-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="e1732-107">Baca selengkapnya...</span><span class="sxs-lookup"><span data-stu-id="e1732-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
