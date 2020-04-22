---
title: Memperbaiki masalah pengiriman email ke folder publik Surat
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716355"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="076b0-102">Memperbaiki masalah pengiriman email ke folder publik Surat</span><span class="sxs-lookup"><span data-stu-id="076b0-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="076b0-103">Jika pengirim eksternal tidak dapat mengirim pesan ke folder publik surat Anda, dan pengirim menerima galat: **tidak dapat ditemukan (550 5.4.1)**, verifikasi domain email untuk folder publik dikonfigurasi sebagai domain relay internal dan bukan otoritatif domain:</span><span class="sxs-lookup"><span data-stu-id="076b0-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="076b0-104">Buka [Exchange Admin Center (eac)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="076b0-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="076b0-105">Buka \> **domain yang diterima** **aliran e-mail** , pilih domain diterima, lalu klik **Edit**.</span><span class="sxs-lookup"><span data-stu-id="076b0-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="076b0-106">Di halaman properti yang terbuka, jika jenis domain diatur ke **otoritatif**, Ubah nilai ke **relay internal** , lalu klik **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="076b0-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="076b0-107">Jika pengirim eksternal menerima galat **Anda tidak memiliki izin (550 5.7.13)**, jalankan perintah berikut ini di [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) untuk melihat izin untuk pengguna anonim di folder publik:</span><span class="sxs-lookup"><span data-stu-id="076b0-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="076b0-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Misalnya, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="076b0-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="076b0-109">Untuk mengizinkan pengguna eksternal untuk mengirim email ke folder publik ini, tambahkan hak akses CreateItems ke pengguna anonim.</span><span class="sxs-lookup"><span data-stu-id="076b0-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="076b0-110">Misalnya, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="076b0-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
