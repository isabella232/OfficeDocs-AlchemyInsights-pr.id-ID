---
title: S/MIME dalam Outlook di web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772265"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="202c7-102">Mengenkripsi pesan email di Outlook</span><span class="sxs-lookup"><span data-stu-id="202c7-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="202c7-103">Enkripsi pesan Microsoft 365 dibangun di Microsoft Azure Rights Management (Azure RMS), yang merupakan bagian dari proteksi informasi Azure.</span><span class="sxs-lookup"><span data-stu-id="202c7-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="202c7-104">Jika langganan Anda meliputi manajemen hak Azure atau perlindungan informasi Azure, **Anda tidak perlu melakukan tindakan apa pun untuk mengaktifkan atau mengaktifkan** Layanan manajemen hak secara manual.</span><span class="sxs-lookup"><span data-stu-id="202c7-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="202c7-105">Berdasarkan umpan balik pelanggan, kami tidak lagi mengaktifkan aturan alur email Exchange untuk secara otomatis mengenkripsi email keluar yang berisi tipe informasi sensitif tertentu dalam penyewa Anda secara default.</span><span class="sxs-lookup"><span data-stu-id="202c7-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="202c7-106">Sebagai gantinya, kami menyediakan instruksi mendetail tentang cara melakukannya sendiri.</span><span class="sxs-lookup"><span data-stu-id="202c7-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="202c7-107">Untuk detail tambahan tentang cara membuat aturan transpor untuk mengenkripsi informasi sensitif, lihat [artikel ini](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="202c7-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="202c7-108">Jika menggunakan Outlook di web (sebelumnya **OWA**): ketika menulis pesan email, cukup klik **proteksi** di OWA.</span><span class="sxs-lookup"><span data-stu-id="202c7-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="202c7-109">Ini akan menerapkan izin "Jangan teruskan".</span><span class="sxs-lookup"><span data-stu-id="202c7-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="202c7-110">Klik **Ubah izin** dan pilih **enkripsi** untuk mengenkripsi pesan saja.</span><span class="sxs-lookup"><span data-stu-id="202c7-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="202c7-111">Jika menggunakan **klien Outlook**: untuk mengirim pesan yang dienkripsi dari Outlook 2013 atau 2016, atau Outlook 2016 untuk Mac, pilih **Options**  >  **izin**opsi, lalu pilih opsi proteksi yang Anda perlukan.</span><span class="sxs-lookup"><span data-stu-id="202c7-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="202c7-112">Untuk secara **otomatis mengenkripsi semua email** yang dikirim ke penerima atau organisasi mitra eksternal tertentu, Anda perlu membuat aturan transpor aliran email di pusat admin Exchange.</span><span class="sxs-lookup"><span data-stu-id="202c7-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="202c7-113">Instruksi mendetail disediakan dalam [artikel dukungan ini](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="202c7-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

