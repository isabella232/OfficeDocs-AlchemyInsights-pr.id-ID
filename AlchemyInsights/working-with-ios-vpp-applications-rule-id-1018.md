---
title: Bekerja dengan iOS VPP aplikasi aturan id 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719960"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="a4170-102">Bekerja dengan aplikasi iOS VPP</span><span class="sxs-lookup"><span data-stu-id="a4170-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="a4170-103">Baca [cara mengelola aplikasi IOS yang dibeli melalui program pembelian volume dengan Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) untuk mempelajari tentang fitur, kendala, dan langkah untuk memanfaatkan program pembelian volume Apple dan dukungan untuk itu di Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="a4170-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="a4170-104">**Masalah umum:** "Saya menugaskan aplikasi iOS VPP ke pengguna saya, namun penginstalan gagal."</span><span class="sxs-lookup"><span data-stu-id="a4170-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="a4170-105">Hal ini dapat terjadi jika Token VPP tunggal digunakan di beberapa penyedia manajemen perangkat seluler.</span><span class="sxs-lookup"><span data-stu-id="a4170-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="a4170-106">Token VPP dari Apple hanya dapat digunakan dengan satu penyedia.</span><span class="sxs-lookup"><span data-stu-id="a4170-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="a4170-107">Jika Anda menggunakan token VPP dengan beberapa penyedia, Anda harus kembali meng-upload token ke Intune.</span><span class="sxs-lookup"><span data-stu-id="a4170-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="a4170-108">Penginstalan juga dapat gagal jika jumlah total penginstalan melebihi jumlah lisensi.</span><span class="sxs-lookup"><span data-stu-id="a4170-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="a4170-109">Untuk melihat laporan penggunaan untuk lisensi Anda, buka halaman \> **lisensi aplikasi** **aplikasi seluler Intune** .</span><span class="sxs-lookup"><span data-stu-id="a4170-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="a4170-110">Untuk mempelajari cara merebut kembali lisensi yang digunakan, lihat [artikel ini.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="a4170-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
