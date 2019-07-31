---
title: Masalah saat masuk ke aplikasi Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: de0a1b78724db9a8e93d8d599ce3b503abcb86e2
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938245"
---
# <a name="fixing-the-office-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="c9e23-102">Memperbaiki pesan "Maaf, account yang lain dari organisasi Anda sudah masuk" aplikasi kantor</span><span class="sxs-lookup"><span data-stu-id="c9e23-102">Fixing the Office apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="c9e23-103">Untuk memperbaiki kesalahan ini, coba langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="c9e23-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="c9e23-104">Menghapus semua pekerjaan account, kecuali account yang terkena, menggunakan > Windows pengaturan **akses kerja atau sekolah**.</span><span class="sxs-lookup"><span data-stu-id="c9e23-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="c9e23-105">[Jelas kantor kredensial](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) menggunakan Windows Credential Manager.</span><span class="sxs-lookup"><span data-stu-id="c9e23-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="c9e23-106">**Catatan:** Jalur registri untuk kantor 2016 telah berubah untuk 16.0.</span><span class="sxs-lookup"><span data-stu-id="c9e23-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="c9e23-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="c9e23-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="c9e23-108">Buka aplikasi kantor, pilih **File** > **Account** > **Sign Out**. Kemudian masuk menggunakan account pengguna dengan lisensi berlaku.</span><span class="sxs-lookup"><span data-stu-id="c9e23-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="c9e23-109">Untuk informasi rinci, lihat [account di kantor](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="c9e23-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="c9e23-110">Untuk Mac, lihat [tidak dapat masuk ke kantor 2016 untuk Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="c9e23-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="c9e23-111">Untuk informasi lebih lanjut, lihat ["Maaf, account yang lain dari organisasi Anda telah masuk di komputer ini" di kantor](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="c9e23-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>