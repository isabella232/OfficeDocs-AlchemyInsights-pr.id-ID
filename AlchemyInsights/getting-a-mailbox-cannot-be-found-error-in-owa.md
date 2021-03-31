---
title: 126 Kesalahan Mendapatkan Kotak Surat di OWA?
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
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426665"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="a0fa7-102">Mendapatkan kotak surat tidak menemukan kesalahan di Outlook di web?</span><span class="sxs-lookup"><span data-stu-id="a0fa7-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="a0fa7-103">Jika Anda menggunakan Outlook di web dan  terjadi kesalahan ketika mendapatkan Kotak Surat tidak dapat ditemukan, akun yang Anda gunakan untuk menyambungkan ke Outlook di web tidak memiliki lisensi Exchange Online, sehingga tidak ada kotak surat yang terkait dengan akun tersebut.</span><span class="sxs-lookup"><span data-stu-id="a0fa7-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="a0fa7-104">Admin dapat menetapkan lisensi ke akun Anda dengan mengikuti langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="a0fa7-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="a0fa7-105">Buka pusat [admin Microsoft 365](https://portal.office.com/adminportal/home#/homepage) lalu masuk ke **Pengguna** **aktif** di bawah bagian Pengguna, lalu pilih pengguna yang melihat kesalahan.</span><span class="sxs-lookup"><span data-stu-id="a0fa7-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="a0fa7-106">Di halaman pengguna yang terbuka,  masuk ke bagian Lisensi  dan Aplikasi, pilih nilai Lokasi yang sesuai, dan tetapkan lisensi yang berisi Exchange Online (perluas lisensi untuk melihat detailnya).</span><span class="sxs-lookup"><span data-stu-id="a0fa7-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="a0fa7-107">Bila Anda sudah selesai, klik **Simpan perubahan.**</span><span class="sxs-lookup"><span data-stu-id="a0fa7-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="a0fa7-108">Dalam beberapa kasus, jika lisensi sudah ditetapkan ke akun pengguna, menghapus dan menetapkan ulang lisensi akan membantu mengatasi masalah tersebut dan mendapatkannya dengan benar disediakan dalam sistem:</span><span class="sxs-lookup"><span data-stu-id="a0fa7-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="a0fa7-109">Periksa untuk melihat apakah langganan M365 Exchange Online (dan lainnya, jika ada) yang sedang berjalan dan belum kedaluwarsa baru-baru ini.</span><span class="sxs-lookup"><span data-stu-id="a0fa7-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="a0fa7-110">Setelah memastikan bahwa langganan anda belum kedaluwarsa dan lisensi yang valid telah ditetapkan ke akun pengguna, perlu waktu hingga 24 jam agar lisensi tersedia, sehingga Anda mungkin harus menunggu hingga masalah Anda atasi.</span><span class="sxs-lookup"><span data-stu-id="a0fa7-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="a0fa7-111">Untuk informasi selengkapnya, [lihat Menetapkan dan mengelola lisensi.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)</span><span class="sxs-lookup"><span data-stu-id="a0fa7-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>