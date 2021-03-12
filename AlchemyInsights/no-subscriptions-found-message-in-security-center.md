---
title: Tidak ditemukan pesan langganan di pusat keamanan
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
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "50713957"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="38207-102">Tidak ditemukan pesan langganan di pusat keamanan</span><span class="sxs-lookup"><span data-stu-id="38207-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="38207-103">Jika saat mengakses pusat keamanan Microsoft Defender Anda mendapatkan pesan "tidak ada langganan ditemukan", artinya Azure Active Directory (AAD) yang digunakan untuk masuk ke Portal tidak memiliki lisensi Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="38207-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="38207-104">Lisensi Windows E5 dan Office E5 adalah lisensi terpisah.</span><span class="sxs-lookup"><span data-stu-id="38207-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="38207-105">Membuka kasus dukungan jika lisensi dibeli tetapi tidak ditetapkan ke instans AAD ini.</span><span class="sxs-lookup"><span data-stu-id="38207-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="38207-106">Anda memiliki:</span><span class="sxs-lookup"><span data-stu-id="38207-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="38207-107">Kemungkinan masalah penyediaan lisensi.</span><span class="sxs-lookup"><span data-stu-id="38207-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="38207-108">Anda tidak sengaja menetapkan lisensi ke Microsoft AAD yang berbeda dari yang digunakan untuk autentikasi ke layanan.</span><span class="sxs-lookup"><span data-stu-id="38207-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>