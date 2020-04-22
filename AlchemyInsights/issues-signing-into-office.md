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
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763004"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="dda26-102">Masalah saat masuk ke aplikasi Office</span><span class="sxs-lookup"><span data-stu-id="dda26-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="dda26-103">Untuk memperbaiki masalah masuk dengan aplikasi Office, coba hal berikut:</span><span class="sxs-lookup"><span data-stu-id="dda26-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="dda26-104">Hapus semua akun kerja, kecuali akun yang terpengaruh, menggunakan pengaturan Windows > **akses kerja atau sekolah**.</span><span class="sxs-lookup"><span data-stu-id="dda26-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="dda26-105">[Hapus kredensial Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) yang menggunakan Pengelola mandat Windows.</span><span class="sxs-lookup"><span data-stu-id="dda26-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="dda26-106">**Catatan:** Lintasan registri untuk Office 2016 telah diubah ke 16,0.</span><span class="sxs-lookup"><span data-stu-id="dda26-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="dda26-107">(Mis: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="dda26-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="dda26-108">Buka aplikasi Office, pilih keluar **File** > **Account** > **dari**akun file. Kemudian masuk menggunakan akun pengguna dengan lisensi yang valid.</span><span class="sxs-lookup"><span data-stu-id="dda26-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="dda26-109">Untuk informasi mendetail, lihat [ akun di Office ](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="dda26-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="dda26-110">Untuk Mac, lihat [Tidak dapat masuk ke aplikasi Office 2016 untuk aplikasi Mac ](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="dda26-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="dda26-111">Jika kesalahan terjadi saat menyambung ke Microsoft 365 menggunakan Office 2013, aktifkan otentikasi modern untuk klien Office.</span><span class="sxs-lookup"><span data-stu-id="dda26-111">If the errors occurs while connecting to Microsoft 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="dda26-112">Untuk informasi selengkapnya, lihat:</span><span class="sxs-lookup"><span data-stu-id="dda26-112">For more information, see:</span></span>
- [<span data-ttu-id="dda26-113">Anda tidak dapat masuk ke Microsoft 365, Azure, atau Intune</span><span class="sxs-lookup"><span data-stu-id="dda26-113">You can't sign in to Microsoft 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="dda26-114">Masalah sambungan masuk setelah pembaruan untuk Office 2016 membangun 16.0.7967 di Windows 10</span><span class="sxs-lookup"><span data-stu-id="dda26-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="dda26-115">"Maaf, akun lain dari organisasi Anda sudah masuk di komputer ini" di Office</span><span class="sxs-lookup"><span data-stu-id="dda26-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="dda26-116">Memecahkan masalah masuk dengan otentikasi modern Office ketika Anda menggunakan ADFS</span><span class="sxs-lookup"><span data-stu-id="dda26-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)