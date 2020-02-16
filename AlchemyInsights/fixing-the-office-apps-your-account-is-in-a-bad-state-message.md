---
title: Memperbaiki aplikasi Office akun Anda berada dalam pesan status buruk
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969539"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="a1159-102">Memperbaiki aplikasi Office "akun Anda dalam keadaan buruk" galat</span><span class="sxs-lookup"><span data-stu-id="a1159-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="a1159-103">Untuk memperbaiki galat ini, cobalah opsi berikut ini di komputer yang terpengaruh:</span><span class="sxs-lookup"><span data-stu-id="a1159-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="a1159-104">Buka aplikasi Office, pilih**akun** >  **file** > **keluar dari semua akun**.</span><span class="sxs-lookup"><span data-stu-id="a1159-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="a1159-105">Masuk lagi menggunakan akun pengguna dengan lisensi yang valid.</span><span class="sxs-lookup"><span data-stu-id="a1159-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="a1159-106">Untuk informasi selengkapnya, lihat [akun di Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="a1159-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="a1159-107">[Hapus kredensial Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) yang menggunakan Pengelola mandat Windows.</span><span class="sxs-lookup"><span data-stu-id="a1159-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="a1159-108">**Catatan:** Lintasan registri untuk Office 2016 telah diubah ke 16,0.</span><span class="sxs-lookup"><span data-stu-id="a1159-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="a1159-109">Sebagai contoh, \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="a1159-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="a1159-110">Pada komputer yang terpengaruh, tetapkan EnableADAL = 0 dengan menggunakan langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="a1159-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="a1159-111">Klik kanan tombol Windows dan pilih **Jalankan**.</span><span class="sxs-lookup"><span data-stu-id="a1159-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="a1159-112">Di kotak **buka** , ketik **regedit**, dan kemudian pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="a1159-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="a1159-113">Pilih **ya** saat diminta untuk mengizinkan Penyunting registri untuk membuat perubahan pada perangkat Anda.</span><span class="sxs-lookup"><span data-stu-id="a1159-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="a1159-114">Di Penyunting registri, tambahkan nilai DWORD EnableADAL dengan pengaturan 0 di bawah HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="a1159-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="a1159-115">Jika galat terjadi saat menyambung ke Office 365 menggunakan Office 2013, [aktifkan otentikasi modern](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) untuk klien Office.</span><span class="sxs-lookup"><span data-stu-id="a1159-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="a1159-116">Untuk informasi selengkapnya, lihat [bagaimana cara memecahkan masalah aplikasi non-browser yang tidak dapat masuk ke Office 365, Azure, atau Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="a1159-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

