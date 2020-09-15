---
title: Kesalahan teams 4c7
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700206"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="6188f-102">kesalahan 4c7 di Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="6188f-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="6188f-103">Kesalahan ini terjadi karena Microsoft teams memerlukan autentikasi formulir.</span><span class="sxs-lookup"><span data-stu-id="6188f-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="6188f-104">Saat Anda menggunakan Active Directory Federation Services (AD FS), autentikasi formulir tidak diaktifkan untuk intranet secara default.</span><span class="sxs-lookup"><span data-stu-id="6188f-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="6188f-105">Jika autentikasi Terpadu Windows gagal, Anda akan diminta untuk masuk menggunakan autentikasi formulir.</span><span class="sxs-lookup"><span data-stu-id="6188f-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="6188f-106">Untuk mengatasi masalah ini, Aktifkan autentikasi formulir dengan menggunakan snap-in konsol manajemen Microsoft (MMC) AD FS di komputer yang memiliki salinan direktori aktif lokal.</span><span class="sxs-lookup"><span data-stu-id="6188f-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="6188f-107">Untuk melakukan ini, ikuti langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="6188f-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="6188f-108">Di panel navigasi, telusuri ke **kebijakan autentikasi**.</span><span class="sxs-lookup"><span data-stu-id="6188f-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="6188f-109">Di bawah **tindakan** di panel detail, pilih **Edit autentikasi utama global**.</span><span class="sxs-lookup"><span data-stu-id="6188f-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="6188f-110">Pada tab **intranet** , pilih **autentikasi formulir**.</span><span class="sxs-lookup"><span data-stu-id="6188f-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="6188f-111">Pilih **OK** (atau **Terapkan**).</span><span class="sxs-lookup"><span data-stu-id="6188f-111">Select **OK** (or **Apply**).</span></span>