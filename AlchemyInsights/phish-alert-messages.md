---
title: 2491 Peringatkan pesan email dari kebijakan 'Pengelabuan Dikirim karena penyewa atau pengesamping pengguna'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544581"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="b8e38-102">Memberitahukan pesan email dari kebijakan 'Pengelabuan Dikirim karena penyewa atau pengesampuan pengguna'</span><span class="sxs-lookup"><span data-stu-id="b8e38-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="b8e38-103">Kebijakan pemberitahuan default bernama "Phish Delivered due to tenant or user override" telah diluncurkan kepada penyewa dengan Pertahanan Microsoft untuk lisensi Office 365 P1 dan P2.</span><span class="sxs-lookup"><span data-stu-id="b8e38-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="b8e38-104">Jika Anda menerima pemberitahuan ini, berikut langkah-langkah untuk menyelidikinya:</span><span class="sxs-lookup"><span data-stu-id="b8e38-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="b8e38-105">Dari pesan pemberitahuan, klik **Tampilkan Pemberitahuan** untuk masuk ke **halaman Pemberitahuan** di Pusat & Kepatuhan.</span><span class="sxs-lookup"><span data-stu-id="b8e38-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="b8e38-106">Pilih pemberitahuan untuk melihat opsi Tampilkan daftar **pesan atau** Tampilkan pesan **di Explorer**.</span><span class="sxs-lookup"><span data-stu-id="b8e38-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="b8e38-107">Kedua opsi ini membawa Anda ke detail pesan, yang mencakup ID Pesan.</span><span class="sxs-lookup"><span data-stu-id="b8e38-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="b8e38-108">Perhatikan bahwa link Threat Explorer akan otomatis memfilter pesan yang cocok dengan kriteria pemberitahuan.</span><span class="sxs-lookup"><span data-stu-id="b8e38-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="b8e38-109">Anda mungkin perlu menyesuaikan filter tanggal di Threat Explorer.</span><span class="sxs-lookup"><span data-stu-id="b8e38-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="b8e38-110">Pesan pengelabuan (phishing) dikirimkan karena pengelabuan yang dikonfigurasi secara manual:</span><span class="sxs-lookup"><span data-stu-id="b8e38-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="b8e38-111">Pengirim atau kumpulan domain yang diperbolehkan oleh pengguna.</span><span class="sxs-lookup"><span data-stu-id="b8e38-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="b8e38-112">Pengirim atau domain yang diperbolehkan diatur oleh admin dalam kebijakan anti spam.</span><span class="sxs-lookup"><span data-stu-id="b8e38-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="b8e38-113">Alamat IP yang diperbolehkan dalam kebijakan filter koneksi.</span><span class="sxs-lookup"><span data-stu-id="b8e38-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="b8e38-114">Aturan aliran email (juga dikenal sebagai aturan transpor) yang dikonfigurasi untuk mengizinkan pesan masuk.</span><span class="sxs-lookup"><span data-stu-id="b8e38-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="b8e38-115">Jika Anda yakin bahwa pesan tidak ditandai sebagai pengelabuan (phish), gunakan [add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) Outlook Report Message untuk mengirimkan sampel pesan ke Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b8e38-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
