---
title: Tidak bisa mengakses folder publik
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819515"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="65af5-102">Outlook tidak bisa tersambung ke folder publik</span><span class="sxs-lookup"><span data-stu-id="65af5-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="65af5-103">Jika akses folder publik tidak berfungsi untuk beberapa pengguna, cobalah hal berikut:</span><span class="sxs-lookup"><span data-stu-id="65af5-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="65af5-104">Sambungkan ke EXO PowerShell dan konfigurasi parameter DefaultPublicFolderMailbox pada akun pengguna yang bermasalah agar sesuai dengan parameter pada akun pengguna yang berfungsi.</span><span class="sxs-lookup"><span data-stu-id="65af5-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="65af5-105">Contoh:</span><span class="sxs-lookup"><span data-stu-id="65af5-105">Example:</span></span>

<span data-ttu-id="65af5-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="65af5-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="65af5-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="65af5-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="65af5-108">Tunggu setidaknya satu jam agar perubahan bisa diterapkan.</span><span class="sxs-lookup"><span data-stu-id="65af5-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="65af5-109">Jika masalah tetap terjadi, ikuti prosedur [ini untuk](https://aka.ms/pfcte) memecahkan masalah akses folder publik menggunakan Outlook.</span><span class="sxs-lookup"><span data-stu-id="65af5-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="65af5-110">**Untuk mengontrol pengguna mana yang bisa mengakses folder publik menggunakan Outlook:**</span><span class="sxs-lookup"><span data-stu-id="65af5-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="65af5-111">Gunakan Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true atau $false</span><span class="sxs-lookup"><span data-stu-id="65af5-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="65af5-112">$true: Memungkinkan pengguna mengakses folder publik di Outlook</span><span class="sxs-lookup"><span data-stu-id="65af5-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="65af5-113">$false: Mencegah akses pengguna ke folder publik di Outlook.</span><span class="sxs-lookup"><span data-stu-id="65af5-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="65af5-114">Ini adalah nilai default.</span><span class="sxs-lookup"><span data-stu-id="65af5-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="65af5-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="65af5-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="65af5-116">**Catatan** Prosedur ini hanya bisa mengontrol koneksi dengan desktop Outlook untuk klien Windows.</span><span class="sxs-lookup"><span data-stu-id="65af5-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="65af5-117">Pengguna bisa terus mengakses folder publik menggunakan OWA atau Outlook untuk Mac.</span><span class="sxs-lookup"><span data-stu-id="65af5-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="65af5-118">Untuk informasi selengkapnya, [lihat Mengumumkan Dukungan untuk Koneksi Terkontrol ke Folder Publik di Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="65af5-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>