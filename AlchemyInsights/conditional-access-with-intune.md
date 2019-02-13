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
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/12/2019
ms.locfileid: "29935941"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="f344f-102">Akses bersyarat dengan Intune</span><span class="sxs-lookup"><span data-stu-id="f344f-102">Conditional Access with Intune</span></span>

<span data-ttu-id="f344f-103">Menggunakan **Akses bersyarat** dengan Intune membutuhkan 3 langkah:</span><span class="sxs-lookup"><span data-stu-id="f344f-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="f344f-p101">Membuat **Kebijakan akses bersyarat** yang mendefinisikan apa yang sumber daya yang dilindungi, dan kondisi apa yang harus dipenuhi untuk mengakses sumber daya tersebut. Sebagai contoh, perangkat harus memenuhi persyaratan sebelum mengakses email perusahaan.</span><span class="sxs-lookup"><span data-stu-id="f344f-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="f344f-p102">Membuat **Kebijakan kepatuhan** untuk menentukan pengaturan yang harus dipenuhi sebelum perangkat dianggap sesuai. Sebagai contoh, perangkat harus memiliki setidaknya 6 digit pin sebelum itu dianggap sesuai.</span><span class="sxs-lookup"><span data-stu-id="f344f-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="f344f-p103">Memastikan **Kepatuhan kebijakan** dan **Kebijakan akses bersyarat** ditargetkan untuk kelompok pengguna yang diinginkan. Ini mungkin membutuhkan menciptakan grup pengguna tertentu di Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f344f-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="f344f-110">Baca lebih lanjut:</span><span class="sxs-lookup"><span data-stu-id="f344f-110">Read more:</span></span>
  
- [<span data-ttu-id="f344f-111">Akses bersyarat praktik terbaik</span><span class="sxs-lookup"><span data-stu-id="f344f-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="f344f-112">Memulai dengan akses bersyarat</span><span class="sxs-lookup"><span data-stu-id="f344f-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

