---
title: Memperbaiki masalah-masalah pengiriman email ke dukungan e-mail folder publik
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: d1c1d5bcb52ba9083e8dd7603feb72436c5154c8
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/17/2019
ms.locfileid: "31910605"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="f4a09-102">Memperbaiki masalah-masalah pengiriman email ke dukungan e-mail folder publik</span><span class="sxs-lookup"><span data-stu-id="f4a09-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="f4a09-103">Jika pengirim eksternal tidak dapat mengirim pesan ke folder publik Anda dukungan e-mail, dan pengirim menerima kesalahan: **tidak dapat ditemukan (550 5.4.1)**, verifikasi email domain untuk map publik dikonfigurasi sebagai domain internal relay bukan domain otoritatif:</span><span class="sxs-lookup"><span data-stu-id="f4a09-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="f4a09-104">Membuka [Pusat admin pertukaran (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="f4a09-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="f4a09-105">Pergi ke **alur E-mail** \> **domain diterima**, pilih domain diterima, dan kemudian klik **mengedit**.</span><span class="sxs-lookup"><span data-stu-id="f4a09-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="f4a09-106">Dalam properti halaman yang terbuka, jika jenis domain diatur ke **Authoritative**, mengubah nilai untuk **Internal relay** dan kemudian klik **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="f4a09-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="f4a09-107">Jika pengirim eksternal menerima kesalahan yang **Anda tidak memiliki izin (550 5.7.13)**, jalankan perintah berikut dalam [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) untuk melihat izin untuk pengguna anonim di map publik:</span><span class="sxs-lookup"><span data-stu-id="f4a09-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="f4a09-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Sebagai contoh, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="f4a09-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="f4a09-109">Untuk membolehkan pengguna eksternal mengirim email ke folder publik ini, tambahkan CreateItems akses hak untuk pengguna anonim.</span><span class="sxs-lookup"><span data-stu-id="f4a09-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="f4a09-110">Sebagai contoh, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="f4a09-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
