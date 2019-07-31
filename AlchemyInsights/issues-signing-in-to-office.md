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
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938247"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="2d203-102">Masuk layar kosong di Office apps</span><span class="sxs-lookup"><span data-stu-id="2d203-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="2d203-103">Untuk mengatasi masalah ini, cobalah berikut ini:</span><span class="sxs-lookup"><span data-stu-id="2d203-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="2d203-104">Menginstal update terbaru untuk [Windows](https://support.microsoft.com/help/4027667/windows-10-update) dan [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="2d203-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="2d203-105">Mengatur ulang Internet Explorer pilihan: pergi ke **Tools** > **Internet Options** > **Advanced** > **Reset tataan Internet Explorer** (Perhatikan bahwa Anda akan kehilangan pengaturan), dan kemudian mencoba masuk ke kantor lagi.</span><span class="sxs-lookup"><span data-stu-id="2d203-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="2d203-106">Menonaktifkan Windows Defender aplikasi penjaga (WDAG) atau program serupa firewall atau antivirus:</span><span class="sxs-lookup"><span data-stu-id="2d203-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="2d203-107">Di Panel kontrol, pergi ke **program**, dan kemudian memilih **fitur Windows mengubah atau mati**.</span><span class="sxs-lookup"><span data-stu-id="2d203-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="2d203-108">Jika Windows Defender aplikasi Guard diaktifkan, coba Nonaktifkan.</span><span class="sxs-lookup"><span data-stu-id="2d203-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="2d203-109">**Catatan:** Anda mungkin perlu me-restart komputer.</span><span class="sxs-lookup"><span data-stu-id="2d203-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="2d203-110">Memastikan bahwa Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) tidak sedang diblokir oleh firewall/anti-anti-virus program atau aplikasi apapun.</span><span class="sxs-lookup"><span data-stu-id="2d203-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="2d203-111">[Jelas kantor kredensial](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) menggunakan Windows Credential Manager.</span><span class="sxs-lookup"><span data-stu-id="2d203-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="2d203-112">**Catatan:** Jalur registri untuk kantor 2016 telah berubah untuk 16.0.</span><span class="sxs-lookup"><span data-stu-id="2d203-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="2d203-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="2d203-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="2d203-114">Untuk selengkapnya, lihat [sambungan isu-isu dalam masuk setelah update ke kantor 2016 membangun 16.0.7967 pada Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="2d203-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>