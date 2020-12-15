---
title: Masuk ke Microsoft Edge secara otomatis
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677766"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="c47ed-102">Masuk ke Microsoft Edge secara otomatis</span><span class="sxs-lookup"><span data-stu-id="c47ed-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="c47ed-103">Microsoft Edge menggunakan akun default OS untuk secara otomatis memasukkan pengguna sesuai dengan cara perangkat pengguna dikonfigurasi.</span><span class="sxs-lookup"><span data-stu-id="c47ed-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="c47ed-104">Skenario setiap tipe konfigurasi perangkat dan proses masuk pengguna dependen diuraikan di bawah ini:</span><span class="sxs-lookup"><span data-stu-id="c47ed-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="c47ed-105">**Perangkat ini hibrid/AAD-J**: opsi ini tersedia di Windows 10, Windows tingkat bawah, dan versi server terkait.</span><span class="sxs-lookup"><span data-stu-id="c47ed-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="c47ed-106">Pengguna secara otomatis masuk dengan akun Azure Active Directory (AD) mereka.</span><span class="sxs-lookup"><span data-stu-id="c47ed-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="c47ed-107">**Perangkat ini tergabung dalam domain**: opsi ini tersedia di Windows 10, Windows tingkat bawah, dan versi server terkait.</span><span class="sxs-lookup"><span data-stu-id="c47ed-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="c47ed-108">Secara default, pengguna dengan akun domain tidak masuk secara otomatis; untuk mengaktifkan masuk otomatis bagi mereka, gunakan kebijakan **Configureonpremisesaccountautosignin** .</span><span class="sxs-lookup"><span data-stu-id="c47ed-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="c47ed-109">Untuk mengaktifkan masuk otomatis bagi pengguna dengan akun Azure AD, pertimbangkan hibrid-bergabung dengan perangkat mereka.</span><span class="sxs-lookup"><span data-stu-id="c47ed-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="c47ed-110">**Akun default OS adalah akun Microsoft**: opsi ini tersedia di Windows 10 RS3 (versi 1709, Build 10.0.16299) dan versi yang lebih baru.</span><span class="sxs-lookup"><span data-stu-id="c47ed-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="c47ed-111">Skenario tidak mungkin terjadi pada perangkat perusahaan.</span><span class="sxs-lookup"><span data-stu-id="c47ed-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="c47ed-112">Namun, jika akun default OS adalah akun Microsoft, maka Microsoft Edge akan secara otomatis masuk ke pengguna dengan akun Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c47ed-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
