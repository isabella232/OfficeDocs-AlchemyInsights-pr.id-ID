---
title: Setel ClientAccessServerEnabled ke True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525958"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="cb707-102">Setel ClientAccessServerEnabled ke True</span><span class="sxs-lookup"><span data-stu-id="cb707-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="cb707-103">Jika Anda tidak bisa membuka pesan email terenkripsi dan sebagai gantinya melihat lampiran **MSG** , lakukan langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="cb707-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="cb707-104">Menyambungkan ke Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="cb707-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="cb707-105">Untuk menyambungkan ke Exchange Online PowerShell, Anda harus masuk menggunakan akun admin global atau Exchange admin.</span><span class="sxs-lookup"><span data-stu-id="cb707-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="cb707-106">untuk.</span><span class="sxs-lookup"><span data-stu-id="cb707-106">a.</span></span> <span data-ttu-id="cb707-107">Buka Windows PowerShell, lalu jalankan perintah berikut: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="cb707-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="cb707-108">b.</span><span class="sxs-lookup"><span data-stu-id="cb707-108">b.</span></span> <span data-ttu-id="cb707-109">Dalam kotak dialog **permintaan kredensial Windows PowerShell** , masukkan akun kerja atau sekolah dan kata sandi Anda, c.</span><span class="sxs-lookup"><span data-stu-id="cb707-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="cb707-110">Klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="cb707-110">Click **OK**.</span></span> 

2. <span data-ttu-id="cb707-111">Jalankan perintah berikut ini untuk membuat sesi baru:</span><span class="sxs-lookup"><span data-stu-id="cb707-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="cb707-112">untuk.</span><span class="sxs-lookup"><span data-stu-id="cb707-112">a.</span></span> <span data-ttu-id="cb707-113">Jalankan perintah berikut:</span><span class="sxs-lookup"><span data-stu-id="cb707-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="cb707-114">Jalankan `Get-IRMConfiguration` perintah.</span><span class="sxs-lookup"><span data-stu-id="cb707-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="cb707-115">Periksa pengaturan **Clientaccessserverenabled** .</span><span class="sxs-lookup"><span data-stu-id="cb707-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="cb707-116">untuk.</span><span class="sxs-lookup"><span data-stu-id="cb707-116">a.</span></span> <span data-ttu-id="cb707-117">Jika pengaturan **Clientaccessserverenabled** diatur ke **false**, Jalankan cmdlet berikut: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="cb707-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="cb707-118">Selalu tutup sesi PowerShell Anda dengan perintah berikut ini: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="cb707-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="cb707-119">Untuk informasi selengkapnya, lihat [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="cb707-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

