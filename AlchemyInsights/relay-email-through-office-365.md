---
title: Relay email melalui Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 56936541c52e56d7aa9b0f5dad7b9a359c5b6185
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809658"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="8a370-102">Menyiapkan perangkat atau aplikasi multifungsi untuk mengirim email</span><span class="sxs-lookup"><span data-stu-id="8a370-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="8a370-103">Untuk mempelajari tentang opsi dan langkah-langkahnya, lihat [Cara menyiapkan perangkat atau aplikasi multifungsi untuk mengirim email menggunakan Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="8a370-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="8a370-104">**Catatan:** Jika perangkat atau aplikasi Anda berhenti berfungsi baru-baru ini, perlu diketahui bahwa kami baru saja memulai rencana kami untuk [menonaktifkan sandi 3DES](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption).</span><span class="sxs-lookup"><span data-stu-id="8a370-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="8a370-105">Untuk melihat perangkat yang terpengaruh, masuk ke [laporan Klien Autentikasi SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="8a370-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="8a370-106">Kesalahan umum mungkin seperti: Kegagalan/kesalahan autentikasi, Kegagalan/kesalahan TLS, Kesalahan algoritma sandi, Ketidakcocokan algoritma, atau Koneksi terputus.</span><span class="sxs-lookup"><span data-stu-id="8a370-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="8a370-107">Untuk mengatasi masalah tersebut:</span><span class="sxs-lookup"><span data-stu-id="8a370-107">To resolve the issue:</span></span>

 - <span data-ttu-id="8a370-108">**Windows Server 2003 IIS SMTP tidak akan berfungsi lagi, diperlukan Windows dengan versi lebih baru.**</span><span class="sxs-lookup"><span data-stu-id="8a370-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="8a370-109">Silakan periksa ke vendor aplikasi atau perangkat untuk melihat jika sandi modern didukung atau jika terdapat pembaruan.</span><span class="sxs-lookup"><span data-stu-id="8a370-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
