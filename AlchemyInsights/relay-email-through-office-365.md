---
title: Relay email melalui Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 074a9106553bf3a2a5e563f9ebaca9dfc38111cb
ms.sourcegitcommit: 9872280f71429d2344b0b441e218fba5b3bd3cf7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/02/2020
ms.locfileid: "45023462"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="199aa-102">Menyiapkan perangkat atau aplikasi multifungsi untuk mengirim email</span><span class="sxs-lookup"><span data-stu-id="199aa-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="199aa-103">Untuk mempelajari tentang opsi dan langkah-langkahnya, lihat [Cara menyiapkan perangkat atau aplikasi multifungsi untuk mengirim email menggunakan Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="199aa-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="199aa-104">**Catatan:** Jika perangkat atau aplikasi Anda berhenti berfungsi baru-baru ini, perlu diketahui bahwa kami baru saja memulai rencana kami untuk [menonaktifkan sandi 3DES](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption).</span><span class="sxs-lookup"><span data-stu-id="199aa-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="199aa-105">Untuk melihat perangkat yang terpengaruh, masuk ke [laporan Klien Autentikasi SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="199aa-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="199aa-106">Kesalahan umum mungkin seperti: Kegagalan/kesalahan autentikasi, Kegagalan/kesalahan TLS, Kesalahan algoritma sandi, Ketidakcocokan algoritma, atau Koneksi terputus.</span><span class="sxs-lookup"><span data-stu-id="199aa-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="199aa-107">Untuk mengatasi masalah tersebut:</span><span class="sxs-lookup"><span data-stu-id="199aa-107">To resolve the issue:</span></span>

 - <span data-ttu-id="199aa-108">**Windows Server 2003 IIS SMTP tidak akan berfungsi lagi, diperlukan Windows dengan versi lebih baru.**</span><span class="sxs-lookup"><span data-stu-id="199aa-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="199aa-109">Silakan periksa ke vendor aplikasi atau perangkat untuk melihat jika sandi modern didukung atau jika terdapat pembaruan.</span><span class="sxs-lookup"><span data-stu-id="199aa-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
