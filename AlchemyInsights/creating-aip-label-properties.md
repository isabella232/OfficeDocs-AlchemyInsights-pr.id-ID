---
title: Membuat kebijakan label AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569204"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="c43a7-102">Membuat kebijakan label AIP</span><span class="sxs-lookup"><span data-stu-id="c43a7-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="c43a7-103">Label perlindungan informasi Azure (AIP) dapat digunakan dengan berbagai data yang biasanya dibuat organisasi dan toko, mulai dari klasifikasi data pribadi terendah hingga klasifikasi tertinggi data yang sangat rahasia.</span><span class="sxs-lookup"><span data-stu-id="c43a7-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="c43a7-104">Kebijakan perlindungan informasi Azure berlaku untuk klien klasik perlindungan informasi Azure (AIP) dan bukan [klien AIP terpadu pelabelan](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="c43a7-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="c43a7-105">Anda dapat mengonfigurasi beberapa elemen dalam kebijakan AIP, termasuk opsi seperti:</span><span class="sxs-lookup"><span data-stu-id="c43a7-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="c43a7-106">Pilihan untuk label yang akan membiarkan administrator atau pengguna mengklasifikasikan dan perlindungan (opsional) dokumen dan email</span><span class="sxs-lookup"><span data-stu-id="c43a7-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="c43a7-107">Pilihan untuk menegakkan klasifikasi ketika pengguna menyimpan dokumen dan mengirim email</span><span class="sxs-lookup"><span data-stu-id="c43a7-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="c43a7-108">Pilihan untuk secara otomatis memberi label pesan email, berdasarkan lampirannya.</span><span class="sxs-lookup"><span data-stu-id="c43a7-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="c43a7-109">Opsi untuk mengontrol apakah bilah perlindungan informasi ditampilkan di aplikasi Office</span><span class="sxs-lookup"><span data-stu-id="c43a7-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="c43a7-110">Untuk opsi tambahan dan informasi tentang kebijakan perlindungan informasi Azure, lihat: [Ikhtisar kebijakan perlindungan informasi Azure](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="c43a7-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="c43a7-111">Untuk sumber daya bermanfaat lainnya mengenai kebijakan AIP, lihat:</span><span class="sxs-lookup"><span data-stu-id="c43a7-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="c43a7-112">Tutorial: mengkonfigurasi pengaturan kebijakan perlindungan informasi Azure dan membuat label baru</span><span class="sxs-lookup"><span data-stu-id="c43a7-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="c43a7-113">Mengonfigurasi kebijakan perlindungan informasi Azure</span><span class="sxs-lookup"><span data-stu-id="c43a7-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="c43a7-114">Membuat dan mengonfigurasi label sensitivitas dan kebijakan mereka</span><span class="sxs-lookup"><span data-stu-id="c43a7-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="c43a7-115">Panduan cara untuk skenario umum yang menggunakan perlindungan informasi Azure</span><span class="sxs-lookup"><span data-stu-id="c43a7-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="c43a7-116">Tinjau dokumentasi perlindungan informasi Azure</span><span class="sxs-lookup"><span data-stu-id="c43a7-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="c43a7-117">Persyaratan untuk perlindungan informasi Azure</span><span class="sxs-lookup"><span data-stu-id="c43a7-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="c43a7-118">Tutorial memulai cepat untuk perlindungan informasi Azure</span><span class="sxs-lookup"><span data-stu-id="c43a7-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="c43a7-119">Unduh klien perlindungan informasi Azure</span><span class="sxs-lookup"><span data-stu-id="c43a7-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)