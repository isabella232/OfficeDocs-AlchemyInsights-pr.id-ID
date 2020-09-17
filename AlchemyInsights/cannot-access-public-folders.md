---
title: Tidak dapat mengakses folder publik
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812550"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="40eb4-102">Outlook tidak dapat tersambung ke folder publik</span><span class="sxs-lookup"><span data-stu-id="40eb4-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="40eb4-103">Jika akses folder publik tidak berfungsi untuk beberapa pengguna, cobalah hal berikut:</span><span class="sxs-lookup"><span data-stu-id="40eb4-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="40eb4-104">Sambungkan ke EXO PowerShell dan konfigurasikan parameter DefaultPublicFolderMailbox pada akun pengguna bermasalah untuk mencocokkan parameter pada akun pengguna yang bekerja.</span><span class="sxs-lookup"><span data-stu-id="40eb4-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="40eb4-105">Misalnya</span><span class="sxs-lookup"><span data-stu-id="40eb4-105">Example:</span></span>

<span data-ttu-id="40eb4-106">Dapatkan-kotak surat pengguna | Kotak surat ft Defaultpublicfolder, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="40eb4-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="40eb4-107">Set-kotak surat ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="40eb4-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="40eb4-108">Tunggu setidaknya satu jam agar perubahan diterapkan.</span><span class="sxs-lookup"><span data-stu-id="40eb4-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="40eb4-109">Jika masalah tetap terjadi, ikuti [prosedur ini](https://aka.ms/pfcte) untuk memecahkan masalah akses folder publik menggunakan Outlook.</span><span class="sxs-lookup"><span data-stu-id="40eb4-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="40eb4-110">**Untuk mengontrol pengguna mana yang bisa mengakses folder publik menggunakan Outlook**:</span><span class="sxs-lookup"><span data-stu-id="40eb4-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="40eb4-111">Menggunakan Set-CASMailbox <mailboxname> -publicfolderclientaccess $True atau $false</span><span class="sxs-lookup"><span data-stu-id="40eb4-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="40eb4-112">$true: Izinkan pengguna mengakses folder publik di Outlook</span><span class="sxs-lookup"><span data-stu-id="40eb4-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="40eb4-113">$false: mencegah akses pengguna ke folder publik di Outlook.</span><span class="sxs-lookup"><span data-stu-id="40eb4-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="40eb4-114">Ini adalah nilai default.</span><span class="sxs-lookup"><span data-stu-id="40eb4-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="40eb4-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="40eb4-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="40eb4-116">**Catatan** Prosedur ini hanya dapat mengontrol koneksi dengan klien Outlook desktop untuk Windows.</span><span class="sxs-lookup"><span data-stu-id="40eb4-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="40eb4-117">Pengguna bisa terus mengakses folder publik menggunakan OWA atau Outlook untuk Mac.</span><span class="sxs-lookup"><span data-stu-id="40eb4-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="40eb4-118">Untuk informasi selengkapnya, lihat [mengumumkan dukungan untuk koneksi terkendali ke folder publik di Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="40eb4-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>