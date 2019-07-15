---
title: Relay email melalui Office 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 9/21/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3c056f5c78935adcf0b64779f9632f9336080a40
ms.sourcegitcommit: dce9cf9bb05d29f0f9bab61fe3fc25e99f0cebf1
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 07/11/2019
ms.locfileid: "35630744"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email-using-office-365"></a><span data-ttu-id="29abb-102">Menyiapkan perangkat atau aplikasi multifungsi untuk mengirimkan email menggunakan Office 365</span><span class="sxs-lookup"><span data-stu-id="29abb-102">Set up a multifunction device or application to send email using Office 365</span></span>

<span data-ttu-id="29abb-103">Untuk mempelajari tentang opsi dan langkah-langkahnya, lihat [Cara menyiapkan perangkat atau aplikasi multifungsi untuk mengirimkan email menggunakan Office 365](https://support.office.com/article/69f58e99-c550-4274-ad18-c805d654b4c4).</span><span class="sxs-lookup"><span data-stu-id="29abb-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Office 365](https://support.office.com/article/69f58e99-c550-4274-ad18-c805d654b4c4).</span></span>
  
<span data-ttu-id="29abb-104">**Catatan:** Jika perangkat atau aplikasi Anda baru-baru ini berhenti berfungsi, harap diperhatikan kami baru-baru ini mulai [menonaktifkan sandi 3DES](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) sesuai rencana.</span><span class="sxs-lookup"><span data-stu-id="29abb-104">**Note:** If you have a device or application which recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="29abb-105">Untuk melihat perangkat yang terpengaruh, masuk ke [laporan Klien Autentikasi SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="29abb-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="29abb-106">Kesalahan umum mungkin seperti: Kegagalan/kesalahan autentikasi, Kegagalan/kesalahan TLS, Kesalahan algoritma sandi, Ketidakcocokan algoritma, atau Koneksi terputus.</span><span class="sxs-lookup"><span data-stu-id="29abb-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="29abb-107">Untuk mengatasi masalah tersebut:</span><span class="sxs-lookup"><span data-stu-id="29abb-107">To resolve the issue:</span></span>
 - <span data-ttu-id="29abb-108">**Windows Server 2003 IIS SMTP tidak akan berfungsi lagi, diperlukan Windows dengan versi lebih baru.**</span><span class="sxs-lookup"><span data-stu-id="29abb-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="29abb-109">Silakan periksa ke vendor aplikasi atau perangkat untuk melihat jika sandi modern didukung atau jika terdapat pembaruan.</span><span class="sxs-lookup"><span data-stu-id="29abb-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
