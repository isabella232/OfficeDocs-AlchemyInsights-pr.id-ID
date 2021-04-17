---
title: 'AIP: Kebijakan tidak seperti yang diharapkan'
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
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821630"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="963e0-102">AIP: Kebijakan tidak seperti yang diharapkan</span><span class="sxs-lookup"><span data-stu-id="963e0-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="963e0-103">Perlindungan Informasi Azure: Kebijakan yang tidak seperti yang diharapkan, lihat panduan yang disarankan untuk berbagai masalah kebijakan:</span><span class="sxs-lookup"><span data-stu-id="963e0-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="963e0-104">Jika Anda mengalami masalah dengan penandaan visual, [tinjau Ketika penandaan visual diterapkan.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="963e0-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="963e0-105">Jika Anda mengalami masalah dengan label otomatis, silakan tinjau Cara mengonfigurasi persyaratan klasifikasi otomatis dan direkomendasikan untuk Perlindungan Informasi [Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) dan Apa tipe informasi [sensitif mencari](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="963e0-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="963e0-106">Jika mengalami masalah dengan perlindungan Native/Pfile, silakan [tinjau konfigurasi File API](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="963e0-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="963e0-107">Periksa apakah Anda menggunakan kebijakan dengan lingkup yang tidak dikonfigurasi dengan benar: Cara mengonfigurasi kebijakan Perlindungan Informasi Azure untuk pengguna tertentu dengan menggunakan [kebijakan yang di lingkup.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)</span><span class="sxs-lookup"><span data-stu-id="963e0-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="963e0-108">Jika label otomatis tidak berfungsi untuk Outlook saat melampirkan dokumen berlabel, verifikasi bahwa DRMEncryptProperty tidak didefinisikan seperti yang diuraikan di sini: [Pengaturan registri IRM untuk keamanan.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)</span><span class="sxs-lookup"><span data-stu-id="963e0-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="963e0-109">Jika Anda masih mengalami masalah, silakan kumpulkan log klien Perlindungan Informasi Azure dan lampirkan log yang diekspor ke tiket ini.</span><span class="sxs-lookup"><span data-stu-id="963e0-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="963e0-110">Buka dokumen Office atau buat email baru di Outlook.</span><span class="sxs-lookup"><span data-stu-id="963e0-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="963e0-111">Klik **Proteksi/Bantuan**  >  **Sensitivitas dan umpan balik.**</span><span class="sxs-lookup"><span data-stu-id="963e0-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="963e0-112">Klik **Ekspor Log.**</span><span class="sxs-lookup"><span data-stu-id="963e0-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="963e0-113">Simpan log ke lokasi pilihan Anda, dan lampirkan log ke permintaan layanan ini.</span><span class="sxs-lookup"><span data-stu-id="963e0-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="963e0-114">Sumber daya tambahan:</span><span class="sxs-lookup"><span data-stu-id="963e0-114">Additional resources:</span></span>

- [<span data-ttu-id="963e0-115">Cara mengonfigurasi label untuk penandaan visual untuk Perlindungan Informasi Azure</span><span class="sxs-lookup"><span data-stu-id="963e0-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="963e0-116">Tinjau dokumentasi Perlindungan Informasi Azure</span><span class="sxs-lookup"><span data-stu-id="963e0-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="963e0-117">Menggunakan label sensitivitas di aplikasi Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="963e0-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

