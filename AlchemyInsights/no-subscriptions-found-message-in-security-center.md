---
title: Tidak ada pesan langganan yang ditemukan di Pusat Keamanan
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544111"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="14ddf-102">Tidak ada pesan langganan yang ditemukan di Pusat Keamanan</span><span class="sxs-lookup"><span data-stu-id="14ddf-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="14ddf-103">Jika saat Pusat Keamanan Pertahanan Microsoft Anda mendapatkan pesan "Langganan tidak ditemukan", artinya Azure Active Directory (AAD) yang digunakan untuk masuk ke portal tidak memiliki ATP Pertahanan Microsoft mereka.</span><span class="sxs-lookup"><span data-stu-id="14ddf-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="14ddf-104">Lisensi Windows E5 dan Office E5 merupakan lisensi terpisah.</span><span class="sxs-lookup"><span data-stu-id="14ddf-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="14ddf-105">Buka kasus dukungan jika lisensi dibeli tetapi tidak ditetapkan pada instans AAD ini.</span><span class="sxs-lookup"><span data-stu-id="14ddf-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="14ddf-106">Anda memiliki:</span><span class="sxs-lookup"><span data-stu-id="14ddf-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="14ddf-107">Kemungkinan masalah penyediaan lisensi.</span><span class="sxs-lookup"><span data-stu-id="14ddf-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="14ddf-108">Anda tidak sengaja menyediakan lisensi ke Microsoft AAD berbeda dari yang digunakan untuk autentikasi ke dalam layanan.</span><span class="sxs-lookup"><span data-stu-id="14ddf-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>