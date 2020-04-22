---
title: Memindahkan pesan email ke kotak surat Arsip
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713649"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="dd7ef-102">Memindahkan email ke kotak pesan arsip</span><span class="sxs-lookup"><span data-stu-id="dd7ef-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="dd7ef-103">Konfirmasikan bahwa **kotak pesan arsip** telah diaktifkan.</span><span class="sxs-lookup"><span data-stu-id="dd7ef-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="dd7ef-104">Jika tidak, gunakan langkah dalam [artikel ini](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) untuk mengaktifkan kotak surat Arsip.</span><span class="sxs-lookup"><span data-stu-id="dd7ef-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="dd7ef-105">Untuk mengarsipkan pesan secara otomatis ke kotak pesan arsip, tag penyimpanan dengan tindakan **Pindahkan ke arsip** harus ditetapkan ke diterapkan secara **otomatis ke seluruh Tag kotak pesan (default)**.</span><span class="sxs-lookup"><span data-stu-id="dd7ef-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="dd7ef-106">Gunakan langkah di sini untuk membuat Tag: [tag default Arsip](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="dd7ef-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="dd7ef-107">Selanjutnya, Tambahkan tag **Arsip** ke kebijakan retensi Anda.</span><span class="sxs-lookup"><span data-stu-id="dd7ef-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="dd7ef-108">Di pusat admin Exchange, pilih **kebijakan retensi** > Tambahkan **tag Pindahkan ke arsip** ke kebijakan > **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="dd7ef-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="dd7ef-109">Sekarang [tetapkan kebijakan penyimpanan](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) ke kotak pesan pengguna tertentu.</span><span class="sxs-lookup"><span data-stu-id="dd7ef-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="dd7ef-110">Kebijakan yang sama akan diterapkan ke kotak surat **primer** dan **Arsip** .</span><span class="sxs-lookup"><span data-stu-id="dd7ef-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="dd7ef-111">Mungkin diperlukan untuk memaksa Managed folder Assistant (MFA) untuk menjalankan dan menerapkan pengaturan baru ke kotak surat pengguna.</span><span class="sxs-lookup"><span data-stu-id="dd7ef-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="dd7ef-112">Jalankan perintah berikut saat [tersambung ke EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) untuk memulai bantuan folder yang dikelola untuk kotak pesan tertentu:</span><span class="sxs-lookup"><span data-stu-id="dd7ef-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="dd7ef-113">Mulai-ManagedFolderAssistant-identitas<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="dd7ef-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="dd7ef-114">Untuk informasi lebih lanjut tentang penyiapan kebijakan pengarsipan, lihat [menyiapkan kebijakan pengarsipan dan penghapusan untuk kotak pesan](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="dd7ef-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  