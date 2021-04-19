---
title: Mengatasi kesalahan masuk Teams AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821990"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="f97d2-102">Mengatasi kesalahan masuk Teams AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="f97d2-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="f97d2-103">Ketika masuk ke Microsoft Teams, Anda mungkin akan menerima kesalahan: Maaf, tetapi kami mengalami masalah dengan penandatanganan Anda di **AADSTS9000411: Permintaan tidak diformat dengan benar. Parameter "login_hint" diduplikasi.**</span><span class="sxs-lookup"><span data-stu-id="f97d2-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="f97d2-104">Untuk mengatasi masalah ini, pastikan klien Microsoft Teams Anda diperbarui.</span><span class="sxs-lookup"><span data-stu-id="f97d2-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="f97d2-105">Untuk informasi selengkapnya tentang memperbarui klien, lihat [Memperbarui Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="f97d2-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="f97d2-106">Jika Anda tidak bisa memperbarui klien Anda karena beberapa alasan, keluar dari klien akan menghapus sebagian besar data singgahan.</span><span class="sxs-lookup"><span data-stu-id="f97d2-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="f97d2-107">Namun, jika masih mengalami masalah setelah logoff/masuk, keluar dari Teams dan hapus cache klien dengan melakukan hal berikut:</span><span class="sxs-lookup"><span data-stu-id="f97d2-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="f97d2-108">Tutup Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f97d2-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="f97d2-109">Masuk ke: %appdata%\microsoft\teams dan hapus semua file.</span><span class="sxs-lookup"><span data-stu-id="f97d2-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="f97d2-110">Buka kembali Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f97d2-110">Reopen Microsoft Teams.</span></span>
