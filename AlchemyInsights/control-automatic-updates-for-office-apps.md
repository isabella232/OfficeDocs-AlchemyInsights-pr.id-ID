---
title: Mengontrol pembaruan otomatis untuk aplikasi Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439334"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="68664-102">Mengontrol pembaruan otomatis untuk aplikasi Office</span><span class="sxs-lookup"><span data-stu-id="68664-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="68664-103">Secara default, pembaruan untuk aplikasi Office diunduh secara otomatis dan diterapkan di latar belakang tanpa campur tangan pengguna.</span><span class="sxs-lookup"><span data-stu-id="68664-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="68664-104">Namun, administrator dapat mengontrol cara pemutakhiran diterapkan dengan menggunakan pengaturan pemutakhiran Office.</span><span class="sxs-lookup"><span data-stu-id="68664-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="68664-105">Pengaturan pembaruan memungkinkan administrator untuk mengaktifkan atau menonaktifkan pembaruan otomatis, menampilkan atau menyembunyikan tombol **Perbarui sekarang** di Office, mengatur tenggat waktu pembaruan, dan banyak lagi.</span><span class="sxs-lookup"><span data-stu-id="68664-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="68664-106">Untuk informasi selengkapnya, lihat:</span><span class="sxs-lookup"><span data-stu-id="68664-106">For detailed information, see:</span></span>

- [<span data-ttu-id="68664-107">Mengkonfigurasi pengaturan pembaruan untuk Office</span><span class="sxs-lookup"><span data-stu-id="68664-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="68664-108">Pembaruan otomatis untuk Office tidak diaktifkan</span><span class="sxs-lookup"><span data-stu-id="68664-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="68664-109">Menentukan bagaimana Office diperbarui setelah diinstal</span><span class="sxs-lookup"><span data-stu-id="68664-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="68664-110">Untuk meninjau pengaturan pembaruan yang sudah ada yang diterapkan ke mesin klien, ikuti langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="68664-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="68664-111">Buka Registry Editor dengan pergi untuk **mulai**  >  **menjalankan**  >  **regedit**.</span><span class="sxs-lookup"><span data-stu-id="68664-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="68664-112">Beralih ke lokasi berikut dan Tinjau pengaturan pembaruan Office:</span><span class="sxs-lookup"><span data-stu-id="68664-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="68664-113">J.</span><span class="sxs-lookup"><span data-stu-id="68664-113">a.</span></span> <span data-ttu-id="68664-114">HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="68664-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="68664-115">B.</span><span class="sxs-lookup"><span data-stu-id="68664-115">b.</span></span> <span data-ttu-id="68664-116">ClickToRun\Configuration</span><span class="sxs-lookup"><span data-stu-id="68664-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="68664-117">**Catatan**  Jika kunci officemgmtcom diatur, Anda mungkin melihat pesan "pembaruan dikelola oleh administrator sistem Anda" di **Office**  >  **account**  >  **Office update**.</span><span class="sxs-lookup"><span data-stu-id="68664-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="68664-118">Untuk informasi lebih lanjut, lihat [mengelola pembaruan untuk microsoft 365 aplikasi dengan Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="68664-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  