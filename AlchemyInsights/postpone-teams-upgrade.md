---
title: Menunda pemutakhiran tim
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2737"
- "4000006"
ms.openlocfilehash: ae0611df247790200d0192e018ff5f0128f23cb4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741774"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="8c87d-102">Cara menunda pemutakhiran tim yang didukung Microsoft</span><span class="sxs-lookup"><span data-stu-id="8c87d-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="8c87d-103">**Penting**: kami bisa membantu memperbaiki hal ini untuk Anda menggunakan diagnostik dukungan, tapi kelihatannya Anda tidak menggunakan pusat admin baru.</span><span class="sxs-lookup"><span data-stu-id="8c87d-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="8c87d-104">Untuk menggunakan pusat admin baru, geser tombol alih di bagian kanan atas yang bertuliskan **Pusat admin baru** ke kanan.</span><span class="sxs-lookup"><span data-stu-id="8c87d-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="8c87d-105">Menggunakan pusat admin baru, klik widget **perlu bantuan?** , ketikkan "tunda pemutakhiran tim", lalu ikuti perintah untuk menjalankan diagnostik.</span><span class="sxs-lookup"><span data-stu-id="8c87d-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="8c87d-106">Jika Anda menerima komunikasi tentang pemutakhiran otomatis berbasis Microsoft dari Skype for Business ke Microsoft teams, dan Anda ingin menunda pemutakhiran otomatis ke yang lebih baru, admin global Anda bisa masuk ke [portal admin teams](https://admin.teams.microsoft.com/dashboard) dan, setelah memilih tombol **refresh status** di bawah Pemutakhiran Microsoft teams, pilih tombol **tunda** .</span><span class="sxs-lookup"><span data-stu-id="8c87d-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="8c87d-107">Untuk melihat tanggal baru untuk pemutakhiran otomatis penyewa Anda ke Microsoft teams, refresh halaman portal admin teams.</span><span class="sxs-lookup"><span data-stu-id="8c87d-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="8c87d-108">**Catatan:** Tombol **tunda** hanya akan tersedia jika Anda telah menerima pemberitahuan pusat pesan tentang pemutakhiran otomatis.</span><span class="sxs-lookup"><span data-stu-id="8c87d-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="8c87d-109">Admin global juga bisa menjalankan [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) untuk mempelajari selengkapnya tentang status pemutakhiran mereka saat ini.</span><span class="sxs-lookup"><span data-stu-id="8c87d-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
