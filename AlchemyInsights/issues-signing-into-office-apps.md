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
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938248"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="0ee12-102">Memperbaiki pesan kantor apps "modul terpercaya Platform komputer Anda tidak berfungsi dengan benar"</span><span class="sxs-lookup"><span data-stu-id="0ee12-102">Fixing the Office apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="0ee12-103">Untuk memperbaiki kesalahan ini, coba langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="0ee12-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="0ee12-104">Menginstal update terbaru untuk [Windows](https://support.microsoft.com/help/4027667/windows-10-update) dan [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="0ee12-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="0ee12-105">[Jelas kantor kredensial](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) menggunakan Windows Credential Manager.</span><span class="sxs-lookup"><span data-stu-id="0ee12-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="0ee12-106">**Catatan:** Jalur registri untuk kantor 2016 telah berubah untuk 16.0.</span><span class="sxs-lookup"><span data-stu-id="0ee12-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="0ee12-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="0ee12-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="0ee12-108">Mencoba [proses pemulihan pengguna](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) untuk memperbaiki kegagalan dipercaya Platform modul (TPM).</span><span class="sxs-lookup"><span data-stu-id="0ee12-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="0ee12-109">Menetapkan EnableADAL = 0 menggunakan langkah-langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="0ee12-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="0ee12-110">Klik kanan tombol mulai Windows, memilih **Jalankan**, ketik **regedit**dan kemudian pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="0ee12-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="0ee12-111">Pilih **ya** untuk memungkinkan Registry Editor untuk membuat perubahan ke perangkat Anda.</span><span class="sxs-lookup"><span data-stu-id="0ee12-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="0ee12-112">Di Penyunting registri, menambahkan nilai DWORD **EnableADAL** dengan suasana **0** di bawah HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="0ee12-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="0ee12-113">Untuk selengkapnya, lihat [sambungan isu-isu dalam masuk setelah update ke kantor 2016 membangun 16.0.7967 pada Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="0ee12-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>