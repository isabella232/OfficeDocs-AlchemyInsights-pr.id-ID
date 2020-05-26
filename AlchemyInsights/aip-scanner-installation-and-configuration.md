---
title: 'AIP scanner: instalasi dan konfigurasi'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358099"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="344cc-102">AIP scanner: instalasi dan konfigurasi</span><span class="sxs-lookup"><span data-stu-id="344cc-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="344cc-103">**Untuk memasang pemindai AIP, ikuti pedoman yang disarankan**:</span><span class="sxs-lookup"><span data-stu-id="344cc-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="344cc-104">Jika Anda meningkatkan dan tidak melakukan instalasi bersih, pastikan Anda telah mengikuti panduan untuk [meningkatkan pemindai perlindungan informasi Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) dan untuk klien pelabelan terpadu, lihat [meningkatkan pemindai perlindungan informasi Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="344cc-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="344cc-105">Verifikasi bahwa Anda mematuhi semua [firewall dan persyaratan pengaturan infrastruktur jaringan](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span><span class="sxs-lookup"><span data-stu-id="344cc-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="344cc-106">Pastikan kebijakan Anda [ditetapkan](https://docs.microsoft.com/azure/information-protection/configure-policy) ke pelabelan otomatis atau memiliki label default dalam kebijakan.</span><span class="sxs-lookup"><span data-stu-id="344cc-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="344cc-107">Pastikan bahwa jenis berkas yang relevan dikonfigurasi untuk label/perlindungan seperti yang dijelaskan dalam [jenis berkas yang didukung oleh klien perlindungan informasi Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="344cc-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="344cc-108">Selain itu, jika Anda ingin mengubah perilaku default, ikuti panduan berikut: [mengubah tingkat perlindungan default file](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="344cc-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="344cc-109">Verifikasikan bahwa akun pengguna yang dikonfigurasi untuk menjalankan layanan pemindai memiliki izin untuk mengakses semua repositori yang dikonfigurasi.</span><span class="sxs-lookup"><span data-stu-id="344cc-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="344cc-110">Jika Anda masih mengalami masalah, silakan ekspor log pemindai dan menambahkannya ke tiket dukungan Anda.</span><span class="sxs-lookup"><span data-stu-id="344cc-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="344cc-111">**Ekspor log perlindungan informasi Azure**</span><span class="sxs-lookup"><span data-stu-id="344cc-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="344cc-112">Navigasikan ke%localappdata%\Microsoft\MSIP di bawah konteks pengguna yang menjalankan layanan pemindai.</span><span class="sxs-lookup"><span data-stu-id="344cc-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="344cc-113">Zip semua isi di bawah MSIP folder.</span><span class="sxs-lookup"><span data-stu-id="344cc-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="344cc-114">Simpan log ke pilihan lokasi Anda, dan pasangkan ke permintaan layanan Anda.</span><span class="sxs-lookup"><span data-stu-id="344cc-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="344cc-115">Anda juga dapat menggunakan [ekspor-AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="344cc-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="344cc-116">**Untuk informasi tambahan, lihat**:</span><span class="sxs-lookup"><span data-stu-id="344cc-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="344cc-117">Menyebarkan pemindai perlindungan informasi Azure untuk secara otomatis mengklasifikasikan dan melindungi file</span><span class="sxs-lookup"><span data-stu-id="344cc-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="344cc-118">Tentukan dan Gunakan token parameter untuk set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="344cc-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="344cc-119">Menjalankan penemuan siklus dan melihat laporan untuk pemindai</span><span class="sxs-lookup"><span data-stu-id="344cc-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="344cc-120">Tinjau dokumentasi perlindungan informasi Azure</span><span class="sxs-lookup"><span data-stu-id="344cc-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="344cc-121">Persyaratan untuk perlindungan informasi Azure</span><span class="sxs-lookup"><span data-stu-id="344cc-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="344cc-122">Unduh klien perlindungan informasi Azure</span><span class="sxs-lookup"><span data-stu-id="344cc-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
