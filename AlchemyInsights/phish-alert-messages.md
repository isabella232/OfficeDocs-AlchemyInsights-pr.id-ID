---
title: 2491 pesan email peringatan dari ' Phish disampaikan karena penghuni atau pengguna menimpa ' kebijakan
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758931"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="39f14-102">Pesan email peringatan dari ' Phish disampaikan karena penyewa atau pengguna menimpa ' kebijakan</span><span class="sxs-lookup"><span data-stu-id="39f14-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="39f14-103">Kebijakan peringatan default bernama "dikirim phish karena penghuni atau pengguna menimpa" telah diluncurkan ke penyewa dengan Office 365 ATP P1 dan P2 lisensi.</span><span class="sxs-lookup"><span data-stu-id="39f14-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="39f14-104">Jika Anda menerima peringatan ini, berikut adalah langkah untuk menyelidiki:</span><span class="sxs-lookup"><span data-stu-id="39f14-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="39f14-105">Dari pesan peringatan, klik **Lihat peringatan** untuk membuka halaman **peringatan** di pusat kepatuhan & keamanan.</span><span class="sxs-lookup"><span data-stu-id="39f14-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="39f14-106">Pilih peringatan untuk melihat pilihan untuk melihat **Daftar pesan** atau **melihat pesan di Explorer**.</span><span class="sxs-lookup"><span data-stu-id="39f14-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="39f14-107">Kedua pilihan ini akan membawa Anda ke rincian pesan, yang mencakup ID pesan.</span><span class="sxs-lookup"><span data-stu-id="39f14-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="39f14-108">Perhatikan bahwa tautan Threat Explorer akan secara otomatis menyaring pesan yang sesuai dengan kriteria peringatan.</span><span class="sxs-lookup"><span data-stu-id="39f14-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="39f14-109">Anda mungkin perlu menyesuaikan filter tanggal di Threat Explorer.</span><span class="sxs-lookup"><span data-stu-id="39f14-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="39f14-110">Pesan phishing dikirim karena menimpa dikonfigurasi secara manual:</span><span class="sxs-lookup"><span data-stu-id="39f14-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="39f14-111">Pengirim atau domain yang diizinkan yang ditetapkan oleh pengguna.</span><span class="sxs-lookup"><span data-stu-id="39f14-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="39f14-112">Pengirim atau domain yang diizinkan yang ditetapkan oleh admin dalam kebijakan anti-spam.</span><span class="sxs-lookup"><span data-stu-id="39f14-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="39f14-113">Alamat IP yang diizinkan dalam kebijakan filter sambungan.</span><span class="sxs-lookup"><span data-stu-id="39f14-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="39f14-114">Aturan aliran e-mail (juga dikenal sebagai aturan transport) yang dikonfigurasi untuk membolehkan pesan.</span><span class="sxs-lookup"><span data-stu-id="39f14-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="39f14-115">Jika Anda yakin pesan salah ditandai sebagai Phish, gunakan Outlook [pesan laporan Add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) untuk mengirimkan sampel pesan ke Microsoft.</span><span class="sxs-lookup"><span data-stu-id="39f14-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
