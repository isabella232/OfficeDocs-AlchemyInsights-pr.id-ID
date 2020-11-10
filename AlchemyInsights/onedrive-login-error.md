---
title: Kesalahan masuk OneDrive AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982481"
---
# <a name="onedrive-login-error-aadsts50011"></a><span data-ttu-id="7e28c-102">Kesalahan masuk OneDrive AADSTS50011</span><span class="sxs-lookup"><span data-stu-id="7e28c-102">OneDrive login error AADSTS50011</span></span>

<span data-ttu-id="7e28c-103">Jika Anda menerima kesalahan "AADSTS50011: URL balasan yang ditentukan dalam permintaan tidak cocok dengan Balasan" saat masuk ke aplikasi OneDrive, periksa hal berikut:</span><span class="sxs-lookup"><span data-stu-id="7e28c-103">If you receive an error "AADSTS50011: The reply URL specified in the request does not match the reply" when signing into the OneDrive app, check for the following:</span></span>

<span data-ttu-id="7e28c-104">Versi OneDrive Anda harus sama dengan atau lebih besar dari versi 20.052. XXXX. XXXX.</span><span class="sxs-lookup"><span data-stu-id="7e28c-104">Your OneDrive version needs to be equal to or greater than version 20.052.XXXX.XXXX.</span></span> <span data-ttu-id="7e28c-105">Untuk memeriksa versi Anda, klik ikon OneDrive biru di area pemberitahuan, pilih **bantuan & pengaturan > pengaturan > tentang**.</span><span class="sxs-lookup"><span data-stu-id="7e28c-105">To check your version, click on the blue OneDrive icon in the notification area, select **Help & Settings > Settings > About**.</span></span>

<span data-ttu-id="7e28c-106">Jaringan Anda mungkin memblokir Traffic ke **g.Live.com** dan **oneclient.SFX.ms**.</span><span class="sxs-lookup"><span data-stu-id="7e28c-106">Your network might block traffic to **g.live.com** and **oneclient.sfx.ms**.</span></span> <span data-ttu-id="7e28c-107">Jika lalu lintas diblokir, OneDrive tidak dapat memperbarui dirinya.</span><span class="sxs-lookup"><span data-stu-id="7e28c-107">If that traffic is blocked, OneDrive cannot update itself.</span></span> <span data-ttu-id="7e28c-108">Bekerja dengan administrator jaringan Anda untuk memastikan Anda memiliki akses ke URL tersebut.</span><span class="sxs-lookup"><span data-stu-id="7e28c-108">Work with your network administrator to ensure you have access to those URLs.</span></span> <span data-ttu-id="7e28c-109">[Titik akhir ini](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) harus dapat dijangkau untuk pelanggan yang menggunakan paket Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7e28c-109">[These endpoints](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) should be reachable for customers using Microsoft 365 plans.</span></span>

<span data-ttu-id="7e28c-110">Jika Anda perlu mendapatkan versi terbaru OneDrive, kunjungi [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .</span><span class="sxs-lookup"><span data-stu-id="7e28c-110">If you need to manually get a current version of OneDrive, visit [https://aka.ms/getonedrive](https://aka.ms/getonedrive).</span></span>
