---
title: penerusan email 726 memblokir
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219858"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="ce628-102">Memblokir atau membuka blokir penerusan email</span><span class="sxs-lookup"><span data-stu-id="ce628-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="ce628-103">Untuk mengaktifkan atau menonaktifkan penerusan email untuk kotak surat tertentu, lihat [mengonfigurasi penerusan email](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="ce628-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="ce628-104">Pada tingkat penyewa, kontrol pengalihan eksternal dilakukan menggunakan kebijakan anti spam keluar.</span><span class="sxs-lookup"><span data-stu-id="ce628-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="ce628-105">Jika diatur ke nonaktif atau otomatis, mungkin blokir penerusan email dengan kesalahan 550 "akses 5.7.520 ditolak, organisasi Anda tidak memperbolehkan penerusan eksternal".</span><span class="sxs-lookup"><span data-stu-id="ce628-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="ce628-106">Selanjutnya, jika pengalihan diatur ke diblokir, itu adalah kesalahan yang akan dilihat pengguna Anda.</span><span class="sxs-lookup"><span data-stu-id="ce628-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="ce628-107">Jika pengalihan sedang diblokir, pastikan kebijakan dikonfigurasi untuk mengaktifkan penerusan otomatis eksternal.</span><span class="sxs-lookup"><span data-stu-id="ce628-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="ce628-108">Anda dapat memeriksa kebijakan filter spam keluar dari pusat keamanan dan kepatuhan atau dengan menjalankan perintah Get-HostedOutboundSpamFilterPolicy | FL Name, AutoForwardingMode.</span><span class="sxs-lookup"><span data-stu-id="ce628-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="ce628-109">Jika Anda ingin menyetel pemblokiran otomatis, perintah yang sama akan memberi tahu status kebijakan Anda sekarang.</span><span class="sxs-lookup"><span data-stu-id="ce628-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="ce628-110">Catatan: disarankan untuk menyimpan otomatis eksternal yang dinonaktifkan pada kebijakan filter spam keluar default Anda dan mengaktifkannya hanya untuk pengguna yang memerlukan penerusan eksternal dengan membuat kebijakan kustom untuk pengguna tersebut.</span><span class="sxs-lookup"><span data-stu-id="ce628-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="ce628-111">Anda dapat membaca selengkapnya dalam [mengonfigurasi penerusan email eksternal di Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="ce628-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>