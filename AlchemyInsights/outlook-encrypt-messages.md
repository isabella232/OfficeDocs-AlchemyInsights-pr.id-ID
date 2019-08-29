---
title: S/MIME di Outlook di web
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666843"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="a8bf2-102">Mengenkripsi pesan email di Outlook</span><span class="sxs-lookup"><span data-stu-id="a8bf2-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="a8bf2-103">Enkripsi pesan Office 365 dibuat di Microsoft Azure Rights Management (Azure RMS), yang merupakan bagian dari perlindungan informasi Azure.</span><span class="sxs-lookup"><span data-stu-id="a8bf2-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="a8bf2-104">Jika langganan Anda mencakup pengelolaan hak Azure atau perlindungan informasi Azure, **Anda tidak perlu melakukan tindakan apa pun untuk mengaktifkan atau** mengaktifkan layanan manajemen hak secara manual.</span><span class="sxs-lookup"><span data-stu-id="a8bf2-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="a8bf2-105">Berdasarkan umpan balik pelanggan, kami tidak akan lagi mengaktifkan aturan aliran surat Exchange untuk secara otomatis mengenkripsi email keluar yang berisi jenis informasi sensitif tertentu di penyewa Anda secara default.</span><span class="sxs-lookup"><span data-stu-id="a8bf2-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="a8bf2-106">Sebaliknya, kami menyediakan petunjuk rinci tentang bagaimana Anda dapat melakukannya sendiri.</span><span class="sxs-lookup"><span data-stu-id="a8bf2-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="a8bf2-107">Untuk rincian tambahan tentang cara membuat aturan transpor untuk mengenkripsi informasi sensitif, lihat [artikel ini](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="a8bf2-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="a8bf2-108">Jika menggunakan Outlook di web (sebelumnya **OWA**): saat menulis pesan email, cukup klik **melindungi** di OWA.</span><span class="sxs-lookup"><span data-stu-id="a8bf2-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="a8bf2-109">Ini akan menerapkan izin "Jangan maju".</span><span class="sxs-lookup"><span data-stu-id="a8bf2-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="a8bf2-110">Klik **Ubah izin** dan pilih **enkripsi** untuk hanya mengenkripsi pesan.</span><span class="sxs-lookup"><span data-stu-id="a8bf2-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="a8bf2-111">Jika menggunakan **klien Outlook**: untuk mengirim pesan terenkripsi dari Outlook 2013 atau 2016, atau Outlook 2016 untuk Mac, pilih **opsi** > **izin**, kemudian pilih opsi perlindungan yang Anda butuhkan.</span><span class="sxs-lookup"><span data-stu-id="a8bf2-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="a8bf2-112">Untuk secara **otomatis mengenkripsi semua email** yang dikirim ke penerima tertentu atau organisasi mitra eksternal, Anda perlu membuat aturan transpor aliran surat di pusat admin Exchange.</span><span class="sxs-lookup"><span data-stu-id="a8bf2-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="a8bf2-113">Petunjuk terperinci disediakan dalam [artikel dukungan ini](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="a8bf2-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

