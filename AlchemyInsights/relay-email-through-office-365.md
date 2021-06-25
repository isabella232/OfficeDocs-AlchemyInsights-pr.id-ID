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
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117986"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="0a4be-102">Menyiapkan perangkat atau aplikasi multifungsi untuk mengirim email</span><span class="sxs-lookup"><span data-stu-id="0a4be-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="0a4be-103">Untuk mempelajari tentang opsi dan langkah-langkahnya, lihat [Cara menyiapkan perangkat atau aplikasi multifungsi untuk mengirim email menggunakan Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="0a4be-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="0a4be-104">Jika Anda memiliki perangkat atau aplikasi yang baru saja berhenti bekerja, masalah paling umum adalah:</span><span class="sxs-lookup"><span data-stu-id="0a4be-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="0a4be-105">**Autentikasi terkait kesalahan saat menggunakan pengiriman klien SMTP Auth** Baru-baru ini kami membuat beberapa perubahan terkait cara kerja Autentikasi SMTP.</span><span class="sxs-lookup"><span data-stu-id="0a4be-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="0a4be-106">Untuk informasi selengkapnya tentang cara mengatasi masalah, lihat bagian autentikasi yang tidak berhasil dari Memperbaiki masalah [dengan printer, pemindai,](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)dan aplikasi LOB yang mengirim email menggunakan Microsoft 365 atau Office 365 .</span><span class="sxs-lookup"><span data-stu-id="0a4be-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="0a4be-107">**Kami hanya menerima versi TLS 1.2 saat membuat koneksi yang aman ke Office 365** Jika menggunakan Koneksi aman (TLS), pastikan perangkat aplikasi Mendukung TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="0a4be-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="0a4be-108">Untuk informasi selengkapnya, lihat [Mempersiapkan TLS 1.2 di Office 365 dan Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="0a4be-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="0a4be-109">Untuk masalah dan solusi lainnya, lihat Memperbaiki masalah [dengan printer, pemindai,](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)dan aplikasi LOB yang mengirim email menggunakan Microsoft 365 atau Office 365 .</span><span class="sxs-lookup"><span data-stu-id="0a4be-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="0a4be-110">Untuk melihat perangkat yang terpengaruh, masuk ke [laporan Klien Autentikasi SMTP](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="0a4be-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="0a4be-111">**Catatan**: Exchange Online tidak mengakomodasi skenario surat massal.</span><span class="sxs-lookup"><span data-stu-id="0a4be-111">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios.</span></span> <span data-ttu-id="0a4be-112">Untuk mengirim email komersial massal (misalnya, buletin pelanggan), Anda harus menggunakan penyedia pihak ketiga yang mengkhususkan dalam layanan ini.</span><span class="sxs-lookup"><span data-stu-id="0a4be-112">To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
