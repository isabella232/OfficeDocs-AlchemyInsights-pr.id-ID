---
title: Sinkronisasi UPN dinonaktifkan
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: f390d659b191fa4c44bd7c8acb32409cd3021489
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36532334"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="d01f1-102">Sinkronisasi UPN dinonaktifkan</span><span class="sxs-lookup"><span data-stu-id="d01f1-102">UPN sync disabled</span></span>

<span data-ttu-id="d01f1-103">Jika Anda memulai sinkronisasi Azure iklan sebelum 30 Maret 2016, Jalankan cmdlet Azure iklan PowerShell berikut untuk mengaktifkan UPN lembut cocok untuk organisasi Anda hanya:</span><span class="sxs-lookup"><span data-stu-id="d01f1-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="d01f1-104">**Set-MsolDirSyncFeature-fitur EnableSoftMatchOnUpn-mengaktifkan $True**</span><span class="sxs-lookup"><span data-stu-id="d01f1-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="d01f1-105">UPN lembut pertandingan secara otomatis diaktifkan untuk organisasi yang mulai sinkronisasi Azure iklan pada atau setelah tanggal 30 Maret 2016.</span><span class="sxs-lookup"><span data-stu-id="d01f1-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="d01f1-106">Untuk mempelajari lebih lanjut tentang mengaktifkan lembut cocok pada UPN dan fitur sinkronisasi lainnya, silakan lihat [Azure iklan menyambung sinkronisasi Layanan fitur](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="d01f1-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

