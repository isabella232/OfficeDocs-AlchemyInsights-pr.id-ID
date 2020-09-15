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
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695290"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="991f8-102">Layar masuk kosong di aplikasi Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="991f8-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="991f8-103">Untuk memperbaiki masalah ini, cobalah yang berikut ini:</span><span class="sxs-lookup"><span data-stu-id="991f8-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="991f8-104">Instal pembaruan terbaru untuk [Windows](https://support.microsoft.com/help/4027667/windows-10-update) dan [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="991f8-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="991f8-105">Reset Opsi Internet Explorer: masuk ke **Tools**  >  **Opsi Internet**Tools  >  **Advanced**  >  **reset pengaturan Internet Explorer** (Perhatikan bahwa Anda akan kehilangan pengaturan kustom), lalu coba masuk ke Office lagi.</span><span class="sxs-lookup"><span data-stu-id="991f8-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="991f8-106">Nonaktifkan Windows Defender Application Guard (WDAG) atau program firewall atau antivirus yang sama:</span><span class="sxs-lookup"><span data-stu-id="991f8-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="991f8-107">Di panel kontrol, masuk ke **program**, lalu pilih **Aktifkan atau nonaktifkan fitur Windows**.</span><span class="sxs-lookup"><span data-stu-id="991f8-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="991f8-108">Jika Windows Defender Application Guard diaktifkan, coba Nonaktifkan.</span><span class="sxs-lookup"><span data-stu-id="991f8-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="991f8-109">**Catatan:** Anda mungkin perlu memulai ulang komputer.</span><span class="sxs-lookup"><span data-stu-id="991f8-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="991f8-110">Pastikan bahwa plugin Microsoft. AAD. broker [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) tidak diblokir oleh aplikasi atau firewall/program antivirus.</span><span class="sxs-lookup"><span data-stu-id="991f8-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="991f8-111">[Kosongkan kredensial Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) menggunakan Pengelola kredensial Windows.</span><span class="sxs-lookup"><span data-stu-id="991f8-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="991f8-112">**Catatan:** Jalur registri untuk Office 2016 telah diubah ke 16,0.</span><span class="sxs-lookup"><span data-stu-id="991f8-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="991f8-113">(Mis: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="991f8-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="991f8-114">Untuk informasi selengkapnya, lihat [masalah koneksi di masuk setelah pembaruan ke Office 2016 Build 16.0.7967 di Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="991f8-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>