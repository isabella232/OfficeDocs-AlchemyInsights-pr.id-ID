---
title: Masalah dengan grup keamanan
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177497"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="73a23-102">Masalah dengan grup keamanan</span><span class="sxs-lookup"><span data-stu-id="73a23-102">Issue with security groups</span></span>

<span data-ttu-id="73a23-103">**Jika Anda mendapatkan kesalahan jaringan AADDS104**</span><span class="sxs-lookup"><span data-stu-id="73a23-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="73a23-104">Aturan grup keamanan jaringan tidak valid adalah penyebab paling umum kesalahan jaringan untuk layanan domain Azure Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="73a23-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="73a23-105">Grup keamanan jaringan untuk jaringan virtual harus mengizinkan akses ke Port dan protokol tertentu.</span><span class="sxs-lookup"><span data-stu-id="73a23-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="73a23-106">Jika port tersebut diblokir, platform Azure tidak bisa memantau atau memperbarui domain terkelola.</span><span class="sxs-lookup"><span data-stu-id="73a23-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="73a23-107">Sinkronisasi antara Azure AD dan Azure AD DS juga terpengaruh.</span><span class="sxs-lookup"><span data-stu-id="73a23-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="73a23-108">Pastikan port default tetap terbuka untuk menghindari gangguan dalam layanan.</span><span class="sxs-lookup"><span data-stu-id="73a23-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="73a23-109">Untuk memahami dan mengatasi masalah umum untuk masalah konfigurasi grup keamanan jaringan, lihat [menambahkan dan memverifikasi grup keamanan](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span><span class="sxs-lookup"><span data-stu-id="73a23-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
