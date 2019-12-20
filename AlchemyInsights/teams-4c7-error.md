---
title: Tim 4c7 kesalahan
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796184"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="5da53-102">galat 4c7 di Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="5da53-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="5da53-103">Galat ini terjadi karena Microsoft teams memerlukan otentikasi formulir.</span><span class="sxs-lookup"><span data-stu-id="5da53-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="5da53-104">Ketika Anda menggunakan Active Directory Federation Services (AD FS), otentikasi formulir tidak diaktifkan untuk intranet secara default.</span><span class="sxs-lookup"><span data-stu-id="5da53-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="5da53-105">Jika otentikasi Terpadu Windows gagal, Anda diminta untuk masuk menggunakan otentikasi formulir.</span><span class="sxs-lookup"><span data-stu-id="5da53-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="5da53-106">Untuk mengatasi masalah ini, aktifkan otentikasi formulir dengan menggunakan AD FS konsol manajemen Microsoft (MMC) snap-in di komputer yang memiliki salinan lokal direktori aktif.</span><span class="sxs-lookup"><span data-stu-id="5da53-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="5da53-107">Untuk melakukan ini, ikuti langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="5da53-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="5da53-108">Di panel navigasi, Jelajahi **kebijakan otentikasi**.</span><span class="sxs-lookup"><span data-stu-id="5da53-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="5da53-109">Di bawah **tindakan** di panel rincian, pilih **mengedit otentikasi utama global**.</span><span class="sxs-lookup"><span data-stu-id="5da53-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="5da53-110">Pada tab **intranet** , pilih **bentuk otentikasi**.</span><span class="sxs-lookup"><span data-stu-id="5da53-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="5da53-111">Pilih **OK** (atau **Terapkan**).</span><span class="sxs-lookup"><span data-stu-id="5da53-111">Select **OK** (or **Apply**).</span></span>