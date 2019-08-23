---
title: Bekerja dengan iOS VPP aplikasi aturan Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: a0bbc1f49f251ef4f16300c8cca98e219008d17e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558002"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="dc6ed-102">Bekerja dengan iOS aplikasi VPP</span><span class="sxs-lookup"><span data-stu-id="dc6ed-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="dc6ed-103">Baca [bagaimana mengelola aplikasi iOS yang dibeli melalui program volume-pembelian dengan Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) untuk mempelajari tentang fitur, kendala, dan langkah-langkah untuk membuat penggunaan Program membeli Apple Volume dan dukungan untuk itu dalam Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="dc6ed-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="dc6ed-104">**Masalah umum:** "Aku ditugaskan iOS VPP app untuk pengguna, tetapi instalasi gagal."</span><span class="sxs-lookup"><span data-stu-id="dc6ed-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="dc6ed-105">Ini dapat terjadi jika tanda VPP tunggal digunakan di beberapa penyedia manajemen perangkat selular.</span><span class="sxs-lookup"><span data-stu-id="dc6ed-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="dc6ed-106">VPP token dari Apple hanya dapat digunakan dengan salah satu penyedia.</span><span class="sxs-lookup"><span data-stu-id="dc6ed-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="dc6ed-107">Jika Anda menggunakan tanda VPP dengan beberapa penyedia, Anda harus kembali upload token untuk Intune.</span><span class="sxs-lookup"><span data-stu-id="dc6ed-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="dc6ed-108">Instalasi juga dapat gagal jika jumlah instalasi melebihi jumlah lisensi.</span><span class="sxs-lookup"><span data-stu-id="dc6ed-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="dc6ed-109">Untuk melihat laporan penggunaan untuk lisensi Anda, buka **Intune Mobile apps** \> halaman **App lisensi** .</span><span class="sxs-lookup"><span data-stu-id="dc6ed-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="dc6ed-110">Untuk mempelajari cara untuk merebut kembali lisensi digunakan, lihat [artikel ini.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="dc6ed-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
