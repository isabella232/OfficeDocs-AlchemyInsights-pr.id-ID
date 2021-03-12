---
title: Mencari dan menghapus pesan email di organisasi Anda
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746436"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="ea1db-102">Mencari dan menghapus pesan email di organisasi Anda</span><span class="sxs-lookup"><span data-stu-id="ea1db-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="ea1db-103">Ikuti langkah-langkah ini:</span><span class="sxs-lookup"><span data-stu-id="ea1db-103">Follow these steps:</span></span>

1. <span data-ttu-id="ea1db-104">Jika Anda bukan admin global, untuk mencari pesan yang harus ditambahkan ke **grup peran Manajer eDiscovery** atau **peran manajemen pencarian kepatuhan**.</span><span class="sxs-lookup"><span data-stu-id="ea1db-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="ea1db-105">Untuk menghapus pesan, Anda harus bergabung dalam **grup peran manajemen organisasi** atau **peran manajemen pencarian dan** penghapusan.</span><span class="sxs-lookup"><span data-stu-id="ea1db-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="ea1db-106">Izin untuk peran ini ditetapkan di [pusat kepatuhan & keamanan.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="ea1db-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="ea1db-107">[Buat pencarian konten](https://docs.microsoft.com/office365/securitycompliance/content-search) untuk menemukan pesan yang akan dihapus.</span><span class="sxs-lookup"><span data-stu-id="ea1db-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="ea1db-108">[Sambungkan ke pusat kepatuhan & keamanan PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="ea1db-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="ea1db-109">Jika Anda menggunakan MFA, lihat instruksi berikut: [menyambungkan ke keamanan & pusat kepatuhan PowerShell menggunakan autentikasi multifaktor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="ea1db-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="ea1db-110">Hapus pesan: Jalankan `New-ComplianceSearchAction` cmdlet untuk menghapus pesan.</span><span class="sxs-lookup"><span data-stu-id="ea1db-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="ea1db-111">Pesan yang dihapus dipindahkan ke folder Item yang dapat dipulihkan pengguna.</span><span class="sxs-lookup"><span data-stu-id="ea1db-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="ea1db-112">Untuk perintah contoh, lihat [langkah 3: Hapus pesan.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="ea1db-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
