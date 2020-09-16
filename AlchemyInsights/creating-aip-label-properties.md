---
title: Membuat kebijakan label AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732178"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="d6a63-102">Membuat kebijakan label AIP</span><span class="sxs-lookup"><span data-stu-id="d6a63-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="d6a63-103">Label proteksi informasi Azure (AIP) dapat digunakan dengan rentang data lengkap yang biasanya dibuat dan disimpan oleh organisasi, dari klasifikasi data pribadi terendah hingga klasifikasi tertinggi dari data yang sangat rahasia.</span><span class="sxs-lookup"><span data-stu-id="d6a63-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="d6a63-104">Kebijakan perlindungan informasi Azure berlaku untuk klien klasik Azure Information Protection (AIP) dan bukan  [klien pelabelan terpadu AIP](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="d6a63-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="d6a63-105">Anda dapat mengonfigurasi beberapa elemen dalam kebijakan AIP, termasuk opsi seperti:</span><span class="sxs-lookup"><span data-stu-id="d6a63-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="d6a63-106">Opsi untuk label mana yang akan memungkinkan administrator atau pengguna mengklasifikasikan dan mengirim dokumen (opsional) dan email</span><span class="sxs-lookup"><span data-stu-id="d6a63-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="d6a63-107">Opsi untuk menerapkan klasifikasi saat pengguna menyimpan dokumen dan mengirim email</span><span class="sxs-lookup"><span data-stu-id="d6a63-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="d6a63-108">Opsi untuk secara otomatis memberi label pesan email, berdasarkan lampirannya.</span><span class="sxs-lookup"><span data-stu-id="d6a63-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="d6a63-109">Opsi untuk mengontrol apakah bilah proteksi informasi ditampilkan di aplikasi Office</span><span class="sxs-lookup"><span data-stu-id="d6a63-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="d6a63-110">Untuk opsi dan informasi tambahan tentang kebijakan perlindungan informasi Azure, lihat: [gambaran umum kebijakan proteksi informasi Azure](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="d6a63-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="d6a63-111">Untuk sumber daya yang bermanfaat lainnya terkait kebijakan RAKUTEN Insight, lihat:</span><span class="sxs-lookup"><span data-stu-id="d6a63-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="d6a63-112">Tutorial: mengonfigurasi pengaturan kebijakan proteksi informasi Azure dan membuat label baru</span><span class="sxs-lookup"><span data-stu-id="d6a63-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="d6a63-113">Mengonfigurasi kebijakan perlindungan informasi Azure</span><span class="sxs-lookup"><span data-stu-id="d6a63-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="d6a63-114">Membuat dan mengonfigurasikan label sensitivitas dan kebijakannya</span><span class="sxs-lookup"><span data-stu-id="d6a63-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="d6a63-115">Panduan cara penggunaan untuk skenario umum yang menggunakan perlindungan informasi Azure</span><span class="sxs-lookup"><span data-stu-id="d6a63-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="d6a63-116">Meninjau dokumentasi perlindungan informasi Azure</span><span class="sxs-lookup"><span data-stu-id="d6a63-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="d6a63-117">Persyaratan untuk proteksi informasi Azure</span><span class="sxs-lookup"><span data-stu-id="d6a63-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="d6a63-118">Tutorial mulai cepat untuk proteksi informasi Azure</span><span class="sxs-lookup"><span data-stu-id="d6a63-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="d6a63-119">Unduh klien perlindungan informasi Azure</span><span class="sxs-lookup"><span data-stu-id="d6a63-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)