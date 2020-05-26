---
title: Mengatasi kesalahan tim sign-in AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357878"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="e2d91-102">Mengatasi kesalahan tim sign-in AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="e2d91-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="e2d91-103">Saat masuk ke Microsoft teams, Anda mungkin menerima pesan kesalahan: **Maaf, namun kami mengalami masalah saat masuk ke AADSTS9000411: permintaan tidak diformat dengan benar. Parameter "login_hint" diduplikasi.**</span><span class="sxs-lookup"><span data-stu-id="e2d91-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="e2d91-104">Untuk mengatasi masalah ini, pastikan klien Microsoft teams Anda diperbarui.</span><span class="sxs-lookup"><span data-stu-id="e2d91-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="e2d91-105">Untuk informasi lebih lanjut tentang cara memperbarui klien, lihat [memperbarui Microsoft teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="e2d91-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="e2d91-106">Jika Anda tidak dapat memperbarui klien Anda untuk beberapa alasan, logoff klien akan menghapus sebagian besar data yang disimpan dalam cache.</span><span class="sxs-lookup"><span data-stu-id="e2d91-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="e2d91-107">Namun, jika Anda masih mengalami masalah setelah logoff/logon, tutup tim dan Kosongkan tembolok klien Anda dengan melakukan hal berikut:</span><span class="sxs-lookup"><span data-stu-id="e2d91-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="e2d91-108">Tutup Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="e2d91-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="e2d91-109">Pergi ke:%AppData%\microsoft\teams dan menghapus semua berkas.</span><span class="sxs-lookup"><span data-stu-id="e2d91-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="e2d91-110">Buka kembali Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="e2d91-110">Reopen Microsoft Teams.</span></span>
