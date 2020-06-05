---
title: Masalah saat masuk ke aplikasi Microsoft 365
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
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579904"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="2ba6e-102">Layar masuk kosong di Microsoft 365 aplikasi</span><span class="sxs-lookup"><span data-stu-id="2ba6e-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="2ba6e-103">Untuk memperbaiki masalah ini, cobalah berikut ini:</span><span class="sxs-lookup"><span data-stu-id="2ba6e-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="2ba6e-104">Instal pemutakhiran terbaru untuk [Windows](https://support.microsoft.com/help/4027667/windows-10-update) dan [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="2ba6e-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="2ba6e-105">Reset Internet Explorer Options: pergi ke **alat**  >  **Internet Options**  >  **lanjutan**  >  **reset Internet Explorer pengaturan** (Perhatikan bahwa Anda akan kehilangan pengaturan kustom), dan kemudian coba masuk ke kantor lagi.</span><span class="sxs-lookup"><span data-stu-id="2ba6e-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="2ba6e-106">Nonaktifkan Windows Defender Application Guard (WDAG) atau program firewall atau anti-virus yang serupa:</span><span class="sxs-lookup"><span data-stu-id="2ba6e-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="2ba6e-107">Di panel kontrol, pergi ke **program**, dan kemudian pilih **fitur Windows mengaktifkan atau menonaktifkan**.</span><span class="sxs-lookup"><span data-stu-id="2ba6e-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="2ba6e-108">Jika pelindung aplikasi Windows Defender diaktifkan, cobalah menonaktifkannya.</span><span class="sxs-lookup"><span data-stu-id="2ba6e-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="2ba6e-109">**Catatan:** Anda mungkin perlu me-restart komputer.</span><span class="sxs-lookup"><span data-stu-id="2ba6e-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="2ba6e-110">Pastikan bahwa Microsoft. AAD. broker plugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) tidak sedang diblokir oleh aplikasi atau firewall/anti-virus program.</span><span class="sxs-lookup"><span data-stu-id="2ba6e-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="2ba6e-111">[Hapus kredensial Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) yang menggunakan Pengelola mandat Windows.</span><span class="sxs-lookup"><span data-stu-id="2ba6e-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="2ba6e-112">**Catatan:** Lintasan registri untuk Office 2016 telah diubah ke 16,0.</span><span class="sxs-lookup"><span data-stu-id="2ba6e-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="2ba6e-113">(Mis: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="2ba6e-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="2ba6e-114">Untuk informasi selengkapnya, lihat [masalah sambungan di masuk setelah pembaruan ke Office 2016 membangun 16.0.7967 di Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="2ba6e-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>