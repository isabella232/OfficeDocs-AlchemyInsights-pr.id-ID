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
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833042"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="9965e-102">Layar masuk kosong di aplikasi Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="9965e-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="9965e-103">Untuk memperbaiki masalah ini, cobalah hal berikut:</span><span class="sxs-lookup"><span data-stu-id="9965e-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="9965e-104">Instal pembaruan terkini untuk [Windows](https://support.microsoft.com/help/4027667/windows-10-update) dan [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="9965e-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="9965e-105">Mengatur ulang opsi Internet Explorer: Masuk ke Alat Opsi Internet Reset Pengaturan Internet Explorer Tingkat Lanjut (perhatikan bahwa Anda akan kehilangan pengaturan kustom), lalu coba masuk lagi  >    >    >   ke Office.</span><span class="sxs-lookup"><span data-stu-id="9965e-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="9965e-106">Menonaktifkan Application Guard Pertahanan Windows (WKAL, Application Guard) atau program antivirus atau firewall yang serupa:</span><span class="sxs-lookup"><span data-stu-id="9965e-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="9965e-107">Di Panel Kontrol, masuk **ke Program**, lalu pilih Aktifkan **atau nonaktifkan fitur Windows**.</span><span class="sxs-lookup"><span data-stu-id="9965e-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="9965e-108">Jika Application Guard Pertahanan Windows diaktifkan, coba nonaktifkan.</span><span class="sxs-lookup"><span data-stu-id="9965e-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="9965e-109">**Catatan:** Anda mungkin perlu memulai ulang komputer.</span><span class="sxs-lookup"><span data-stu-id="9965e-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="9965e-110">Pastikan bahwa plug-in Microsoft.AAD.BrokerPlugin [AAD WAM tidak](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) diblokir oleh program aplikasi atau firewall/antivirus apa pun.</span><span class="sxs-lookup"><span data-stu-id="9965e-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="9965e-111">[Hapus kredensial Office menggunakan](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Pengelola Kredensial Windows.</span><span class="sxs-lookup"><span data-stu-id="9965e-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="9965e-112">**Catatan:** Jalur registri untuk Office 2016 telah berubah menjadi 16.0.</span><span class="sxs-lookup"><span data-stu-id="9965e-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="9965e-113">(misalnya: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="9965e-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="9965e-114">Untuk informasi selengkapnya, lihat Masalah koneksi masuk setelah pembaruan ke [Office 2016 build 16.0.7967 di Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="9965e-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>