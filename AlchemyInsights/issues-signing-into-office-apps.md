---
title: Masalah masuk ke aplikasi Microsoft 365
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
- "9000571"
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833006"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="b9478-102">Memperbaiki pesan "Modul Platform Tepercaya komputer Anda tidak berfungsi dengan baik" aplikasi Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b9478-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="b9478-103">Untuk memperbaiki kesalahan ini, coba hal berikut ini:</span><span class="sxs-lookup"><span data-stu-id="b9478-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="b9478-104">Instal pembaruan terkini untuk [Windows](https://support.microsoft.com/help/4027667/windows-10-update) dan [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="b9478-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="b9478-105">[Hapus kredensial Office menggunakan](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) Pengelola Kredensial Windows.</span><span class="sxs-lookup"><span data-stu-id="b9478-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="b9478-106">**Catatan:** Jalur registri untuk Office 2016 telah berubah menjadi 16.0.</span><span class="sxs-lookup"><span data-stu-id="b9478-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="b9478-107">(misalnya: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="b9478-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="b9478-108">Coba proses [pemulihan pengguna untuk](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) memperbaiki kegagalan Trusted Platform Module (TPM).</span><span class="sxs-lookup"><span data-stu-id="b9478-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="b9478-109">Atur EnableADAL = 0 menggunakan langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="b9478-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="b9478-110">Klik kanan tombol Mulai Windows, pilih **Jalankan**, ketik **regedit**, lalu pilih **OK.**</span><span class="sxs-lookup"><span data-stu-id="b9478-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="b9478-111">Pilih **Ya** untuk mengizinkan Editor Registri membuat perubahan ke perangkat Anda.</span><span class="sxs-lookup"><span data-stu-id="b9478-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="b9478-112">Di Editor Registri, tambahkan nilai DWORD dari **EnableADAL** dengan pengaturan **0 di bawah** HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="b9478-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="b9478-113">Untuk informasi selengkapnya, lihat Masalah koneksi masuk setelah pembaruan ke [Office 2016 build 16.0.7967 di Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="b9478-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>