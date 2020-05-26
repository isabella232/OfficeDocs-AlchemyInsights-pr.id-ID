---
title: 618 kebijakan berbagi kalender
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373002"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="b9ebb-102">Galat kebijakan saat berbagi kalender</span><span class="sxs-lookup"><span data-stu-id="b9ebb-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="b9ebb-103">Lakukan salah satu dari berikut ini, yang sesuai untuk situasi Anda:</span><span class="sxs-lookup"><span data-stu-id="b9ebb-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="b9ebb-104">Menyambung ke Exchange Online menggunakan PowerShell jarak jauh.</span><span class="sxs-lookup"><span data-stu-id="b9ebb-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="b9ebb-105">Untuk informasi selengkapnya, lihat [tersambung ke Exchange Online menggunakan PowerShell jarak jauh](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="b9ebb-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="b9ebb-106">Di server lokal, buka Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="b9ebb-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="b9ebb-107">Menentukan kebijakan berbagi yang ditetapkan untuk pengguna.</span><span class="sxs-lookup"><span data-stu-id="b9ebb-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="b9ebb-108">Untuk melakukannya, jalankan perintah berikut ini dan catat kebijakan yang dikembalikan:</span><span class="sxs-lookup"><span data-stu-id="b9ebb-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="b9ebb-109">Memperbarui kebijakan berbagi untuk pengguna.</span><span class="sxs-lookup"><span data-stu-id="b9ebb-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="b9ebb-110">Untuk melakukan ini, ikuti langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="b9ebb-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="b9ebb-111">Buka Pusat admin Exchange.</span><span class="sxs-lookup"><span data-stu-id="b9ebb-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="b9ebb-112">Klik **organisasi**, dan kemudian klik dua kali kebijakan yang ditetapkan untuk pengguna di bawah masing- **masing berbagi**.</span><span class="sxs-lookup"><span data-stu-id="b9ebb-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="b9ebb-113">Ini adalah kebijakan yang dikembalikan di langkah 2.</span><span class="sxs-lookup"><span data-stu-id="b9ebb-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="b9ebb-114">Pada halaman aturan berbagi, pilih tingkat berbagi kalender yang ingin Anda Izinkan di bawah **menentukan informasi apa yang Anda ingin berbagi**; Klik **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="b9ebb-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="b9ebb-115">Untuk informasi selengkapnya, lihat: ["kebijakan tidak mengizinkan memberikan izin pada tingkat ini ke satu atau lebih Penerima" galat saat pengguna berusaha berbagi kalender](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="b9ebb-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
