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
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/25/2019
ms.locfileid: "36504997"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="966f1-102">Akses bersyarat dengan Intune</span><span class="sxs-lookup"><span data-stu-id="966f1-102">Conditional Access with Intune</span></span>

<span data-ttu-id="966f1-103">Menggunakan **akses bersyarat** dengan Intune memerlukan 3 langkah:</span><span class="sxs-lookup"><span data-stu-id="966f1-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="966f1-104">Buat **kebijakan akses bersyarat** yang menentukan sumber daya apa yang dilindungi, dan kondisi apa yang perlu dipenuhi untuk mengakses sumber daya tersebut.</span><span class="sxs-lookup"><span data-stu-id="966f1-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="966f1-105">Misalnya, perangkat harus kompatibel sebelum mengakses email perusahaan.</span><span class="sxs-lookup"><span data-stu-id="966f1-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="966f1-106">Buat **kebijakan kepatuhan** untuk menentukan pengaturan yang harus dipenuhi sebelum perangkat dianggap sesuai.</span><span class="sxs-lookup"><span data-stu-id="966f1-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="966f1-107">Misalnya, perangkat harus memiliki PIN minimal 6 digit sebelum dianggap sesuai.</span><span class="sxs-lookup"><span data-stu-id="966f1-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="966f1-108">Memastikan **kebijakan kepatuhan** dan **kebijakan akses bersyarat** ditargetkan ke grup pengguna yang diinginkan.</span><span class="sxs-lookup"><span data-stu-id="966f1-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="966f1-109">Ini mungkin memerlukan membuat grup pengguna tertentu di Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="966f1-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="966f1-110">Selengkapnya:</span><span class="sxs-lookup"><span data-stu-id="966f1-110">Read more:</span></span>
  
- [<span data-ttu-id="966f1-111">Praktik terbaik akses bersyarat</span><span class="sxs-lookup"><span data-stu-id="966f1-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="966f1-112">Memulai dengan akses bersyarat</span><span class="sxs-lookup"><span data-stu-id="966f1-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

