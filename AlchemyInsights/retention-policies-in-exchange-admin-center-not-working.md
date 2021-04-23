---
title: Kebijakan Penyimpanan di Pusat Admin Exchange tidak berfungsi
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952231"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="98e85-102">Kebijakan Penyimpanan di Pusat Admin Exchange</span><span class="sxs-lookup"><span data-stu-id="98e85-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="98e85-103">Jika Anda ingin kami menjalankan pemeriksaan otomatis untuk pengaturan yang disebutkan di bawah ini, pilih tombol kembali <-- di bagian atas halaman ini, lalu masukkan alamat email pengguna yang mengalami masalah dengan kebijakan penyimpanan.</span><span class="sxs-lookup"><span data-stu-id="98e85-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="98e85-104">Jika Anda mengalami masalah dengan kebijakan penyimpanan di Pusat Admin Exchange yang tidak berlaku pada kotak surat atau item yang tidak berpindah ke kotak surat arsip, periksa hal berikut ini:</span><span class="sxs-lookup"><span data-stu-id="98e85-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="98e85-105">**Penyebab Akar:**</span><span class="sxs-lookup"><span data-stu-id="98e85-105">**Root Causes:**</span></span>

- <span data-ttu-id="98e85-106">**Asisten Folder** Terkelola belum memproses kotak surat pengguna.</span><span class="sxs-lookup"><span data-stu-id="98e85-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="98e85-107">Asisten Folder Terkelola mencoba memproses setiap kotak surat di organisasi berbasis awan sekali setiap tujuh hari.</span><span class="sxs-lookup"><span data-stu-id="98e85-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="98e85-108">**Solusi:** Jalankan Asisten Folder yang Dikelola.</span><span class="sxs-lookup"><span data-stu-id="98e85-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="98e85-109">**RetentionHold** telah **diaktifkan** pada kotak surat.</span><span class="sxs-lookup"><span data-stu-id="98e85-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="98e85-110">Jika kotak surat telah ditempatkan di Tempat Penyimpanan, kebijakan penyimpanan pada kotak surat tidak akan diproses selama waktu itu.</span><span class="sxs-lookup"><span data-stu-id="98e85-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="98e85-111">**Solusi:** Periksa status pengaturan dan pembaruan Penyimpanan jika diperlukan.</span><span class="sxs-lookup"><span data-stu-id="98e85-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="98e85-112">Untuk detailnya, lihat [Penyimpanan Kotak Surat.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="98e85-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="98e85-113">**Catatan:** Jika kotak surat lebih kecil dari 10 MB, Asisten Folder Yang Dikelola tidak akan memproses kotak surat secara otomatis.</span><span class="sxs-lookup"><span data-stu-id="98e85-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="98e85-114">Untuk informasi selengkapnya tentang kebijakan penyimpanan di Pusat Admin Exchange, lihat:</span><span class="sxs-lookup"><span data-stu-id="98e85-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="98e85-115">Tag penyimpanan dan kebijakan penyimpanan</span><span class="sxs-lookup"><span data-stu-id="98e85-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="98e85-116">[Menerapkan kebijakan penyimpanan ke kotak surat](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) atau Menambahkan atau menghapus tag [penyimpanan](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="98e85-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="98e85-117">Cara mengidentifikasi tipe penyimpanan yang ditempatkan di kotak surat</span><span class="sxs-lookup"><span data-stu-id="98e85-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
