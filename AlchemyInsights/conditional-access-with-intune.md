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
# <a name="conditional-access-with-intune"></a><span data-ttu-id="5faff-102">Akses bersyarat dengan Intune</span><span class="sxs-lookup"><span data-stu-id="5faff-102">Conditional Access with Intune</span></span>

<span data-ttu-id="5faff-103">Menggunakan **akses bersyarat** dengan Intune memerlukan 3 langkah:</span><span class="sxs-lookup"><span data-stu-id="5faff-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="5faff-104">Buat **kebijakan kepatuhan** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [IOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) untuk menentukan pengaturan yang harus dipenuhi sebelum perangkat dianggap sesuai.</span><span class="sxs-lookup"><span data-stu-id="5faff-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="5faff-105">Misalnya, perangkat harus memiliki PIN minimal 6 digit sebelum dianggap sesuai.</span><span class="sxs-lookup"><span data-stu-id="5faff-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="5faff-106">Buat **kebijakan akses bersyarat** yang menentukan sumber daya apa yang dilindungi, dan kondisi apa yang perlu dipenuhi untuk mengakses sumber daya tersebut.</span><span class="sxs-lookup"><span data-stu-id="5faff-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="5faff-107">[Misalnya,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) perangkat harus kompatibel sebelum mengakses email perusahaan.</span><span class="sxs-lookup"><span data-stu-id="5faff-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="5faff-108">Pastikan **kebijakan kepatuhan** dan **kebijakan akses bersyarat** ditargetkan ke grup pengguna yang diinginkan.</span><span class="sxs-lookup"><span data-stu-id="5faff-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="5faff-109">Ini mungkin memerlukan membuat grup pengguna tertentu di Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5faff-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="5faff-110">**Link bermanfaat:**</span><span class="sxs-lookup"><span data-stu-id="5faff-110">**Helpful links:**</span></span>

[<span data-ttu-id="5faff-111">Ikhtisar kepatuhan perangkat</span><span class="sxs-lookup"><span data-stu-id="5faff-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="5faff-112">Pemecahan masalah CA</span><span class="sxs-lookup"><span data-stu-id="5faff-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="5faff-113">Kebijakan pemecahan masalah</span><span class="sxs-lookup"><span data-stu-id="5faff-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="5faff-114">Untuk melindungi email (Exchange Online) dari akses oleh perangkat noncompliant, kedua dokumen harus diikuti:</span><span class="sxs-lookup"><span data-stu-id="5faff-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="5faff-115">Melindungi akses email dari perangkat menggunakan EAS</span><span class="sxs-lookup"><span data-stu-id="5faff-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="5faff-116">Lindungi akses email dari perangkat yang menggunakan klien autentikasi modern seperti Outlook</span><span class="sxs-lookup"><span data-stu-id="5faff-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)