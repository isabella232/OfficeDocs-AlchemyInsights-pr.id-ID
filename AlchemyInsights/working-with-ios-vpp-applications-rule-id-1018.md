---
title: Bekerja dengan aturan aplikasi VPP iOS id 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688949"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="048eb-102">Bekerja dengan aplikasi iOS VPP</span><span class="sxs-lookup"><span data-stu-id="048eb-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="048eb-103">Baca [cara mengelola aplikasi IOS yang dibeli melalui program pembelian-Borongan dengan Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) untuk mempelajari tentang fitur, batasan, dan langkah-langkah untuk memanfaatkan program pembelian di Apple dan dukungan untuk Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="048eb-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="048eb-104">**Masalah umum:** "Saya menugaskan aplikasi VPP iOS kepada pengguna saya, tapi penginstalan gagal."</span><span class="sxs-lookup"><span data-stu-id="048eb-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="048eb-105">Hal ini bisa terjadi jika Token VPP digunakan di beberapa penyedia manajemen perangkat seluler.</span><span class="sxs-lookup"><span data-stu-id="048eb-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="048eb-106">Token VPP dari Apple hanya dapat digunakan dengan satu penyedia.</span><span class="sxs-lookup"><span data-stu-id="048eb-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="048eb-107">Jika Anda menggunakan token VPP dengan beberapa penyedia, Anda harus mengunggah ulang token ke Intune.</span><span class="sxs-lookup"><span data-stu-id="048eb-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="048eb-108">Penginstalan juga bisa gagal jika jumlah total instalasi melebihi jumlah lisensi.</span><span class="sxs-lookup"><span data-stu-id="048eb-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="048eb-109">Untuk menampilkan laporan penggunaan untuk lisensi Anda, buka **Intune Mobile apps** \> halaman **lisensi aplikasi** seluler Intune.</span><span class="sxs-lookup"><span data-stu-id="048eb-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="048eb-110">Untuk mempelajari cara mendapatkan kembali lisensi yang sedang digunakan, lihat [artikel ini.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="048eb-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
