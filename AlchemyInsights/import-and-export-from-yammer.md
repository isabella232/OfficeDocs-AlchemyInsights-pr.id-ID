---
title: Mengimpor dan mengekspor dari Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036123"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="a9cd2-102">Mengimpor dan mengekspor dari Yammer</span><span class="sxs-lookup"><span data-stu-id="a9cd2-102">Import and export from Yammer</span></span>

<span data-ttu-id="a9cd2-103">**Mengimpor**</span><span class="sxs-lookup"><span data-stu-id="a9cd2-103">**Import**</span></span>

<span data-ttu-id="a9cd2-104">Opsi impor pengguna berbeda-beda tergantung pada apakah jaringan Yammer Anda berada dalam [mode asli untuk Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), atau tidak.</span><span class="sxs-lookup"><span data-stu-id="a9cd2-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="a9cd2-105">**Mode non-asli**: pengguna dapat diimpor ke grup menggunakan [Tambahkan dari buku alamat](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (batas ke pengguna 100) dalam pengaturan grup, atau ke jaringan menggunakan [pembaruan massal](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) dalam admin jaringan.</span><span class="sxs-lookup"><span data-stu-id="a9cd2-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="a9cd2-106">**Mode asli**: keanggotaan grup dan operasi keanggotaan jaringan harus dilakukan dari [portal admin Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), [portal Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), atau menggunakan opsi lain Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a9cd2-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="a9cd2-107">Jaringan dalam mode asli tidak lagi memiliki akses ke pembaruan sekaligus fitur warisan lainnya.</span><span class="sxs-lookup"><span data-stu-id="a9cd2-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a9cd2-108">Yammer tidak pernah mendukung mengimpor konten dari dalam admin jaringan Meskipun fitur ekspor data digunakan di jaringan lain.</span><span class="sxs-lookup"><span data-stu-id="a9cd2-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="a9cd2-109">Konten dapat diposting ulang oleh solusi mitra atau api REST Yammer.</span><span class="sxs-lookup"><span data-stu-id="a9cd2-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="a9cd2-110">**Ex**</span><span class="sxs-lookup"><span data-stu-id="a9cd2-110">**Export**</span></span>

<span data-ttu-id="a9cd2-111">[Mengekspor data jaringan dalam admin jaringan](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) memperbolehkan ekspor konten dari jaringan Yammer, termasuk pesan dan file.</span><span class="sxs-lookup"><span data-stu-id="a9cd2-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="a9cd2-112">Lampiran bisa sangat besar dan akan menyebabkan ekspor untuk mendapatkan waktu yang signifikan untuk menyelesaikannya.</span><span class="sxs-lookup"><span data-stu-id="a9cd2-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="a9cd2-113">Kami merekomendasikan bahwa jaringan aktif diekspor menggunakan [api ekspor data](https://developer.yammer.com/docs/data-export-api) dalam potongan menurut hari atau minggu.</span><span class="sxs-lookup"><span data-stu-id="a9cd2-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="a9cd2-114">Dukungan Microsoft tidak menyediakan skrip kustom untuk tujuan ini.</span><span class="sxs-lookup"><span data-stu-id="a9cd2-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="a9cd2-115">[Ekspor GDPR](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) terpisah ada untuk mengekspor konten untuk pengguna individual.</span><span class="sxs-lookup"><span data-stu-id="a9cd2-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>