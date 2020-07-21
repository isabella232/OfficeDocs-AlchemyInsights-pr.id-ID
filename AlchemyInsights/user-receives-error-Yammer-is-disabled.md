---
title: Pengguna menerima galat AADSTS7000112 Yammer dinonaktifkan
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198056"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="4fd64-102">Pengguna menerima galat AADSTS7000112 Yammer dinonaktifkan</span><span class="sxs-lookup"><span data-stu-id="4fd64-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="4fd64-103">Jika Anda menerima galat "AADSTS7000112: Application ' 00000005-0000-0ff1-ce00-000000000000 ' (heboh) dinonaktifkan", ada masalah dengan prinsipal layanan dalam Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4fd64-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="4fd64-104">Administrator mungkin telah dinonaktifkan prinsip layanan untuk memblokir akses ke Yammer.</span><span class="sxs-lookup"><span data-stu-id="4fd64-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="4fd64-105">Menonaktifkan pimpinan Layanan tidak disarankan dan dapat menyebabkan masalah tambahan.</span><span class="sxs-lookup"><span data-stu-id="4fd64-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="4fd64-106">Untuk informasi lebih lanjut tentang pendekatan yang didukung untuk memblokir akses pengguna ke heboh, lihat [mematikan heboh akses untuk Microsoft 365 pengguna](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="4fd64-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="4fd64-107">Untuk memperbaiki masalah ini di Azure portal dan memulihkan akses pengguna ke Yammer:</span><span class="sxs-lookup"><span data-stu-id="4fd64-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="4fd64-108">Buka halaman Azure Active Directory, dan pilih **aplikasi Enterprise** di bawah **Kelola** di panel navigasi kiri.</span><span class="sxs-lookup"><span data-stu-id="4fd64-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="4fd64-109">Ketik **Office 365 heboh** di kotak pencarian, dan pilih nama aplikasi untuk membuka pengaturan.</span><span class="sxs-lookup"><span data-stu-id="4fd64-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="4fd64-110">Pilih **properti** di bawah **Kelola** di panel navigasi kiri.</span><span class="sxs-lookup"><span data-stu-id="4fd64-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="4fd64-111">Tetapkan nilai **diaktifkan bagi pengguna untuk masuk?** untuk **ya**, dan kemudian pilih **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="4fd64-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="4fd64-112">Masuk ke heboh lagi.</span><span class="sxs-lookup"><span data-stu-id="4fd64-112">Sign in to Yammer again.</span></span> <span data-ttu-id="4fd64-113">Anda mungkin perlu menghapus cookie.</span><span class="sxs-lookup"><span data-stu-id="4fd64-113">You might need to clear cookies.</span></span>

<span data-ttu-id="4fd64-114">Selain itu, jalankan perintah PowerShell untuk menetapkan nilai.</span><span class="sxs-lookup"><span data-stu-id="4fd64-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="4fd64-115">Untuk informasi lebih lanjut, lihat ["Maaf, tapi kami mengalami masalah saat masuk Anda" kesalahan ketika Anda mengklik ubin heboh di Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="4fd64-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 