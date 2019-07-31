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
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938246"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="49ed3-102">Masalah saat masuk ke aplikasi Office</span><span class="sxs-lookup"><span data-stu-id="49ed3-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="49ed3-103">Untuk memperbaiki masalah masuk dengan kantor apps, cobalah berikut ini:</span><span class="sxs-lookup"><span data-stu-id="49ed3-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="49ed3-104">Menghapus semua pekerjaan account, kecuali account yang terkena, menggunakan > Windows pengaturan **akses kerja atau sekolah**.</span><span class="sxs-lookup"><span data-stu-id="49ed3-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="49ed3-105">[Jelas kantor kredensial](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) menggunakan Windows Credential Manager.</span><span class="sxs-lookup"><span data-stu-id="49ed3-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="49ed3-106">**Catatan:** Jalur registri untuk kantor 2016 telah berubah untuk 16.0.</span><span class="sxs-lookup"><span data-stu-id="49ed3-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="49ed3-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="49ed3-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="49ed3-108">Buka aplikasi kantor, pilih **File** > **Account** > **Sign Out**. Kemudian masuk menggunakan account pengguna dengan lisensi berlaku.</span><span class="sxs-lookup"><span data-stu-id="49ed3-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="49ed3-109">Untuk informasi rinci, lihat [account di kantor](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="49ed3-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="49ed3-110">Untuk Mac, lihat [tidak dapat masuk ke kantor 2016 untuk Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="49ed3-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="49ed3-111">Jika kesalahan terjadi saat menghubungkan ke Office 365 menggunakan kantor 2013, mengaktifkan otentikasi modern untuk kantor klien.</span><span class="sxs-lookup"><span data-stu-id="49ed3-111">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="49ed3-112">Untuk informasi selengkapnya, lihat:</span><span class="sxs-lookup"><span data-stu-id="49ed3-112">For more information, see:</span></span>
- [<span data-ttu-id="49ed3-113">Anda tidak dapat masuk ke kantor 365, Azure, atau Intune</span><span class="sxs-lookup"><span data-stu-id="49ed3-113">You can't sign in to Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="49ed3-114">Masalah sambungan di masuk setelah update ke kantor 2016 membangun 16.0.7967 Windows 10</span><span class="sxs-lookup"><span data-stu-id="49ed3-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="49ed3-115">"Maaf, account yang lain dari organisasi Anda telah masuk di komputer ini" di kantor</span><span class="sxs-lookup"><span data-stu-id="49ed3-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="49ed3-116">Memecahkan masalah masuk dengan kantor modern otentikasi ketika Anda menggunakan ADFS</span><span class="sxs-lookup"><span data-stu-id="49ed3-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)