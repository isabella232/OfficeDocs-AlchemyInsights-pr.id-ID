---
title: Tidak dapat masuk ke Teams karena kesalahan autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932042"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="3b11e-102">Tidak dapat masuk ke Teams karena kesalahan autologon.microsoftazuread-sso dot com: 443</span><span class="sxs-lookup"><span data-stu-id="3b11e-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="3b11e-103">Jika SSO Tanpa Hambatan diaktifkan sebagai otentikasi O365, URL "autologon.microsoftazuread-sso.com" mungkin perlu ditambahkan ke Situs Intranet.</span><span class="sxs-lookup"><span data-stu-id="3b11e-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="3b11e-104">Jika sebelumnya sudah ditambahkan ke Situs Tepercaya dan SSO Tanpa Hambatan sedang digunakan, situs harus dihapus dari Situs Tepercaya.</span><span class="sxs-lookup"><span data-stu-id="3b11e-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="3b11e-105">Tinjau [Daftar Periksa Pemecahan Masalah SSO Tanpa Hambatan](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="3b11e-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="3b11e-106">Ikuti langkah-langkah ini untuk menambahkan URL ke daftar Situs Intranet:</span><span class="sxs-lookup"><span data-stu-id="3b11e-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="3b11e-107">Buka Internet Explorer dengan mengklik tombol **Mulai**.</span><span class="sxs-lookup"><span data-stu-id="3b11e-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="3b11e-108">Dalam kotak pencarian, ketik Internet Explorer, lalu klik **Internet Explorer** dalam daftar hasil.</span><span class="sxs-lookup"><span data-stu-id="3b11e-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="3b11e-109">Klik **Alat**, lalu klik **Opsi Internet**.</span><span class="sxs-lookup"><span data-stu-id="3b11e-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="3b11e-110">Klik tab **Keamanan**.</span><span class="sxs-lookup"><span data-stu-id="3b11e-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="3b11e-111">Sekarang klik **Situs Intranet Lokal** lalu klik tombol **situs** lalu tombol **Tingkat Lanjut**.</span><span class="sxs-lookup"><span data-stu-id="3b11e-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="3b11e-112">Masukkan URL Situs Web dan klik **Tambahkan**.</span><span class="sxs-lookup"><span data-stu-id="3b11e-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="3b11e-113">Setelah selesai, klik **Tutup**.</span><span class="sxs-lookup"><span data-stu-id="3b11e-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="3b11e-114">Untuk informasi selengkapnya, lihat [Dokumentasi untuk penyebaran SSO Tanpa Hambatan untuk O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (mencakup proses berbasis Kebijakan untuk menambahkan URL ke Situs Intranet di Langkah 3).</span><span class="sxs-lookup"><span data-stu-id="3b11e-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
