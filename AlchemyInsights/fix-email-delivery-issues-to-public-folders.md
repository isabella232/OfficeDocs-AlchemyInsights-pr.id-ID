---
title: Memperbaiki masalah pengiriman email ke folder publik email aktif
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677931"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="58999-102">Memperbaiki masalah pengiriman email ke folder publik email aktif</span><span class="sxs-lookup"><span data-stu-id="58999-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="58999-103">Jika pengirim eksternal tidak dapat mengirim pesan ke folder publik yang mendukung email Anda, dan pengirim menerima kesalahan: **tidak dapat ditemukan (550 5.4.1)**, verifikasi domain email untuk folder publik dikonfigurasikan sebagai domain relay internal dan bukan domain otoritatif:</span><span class="sxs-lookup"><span data-stu-id="58999-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="58999-104">Buka [Pusat admin Exchange (eac)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="58999-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="58999-105">Masuk ke domain **email** yang \> **diterima**, pilih domain diterima, lalu klik **Edit**.</span><span class="sxs-lookup"><span data-stu-id="58999-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="58999-106">Di halaman properti yang terbuka, jika tipe domain diatur ke **otoritatif**, Ubah nilai ke **relay internal** lalu klik **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="58999-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="58999-107">Jika pengirim eksternal menerima kesalahan yang **tidak Anda miliki izin (550 5.7.13)**, jalankan perintah berikut di [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) untuk melihat izin untuk pengguna anonim dalam folder publik:</span><span class="sxs-lookup"><span data-stu-id="58999-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="58999-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Misalnya, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="58999-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="58999-109">Untuk memperbolehkan pengguna eksternal mengirim email ke folder publik ini, tambahkan akses CreateItems ke pengguna anonim.</span><span class="sxs-lookup"><span data-stu-id="58999-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="58999-110">Misalnya, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .</span><span class="sxs-lookup"><span data-stu-id="58999-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
