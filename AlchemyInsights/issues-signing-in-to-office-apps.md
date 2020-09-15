---
title: Masalah masuk ke aplikasi Microsoft 365
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
- "9000571"
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695326"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="e0e01-102">Memperbaiki aplikasi Microsoft 365 "Maaf, akun lain dari organisasi Anda sudah masuk"</span><span class="sxs-lookup"><span data-stu-id="e0e01-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="e0e01-103">Untuk memperbaiki kesalahan ini, coba hal berikut ini:</span><span class="sxs-lookup"><span data-stu-id="e0e01-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="e0e01-104">Hapus semua akun kerja, kecuali akun yang terpengaruh, menggunakan pengaturan Windows > **mengakses kantor atau sekolah**.</span><span class="sxs-lookup"><span data-stu-id="e0e01-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="e0e01-105">[Kosongkan kredensial Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) menggunakan Pengelola kredensial Windows.</span><span class="sxs-lookup"><span data-stu-id="e0e01-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="e0e01-106">**Catatan:** Jalur registri untuk Office 2016 telah diubah ke 16,0.</span><span class="sxs-lookup"><span data-stu-id="e0e01-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="e0e01-107">(Mis: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="e0e01-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="e0e01-108">Buka aplikasi Office, pilih akun **file**  >  **Account**  >  **keluar**. Lalu masuk menggunakan akun pengguna dengan lisensi yang valid.</span><span class="sxs-lookup"><span data-stu-id="e0e01-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="e0e01-109">Untuk informasi mendetail, lihat [ akun di Office ](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="e0e01-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="e0e01-110">Untuk Mac, lihat [Tidak dapat masuk ke aplikasi Office 2016 untuk aplikasi Mac ](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="e0e01-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="e0e01-111">Untuk informasi selengkapnya, lihat ["Maaf, akun lain dari organisasi Anda sudah masuk di komputer ini" di Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="e0e01-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>