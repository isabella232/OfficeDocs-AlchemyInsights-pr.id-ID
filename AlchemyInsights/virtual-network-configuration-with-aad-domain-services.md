---
title: Konfigurasi virtual dengan layanan domain AAD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885205"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="7de1f-102">Konfigurasi virtual dengan layanan domain AAD</span><span class="sxs-lookup"><span data-stu-id="7de1f-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="7de1f-103">Konfigurasi virtual dengan layanan domain AAD melibatkan langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="7de1f-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="7de1f-104">Memeriksa kesehatan domain Anda di portal Azure https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="7de1f-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="7de1f-105">Memeriksa NSG Anda untuk aturan yang memblokir port yang diperlukan untuk menyinkronkan di layanan domain Azure AD pada portal https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="7de1f-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="7de1f-106">Memastikan bahwa jaringan virtual Anda disebarkan di kawasan Azure yang sama dengan domain Azure AD domain terkelola layanan Anda.</span><span class="sxs-lookup"><span data-stu-id="7de1f-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="7de1f-107">Memastikan Anda tidak memiliki domain yang ada dengan nama domain yang sama yang tersedia di jaringan virtual.</span><span class="sxs-lookup"><span data-stu-id="7de1f-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="7de1f-108">Untuk detail selengkapnya tentang pertimbangan desain pada jaringan virtual Azure untuk mendukung layanan domain AAD, lihat [pertimbangan jaringan virtual](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span><span class="sxs-lookup"><span data-stu-id="7de1f-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

