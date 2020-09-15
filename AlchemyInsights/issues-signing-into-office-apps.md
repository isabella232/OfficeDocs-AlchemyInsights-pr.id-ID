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
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695182"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="bd608-102">Memperbaiki aplikasi Microsoft 365 "modul platform tepercaya komputer Anda tidak berfungsi dengan benar"</span><span class="sxs-lookup"><span data-stu-id="bd608-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="bd608-103">Untuk memperbaiki kesalahan ini, coba hal berikut ini:</span><span class="sxs-lookup"><span data-stu-id="bd608-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="bd608-104">Instal pembaruan terbaru untuk [Windows](https://support.microsoft.com/help/4027667/windows-10-update) dan [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="bd608-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="bd608-105">[Kosongkan kredensial Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) menggunakan Pengelola kredensial Windows.</span><span class="sxs-lookup"><span data-stu-id="bd608-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="bd608-106">**Catatan:** Jalur registri untuk Office 2016 telah diubah ke 16,0.</span><span class="sxs-lookup"><span data-stu-id="bd608-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="bd608-107">(Mis: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="bd608-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="bd608-108">Cobalah [proses pemulihan pengguna](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) untuk memperbaiki kegagalan Trusted platform Module (TPM).</span><span class="sxs-lookup"><span data-stu-id="bd608-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="bd608-109">Atur EnableADAL = 0 menggunakan langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="bd608-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="bd608-110">Klik kanan tombol mulai Windows, pilih **Jalankan**, ketik **regedit**, lalu pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="bd608-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="bd608-111">Pilih **ya** untuk memperbolehkan editor registri membuat perubahan pada perangkat Anda.</span><span class="sxs-lookup"><span data-stu-id="bd608-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="bd608-112">Dalam editor registri, tambahkan nilai DWORD **Enableadal** dengan pengaturan **0** di bawah HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="bd608-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="bd608-113">Untuk informasi selengkapnya, lihat [masalah koneksi di masuk setelah pembaruan ke Office 2016 Build 16.0.7967 di Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="bd608-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>