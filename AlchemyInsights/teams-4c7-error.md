---
title: Kesalahan Teams 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786672"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="0e69d-102">Kesalahan 4c7 di Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="0e69d-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="0e69d-103">Kesalahan ini terjadi karena Microsoft Teams memerlukan Autentikasi Forms.</span><span class="sxs-lookup"><span data-stu-id="0e69d-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="0e69d-104">Ketika Anda menggunakan Active Directory Federation Services (AD FS), Autentikasi Formulir tidak diaktifkan untuk intranet secara default.</span><span class="sxs-lookup"><span data-stu-id="0e69d-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="0e69d-105">Jika Autentikasi Terpadu Windows gagal, Anda akan diminta untuk masuk menggunakan Autentikasi Forms.</span><span class="sxs-lookup"><span data-stu-id="0e69d-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="0e69d-106">Untuk mengatasi masalah ini, aktifkan Autentikasi Forms dengan menggunakan snap-in KONSOL Manajemen Microsoft (MMC) AD FS di komputer yang memiliki salinan lokal Direktori Aktif.</span><span class="sxs-lookup"><span data-stu-id="0e69d-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="0e69d-107">Untuk melakukan ini, ikuti langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="0e69d-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="0e69d-108">Di panel navigasi, telusuri ke **Kebijakan Autentikasi.**</span><span class="sxs-lookup"><span data-stu-id="0e69d-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="0e69d-109">Di **bawah Tindakan** di panel detail, pilih Edit **Autentikasi Utama Global.**</span><span class="sxs-lookup"><span data-stu-id="0e69d-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="0e69d-110">Pada tab **Intranet,** pilih **Autentikasi Formulir**.</span><span class="sxs-lookup"><span data-stu-id="0e69d-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="0e69d-111">Pilih **OK** (atau **Terapkan**).</span><span class="sxs-lookup"><span data-stu-id="0e69d-111">Select **OK** (or **Apply**).</span></span>