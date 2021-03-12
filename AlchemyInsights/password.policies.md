---
title: Kebijakan kata sandi
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744988"
---
# <a name="password-policies"></a><span data-ttu-id="854ff-102">Kebijakan kata sandi</span><span class="sxs-lookup"><span data-stu-id="854ff-102">Password policies</span></span>

<span data-ttu-id="854ff-103">**Saya mengalami masalah dengan kebijakan kata sandi untuk pengguna**</span><span class="sxs-lookup"><span data-stu-id="854ff-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="854ff-104">Kebijakan kata sandi untuk pengguna bergantung pada apakah pengguna hanya Cloud atau di tempat.</span><span class="sxs-lookup"><span data-stu-id="854ff-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="854ff-105">Hanya pengguna awan harus memilih kata sandi yang memenuhi persyaratan dalam artikel ini: [kebijakan kata sandi yang hanya berlaku untuk akun pengguna awan](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="854ff-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="854ff-106">Pengguna di tempat harus memilih kata sandi yang memenuhi persyaratan di tempat.</span><span class="sxs-lookup"><span data-stu-id="854ff-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="854ff-107">Jika pengguna lokal tidak dapat mengatur kata sandinya, periksa persyaratan lokal Anda.</span><span class="sxs-lookup"><span data-stu-id="854ff-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="854ff-108">**Saya tidak tahu cara mengatur atau memeriksa kebijakan kedaluwarsa kata sandi**</span><span class="sxs-lookup"><span data-stu-id="854ff-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="854ff-109">Anda dapat mengatur dan memeriksa kebijakan kedaluwarsa untuk pengguna awan dalam penyewa Anda menggunakan PowerShell.</span><span class="sxs-lookup"><span data-stu-id="854ff-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="854ff-110">Ikuti instruksi dalam artikel ini: [mengatur atau memeriksa kebijakan kata sandi menggunakan PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="854ff-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="854ff-111">Kebijakan kedaluwarsa kata sandi untuk pengguna di tempat diatur di iklan lokal Anda.</span><span class="sxs-lookup"><span data-stu-id="854ff-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="854ff-112">**Link bermanfaat lainnya:**</span><span class="sxs-lookup"><span data-stu-id="854ff-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="854ff-113">Mulai menggunakan pengaturan ulang kata sandi</span><span class="sxs-lookup"><span data-stu-id="854ff-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="854ff-114">Memecahkan masalah penyetelan ulang kata sandi yang dimulai administrator</span><span class="sxs-lookup"><span data-stu-id="854ff-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
