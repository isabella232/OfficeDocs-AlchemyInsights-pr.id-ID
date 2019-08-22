---
title: Akses bersyarat dengan Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/22/2019
ms.locfileid: "36504997"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="59aa1-102">Akses bersyarat dengan Intune</span><span class="sxs-lookup"><span data-stu-id="59aa1-102">Conditional Access with Intune</span></span>

<span data-ttu-id="59aa1-103">Menggunakan **Akses bersyarat** dengan Intune membutuhkan 3 langkah:</span><span class="sxs-lookup"><span data-stu-id="59aa1-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="59aa1-104">Membuat **Kebijakan akses bersyarat** yang mendefinisikan apa yang sumber daya yang dilindungi, dan kondisi apa yang harus dipenuhi untuk mengakses sumber daya tersebut.</span><span class="sxs-lookup"><span data-stu-id="59aa1-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="59aa1-105">Sebagai contoh, perangkat harus memenuhi persyaratan sebelum mengakses email perusahaan.</span><span class="sxs-lookup"><span data-stu-id="59aa1-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="59aa1-106">Membuat **Kebijakan kepatuhan** untuk menentukan pengaturan yang harus dipenuhi sebelum perangkat dianggap sesuai.</span><span class="sxs-lookup"><span data-stu-id="59aa1-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="59aa1-107">Sebagai contoh, perangkat harus memiliki setidaknya 6 digit pin sebelum itu dianggap sesuai.</span><span class="sxs-lookup"><span data-stu-id="59aa1-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="59aa1-108">Memastikan **Kepatuhan kebijakan** dan **Kebijakan akses bersyarat** ditargetkan untuk kelompok pengguna yang diinginkan.</span><span class="sxs-lookup"><span data-stu-id="59aa1-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="59aa1-109">Ini mungkin membutuhkan menciptakan grup pengguna tertentu di Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="59aa1-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="59aa1-110">Baca lebih lanjut:</span><span class="sxs-lookup"><span data-stu-id="59aa1-110">Read more:</span></span>
  
- [<span data-ttu-id="59aa1-111">Akses bersyarat praktik terbaik</span><span class="sxs-lookup"><span data-stu-id="59aa1-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="59aa1-112">Memulai dengan akses bersyarat</span><span class="sxs-lookup"><span data-stu-id="59aa1-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

