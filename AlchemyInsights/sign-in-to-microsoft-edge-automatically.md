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
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398732"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="c3da9-102">Masuk ke Microsoft Edge secara otomatis</span><span class="sxs-lookup"><span data-stu-id="c3da9-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="c3da9-103">Microsoft Edge menggunakan akun default OS untuk secara otomatis masuk ke pengguna sesuai dengan bagaimana perangkat pengguna dikonfigurasi.</span><span class="sxs-lookup"><span data-stu-id="c3da9-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="c3da9-104">Skenario setiap tipe konfigurasi perangkat dan proses masuk pengguna dependennya dijelaskan di bawah ini:</span><span class="sxs-lookup"><span data-stu-id="c3da9-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="c3da9-105">**Perangkat adalah hibrid/AAD-J**: Opsi ini tersedia di Windows 10, Windows tingkat bawah, dan versi server yang terkait.</span><span class="sxs-lookup"><span data-stu-id="c3da9-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="c3da9-106">Pengguna secara otomatis masuk dengan akun Azure Active Directory (AD) mereka.</span><span class="sxs-lookup"><span data-stu-id="c3da9-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="c3da9-107">**Perangkat tergabung dalam domain:** Opsi ini tersedia di Windows 10, Windows tingkat bawah, dan versi server yang terkait.</span><span class="sxs-lookup"><span data-stu-id="c3da9-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="c3da9-108">Secara default, pengguna dengan akun domain tidak masuk secara otomatis; untuk mengaktifkan masuk otomatis bagi mereka, gunakan kebijakan **ConfigureOnPremisesAccountAutoSignIn.**</span><span class="sxs-lookup"><span data-stu-id="c3da9-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="c3da9-109">Untuk mengaktifkan masuk otomatis bagi pengguna dengan akun Azure AD, pertimbangkan untuk menggabungkan perangkat mereka dengan hibrid.</span><span class="sxs-lookup"><span data-stu-id="c3da9-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="c3da9-110">Akun default OS adalah akun **Microsoft:** Opsi ini tersedia di Windows 10 RS3 (versi 1709, build 10.0.16299) dan versi yang lebih baru.</span><span class="sxs-lookup"><span data-stu-id="c3da9-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="c3da9-111">Skenario tidak seperti terjadi pada perangkat perusahaan.</span><span class="sxs-lookup"><span data-stu-id="c3da9-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="c3da9-112">Namun, jika akun default OS adalah akun Microsoft, maka Microsoft Edge akan secara otomatis masuk ke pengguna tersebut dengan akun Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c3da9-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
