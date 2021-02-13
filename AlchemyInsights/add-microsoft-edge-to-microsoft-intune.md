---
title: Menambahkan Microsoft Edge ke Microsoft Intune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194511"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="2529a-102">Menambahkan Microsoft Edge ke Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="2529a-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="2529a-103">Agar dapat menggunakan, mengonfigurasi, memantau, dan memproteksi Microsoft Edge untuk Windows 10, Anda harus menambahkannya terlebih dahulu ke Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="2529a-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="2529a-104">Intune mendukung Microsoft Edge 77 dan versi yang lebih baru.</span><span class="sxs-lookup"><span data-stu-id="2529a-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="2529a-105">Intune akan mendeteksi instalasi Microsoft Edge yang sudah ada sebelumnya.</span><span class="sxs-lookup"><span data-stu-id="2529a-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="2529a-106">Jika Microsoft Edge terinstal dalam konteks pengguna, instalasi sistem akan menimpa instalasi dalam konteks pengguna.</span><span class="sxs-lookup"><span data-stu-id="2529a-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="2529a-107">Jika Microsoft Edge terinstal dalam konteks sistem, keberhasilan penginstalan akan dilaporkan.</span><span class="sxs-lookup"><span data-stu-id="2529a-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="2529a-108">Pra-instal Microsoft Edge 77 dan versi yang lebih baru, untuk semua saluran dalam konteks pengguna, akan ditimpa dengan Microsoft Edge terinstal dalam konteks sistem.</span><span class="sxs-lookup"><span data-stu-id="2529a-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="2529a-109">**Prasyarat**</span><span class="sxs-lookup"><span data-stu-id="2529a-109">**Prerequisite**</span></span>

<span data-ttu-id="2529a-110">Versi Windows 10 versi 1709 atau yang lebih baru</span><span class="sxs-lookup"><span data-stu-id="2529a-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="2529a-111">**Langkah-langkah untuk menambahkan Edge ke Intune**</span><span class="sxs-lookup"><span data-stu-id="2529a-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="2529a-112">[Mengonfigurasi aplikasi di Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="2529a-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="2529a-113">[Mengonfigurasi informasi aplikasi](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="2529a-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="2529a-114">[Mengonfigurasi pengaturan aplikasi](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="2529a-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="2529a-115">[Memilih tag lingkup (opsional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="2529a-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="2529a-116">[Tambahkan aplikasi](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="2529a-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="2529a-117">Untuk bantuan selengkapnya, lihat [pemecahan masalah](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="2529a-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




