---
title: Pesan 2491 alert email dari kebijakan 'Terkirim Phish karena pengguna atau penyewa menimpa'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391340"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="5e31c-102">Email pemberitahuan pesan dari 'Terkirim Phish karena pengguna atau penyewa menimpa' kebijakan</span><span class="sxs-lookup"><span data-stu-id="5e31c-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="5e31c-103">Kebijakan alert default bernama "Phish disampaikan karena menimpa penyewa atau pengguna" telah digulirkan untuk penyewa dengan lisensi Office 365 ATP P1 dan P2.</span><span class="sxs-lookup"><span data-stu-id="5e31c-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="5e31c-104">Jika Anda menerima peringatan ini, berikut adalah langkah-langkah untuk menyelidiki:</span><span class="sxs-lookup"><span data-stu-id="5e31c-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="5e31c-105">Dari pesan peringatan, klik **Lihat waspada** untuk pergi ke halaman **peringatan** dalam & keamanan Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="5e31c-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="5e31c-106">Pilih waspada untuk melihat pilihan untuk **tampilan daftar pesan** atau **Pesan Lihat dalam Explorer**.</span><span class="sxs-lookup"><span data-stu-id="5e31c-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="5e31c-107">Kedua pilihan ini membawa Anda ke rincian pesan, termasuk pesan ID.</span><span class="sxs-lookup"><span data-stu-id="5e31c-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="5e31c-108">Perhatikan bahwa ancaman Explorer link secara otomatis akan menyaring pesan yang sesuai kriteria waspada.</span><span class="sxs-lookup"><span data-stu-id="5e31c-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="5e31c-109">Anda mungkin perlu menyesuaikan tanggal filter di Explorer ancaman.</span><span class="sxs-lookup"><span data-stu-id="5e31c-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="5e31c-110">Pesan phishing disampaikan karena menimpa dikonfigurasi secara manual:</span><span class="sxs-lookup"><span data-stu-id="5e31c-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="5e31c-111">Diperbolehkan pengirim atau domain yang ditetapkan oleh pengguna.</span><span class="sxs-lookup"><span data-stu-id="5e31c-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="5e31c-112">Diperbolehkan pengirim atau domain yang ditetapkan oleh admin dalam kebijakan anti spam.</span><span class="sxs-lookup"><span data-stu-id="5e31c-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="5e31c-113">Alamat IP yang diizinkan dalam kebijakan filter koneksi.</span><span class="sxs-lookup"><span data-stu-id="5e31c-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="5e31c-114">Mail aliran aturan (juga dikenal sebagai aturan transport) yang dikonfigurasi untuk membolehkan pesan di.</span><span class="sxs-lookup"><span data-stu-id="5e31c-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="5e31c-115">Jika Anda yakin pesan salah ditandai sebagai phish, menggunakan Outlook [laporan pesan Tambah-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) untuk mengirimkan pesan sampel ke Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5e31c-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
