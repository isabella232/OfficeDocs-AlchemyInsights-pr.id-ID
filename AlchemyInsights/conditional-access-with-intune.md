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
# <a name="conditional-access-with-intune"></a><span data-ttu-id="f7869-102">Akses bersyarat dengan Intune</span><span class="sxs-lookup"><span data-stu-id="f7869-102">Conditional Access with Intune</span></span>

<span data-ttu-id="f7869-103">Menggunakan  **akses bersyarat**  dengan Intune memerlukan 3 langkah:</span><span class="sxs-lookup"><span data-stu-id="f7869-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="f7869-104">Membuat  **kebijakan kepatuhan**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [IOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) untuk menentukan pengaturan yang harus dipenuhi sebelum perangkat dianggap patuh.</span><span class="sxs-lookup"><span data-stu-id="f7869-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="f7869-105">Misalnya, perangkat harus memiliki PIN minimal 6 digit sebelum dianggap patuh.</span><span class="sxs-lookup"><span data-stu-id="f7869-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="f7869-106">Buat **kebijakan akses bersyarat**  yang menentukan sumber daya yang sedang diproteksi, dan kondisi apa yang harus dipenuhi untuk mengakses sumber daya tersebut.</span><span class="sxs-lookup"><span data-stu-id="f7869-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="f7869-107">[Misalnya,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  perangkat harus memenuhi syarat sebelum mengakses email korporat.</span><span class="sxs-lookup"><span data-stu-id="f7869-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="f7869-108">Pastikan kebijakan **kepatuhan**  dan  **kebijakan akses bersyarat**  ditargetkan ke grup pengguna yang diinginkan.</span><span class="sxs-lookup"><span data-stu-id="f7869-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="f7869-109">Ini mungkin mengharuskan pembuatan grup pengguna tertentu di Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f7869-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="f7869-110">**Link yang berguna:**</span><span class="sxs-lookup"><span data-stu-id="f7869-110">**Helpful links:**</span></span>

[<span data-ttu-id="f7869-111">Gambaran umum kepatuhan perangkat</span><span class="sxs-lookup"><span data-stu-id="f7869-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="f7869-112">Pemecahan masalah CA</span><span class="sxs-lookup"><span data-stu-id="f7869-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="f7869-113">Kebijakan pemecahan masalah</span><span class="sxs-lookup"><span data-stu-id="f7869-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="f7869-114">Untuk melindungi email (Exchange Online) dari akses dengan perangkat yang tidak patuh, kedua dokumen harus diikuti:</span><span class="sxs-lookup"><span data-stu-id="f7869-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="f7869-115">Proteksi akses email dari perangkat menggunakan EA</span><span class="sxs-lookup"><span data-stu-id="f7869-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="f7869-116">Proteksi akses email dari perangkat menggunakan klien autentikasi modern seperti Outlook</span><span class="sxs-lookup"><span data-stu-id="f7869-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)