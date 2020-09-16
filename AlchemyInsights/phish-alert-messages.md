---
title: 2491 pemberitahuan pesan email dari kebijakan ' Phish dikirim karena penyewa atau menimpa pengguna '
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
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728614"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="347d9-102">Pemberitahuan pesan email dari kebijakan ' Phish dikirim karena penyewa atau menimpa pengguna '</span><span class="sxs-lookup"><span data-stu-id="347d9-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="347d9-103">Kebijakan pemberitahuan default bernama "Phish dikirim karena penyewa atau menimpa pengguna" telah diluncurkan kepada penyewa dengan lisensi Office 365 ATP P1 dan P2.</span><span class="sxs-lookup"><span data-stu-id="347d9-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="347d9-104">Jika Anda menerima pemberitahuan ini, berikut adalah langkah-langkah untuk menyelidiki:</span><span class="sxs-lookup"><span data-stu-id="347d9-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="347d9-105">Dari pesan peringatan, klik **pemberitahuan tampilan** untuk masuk ke halaman **pemberitahuan** di pusat kepatuhan & keamanan.</span><span class="sxs-lookup"><span data-stu-id="347d9-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="347d9-106">Pilih pemberitahuan untuk melihat opsi untuk **menampilkan daftar pesan** atau **menampilkan pesan di Explorer**.</span><span class="sxs-lookup"><span data-stu-id="347d9-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="347d9-107">Kedua opsi ini akan membawa Anda ke detail pesan, yang menyertakan ID pesan.</span><span class="sxs-lookup"><span data-stu-id="347d9-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="347d9-108">Perhatikan bahwa tautan penjelajah ancaman akan secara otomatis memfilter pesan yang sesuai dengan kriteria peringatan.</span><span class="sxs-lookup"><span data-stu-id="347d9-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="347d9-109">Anda mungkin perlu menyesuaikan filter tanggal di Threat Explorer.</span><span class="sxs-lookup"><span data-stu-id="347d9-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="347d9-110">Pesan Pengelabuan terkirim karena menimpa dikonfigurasi secara manual:</span><span class="sxs-lookup"><span data-stu-id="347d9-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="347d9-111">Pengirim atau domain yang diizinkan yang diatur oleh pengguna.</span><span class="sxs-lookup"><span data-stu-id="347d9-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="347d9-112">Pengirim atau domain yang diizinkan yang diatur oleh admin dalam kebijakan anti spam.</span><span class="sxs-lookup"><span data-stu-id="347d9-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="347d9-113">Alamat IP yang diperbolehkan dalam kebijakan filter koneksi.</span><span class="sxs-lookup"><span data-stu-id="347d9-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="347d9-114">Aturan alur email (juga dikenal sebagai aturan transpor) yang dikonfigurasi untuk memperbolehkan pesan masuk.</span><span class="sxs-lookup"><span data-stu-id="347d9-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="347d9-115">Jika Anda yakin pesan ditandai dengan Phish, gunakan [Add-in pesan laporan](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) Outlook untuk mengirimkan contoh pesan ke Microsoft.</span><span class="sxs-lookup"><span data-stu-id="347d9-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
