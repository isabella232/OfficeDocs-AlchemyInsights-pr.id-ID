---
title: Kebijakan berbagi kalender 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684233"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="c121e-102">Kesalahan kebijakan saat berbagi kalender</span><span class="sxs-lookup"><span data-stu-id="c121e-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="c121e-103">Lakukan salah satu hal berikut ini, yang sesuai untuk situasi Anda:</span><span class="sxs-lookup"><span data-stu-id="c121e-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="c121e-104">Menyambungkan ke Exchange Online menggunakan PowerShell jarak jauh.</span><span class="sxs-lookup"><span data-stu-id="c121e-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="c121e-105">Untuk informasi selengkapnya, lihat [menyambungkan ke Exchange Online menggunakan PowerShell jarak jauh](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="c121e-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="c121e-106">Di server lokal, buka Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="c121e-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="c121e-107">Menentukan kebijakan berbagi yang ditetapkan untuk pengguna.</span><span class="sxs-lookup"><span data-stu-id="c121e-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="c121e-108">Untuk melakukan ini, jalankan perintah berikut ini dan catat kebijakan yang dikembalikan:</span><span class="sxs-lookup"><span data-stu-id="c121e-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="c121e-109">Memperbarui kebijakan berbagi untuk pengguna.</span><span class="sxs-lookup"><span data-stu-id="c121e-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="c121e-110">Untuk melakukan ini, ikuti langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="c121e-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="c121e-111">Buka Pusat admin Exchange.</span><span class="sxs-lookup"><span data-stu-id="c121e-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="c121e-112">Klik **organisasi**, lalu klik dua kali kebijakan yang ditetapkan untuk pengguna di bawah **masing-masing berbagi**.</span><span class="sxs-lookup"><span data-stu-id="c121e-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="c121e-113">Ini adalah kebijakan yang dikembalikan di langkah 2.</span><span class="sxs-lookup"><span data-stu-id="c121e-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="c121e-114">Pada halaman aturan berbagi, pilih tingkat berbagi kalender yang ingin Anda Izinkan di bawah **tentukan informasi apa yang ingin Anda bagikan**; Klik **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="c121e-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="c121e-115">Untuk informasi selengkapnya, lihat: ["kebijakan tidak memperbolehkan pemberian izin pada tingkat ini ke satu atau beberapa penerima pesan kesalahan" ketika pengguna mencoba berbagi kalender](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="c121e-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
