---
title: 'Pemindai AIP: penginstalan dan konfigurasi'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821666"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="a534d-102">Pemindai AIP: penginstalan dan konfigurasi</span><span class="sxs-lookup"><span data-stu-id="a534d-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="a534d-103">**Untuk menginstal pemindai AIP, ikuti panduan yang disarankan:**</span><span class="sxs-lookup"><span data-stu-id="a534d-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="a534d-104">Jika Anda memutakhirkan dan tidak melakukan penginstalan yang bersih, pastikan Anda telah mengikuti panduan untuk memutakhirkan pemindai Perlindungan Informasi Azure dan untuk klien label yang terpadu, lihat memutakhirkan pemindai [Perlindungan](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)Informasi [Azure.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner)</span><span class="sxs-lookup"><span data-stu-id="a534d-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="a534d-105">Verifikasi bahwa Anda mematuhi semua [persyaratan pengaturan infrastruktur jaringan dan Firewall.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)</span><span class="sxs-lookup"><span data-stu-id="a534d-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="a534d-106">Pastikan kebijakan [Anda diatur ke](https://docs.microsoft.com/azure/information-protection/configure-policy) label otomatis atau memiliki label default di kebijakan tersebut.</span><span class="sxs-lookup"><span data-stu-id="a534d-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="a534d-107">Pastikan bahwa tipe file yang relevan dikonfigurasi untuk label/proteksi seperti yang dijelaskan dalam [Tipe file yang didukung oleh klien Perlindungan Informasi Azure.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)</span><span class="sxs-lookup"><span data-stu-id="a534d-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="a534d-108">Selain itu, jika ingin mengubah perilaku default, ikuti panduan berikut: [Mengubah tingkat proteksi default file](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="a534d-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="a534d-109">Verifikasi bahwa akun pengguna yang dikonfigurasi untuk menjalankan layanan pemindai memiliki izin untuk mengakses semua penyimpanan yang dikonfigurasi.</span><span class="sxs-lookup"><span data-stu-id="a534d-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="a534d-110">Jika Anda masih mengalami masalah, silakan ekspor log pemindai dan tambahkan ke tiket dukungan Anda.</span><span class="sxs-lookup"><span data-stu-id="a534d-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="a534d-111">**Mengekspor log Pemindai Perlindungan Informasi Azure**</span><span class="sxs-lookup"><span data-stu-id="a534d-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="a534d-112">Navigasikan ke %localappdata%\Microsoft\MSIP di bawah konteks pengguna yang menjalankan layanan pemindai.</span><span class="sxs-lookup"><span data-stu-id="a534d-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="a534d-113">Zip semua konten di bawah folder MSIP.</span><span class="sxs-lookup"><span data-stu-id="a534d-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="a534d-114">Simpan log ke lokasi pilihan, lalu lampirkan ke permintaan layanan Anda.</span><span class="sxs-lookup"><span data-stu-id="a534d-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="a534d-115">Anda juga bisa menggunakan [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="a534d-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="a534d-116">**Untuk informasi tambahan, lihat:**</span><span class="sxs-lookup"><span data-stu-id="a534d-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="a534d-117">Menyebarkan pemindai Perlindungan Informasi Azure untuk mengklasifikasikan dan melindungi file secara otomatis</span><span class="sxs-lookup"><span data-stu-id="a534d-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="a534d-118">Menentukan dan menggunakan parameter Token untuk Set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="a534d-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="a534d-119">Menjalankan siklus penemuan dan menampilkan laporan untuk pemindai</span><span class="sxs-lookup"><span data-stu-id="a534d-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="a534d-120">Tinjau dokumentasi Perlindungan Informasi Azure</span><span class="sxs-lookup"><span data-stu-id="a534d-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="a534d-121">Persyaratan untuk Perlindungan Informasi Azure</span><span class="sxs-lookup"><span data-stu-id="a534d-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="a534d-122">Unduh klien Perlindungan Informasi Azure</span><span class="sxs-lookup"><span data-stu-id="a534d-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
