---
title: 'AIP: kebijakan tidak berperilaku seperti yang diharapkan'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7926ff9ebbd54969fb5b3ae5d909baffe96a4292
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493159"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="142cd-102">AIP: kebijakan tidak berperilaku seperti yang diharapkan</span><span class="sxs-lookup"><span data-stu-id="142cd-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="142cd-103">Perlindungan informasi Azure: kebijakan yang tidak berperilaku seperti yang diharapkan, lihat berikut ini untuk panduan yang disarankan untuk berbagai masalah kebijakan:</span><span class="sxs-lookup"><span data-stu-id="142cd-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="142cd-104">Jika Anda mengalami masalah dengan tanda visual, silakan Tinjau [saat tanda visual diterapkan](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="142cd-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="142cd-105">Jika Anda mengalami masalah dengan pelabelan otomatis, Tinjau [cara mengonfigurasi ketentuan untuk klasifikasi otomatis dan direkomendasikan untuk perlindungan informasi Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) dan [apa yang dicari oleh jenis informasi sensitif](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="142cd-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>
3. <span data-ttu-id="142cd-106">Jika Anda mengalami masalah dengan perlindungan Native/Pfile, silakan Tinjau [konfigurasi file api](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="142cd-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="142cd-107">Periksa apakah Anda menggunakan kebijakan scoped yang tidak dikonfigurasi dengan benar: [cara mengkonfigurasi kebijakan perlindungan informasi Azure untuk pengguna tertentu dengan menggunakan kebijakan scoped](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="142cd-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="142cd-108">Jika pelabelan otomatis tidak bekerja untuk Outlook saat melampirkan dokumen berlabel, verifikasi bahwa DRMEncryptProperty tidak ditetapkan seperti yang dijelaskan di sini: [IRM pengaturan registri untuk keamanan](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="142cd-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="142cd-109">Jika Anda masih mengalami masalah, silakan mengumpulkan klien perlindungan informasi Azure log dan melampirkan log diekspor ke tiket ini.</span><span class="sxs-lookup"><span data-stu-id="142cd-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="142cd-110">Buka dokumen Office atau buat email baru di Outlook.</span><span class="sxs-lookup"><span data-stu-id="142cd-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="142cd-111">Klik **Lindungi/sensitivitas**  >  **bantuan dan umpan balik**.</span><span class="sxs-lookup"><span data-stu-id="142cd-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="142cd-112">Klik **ekspor log**.</span><span class="sxs-lookup"><span data-stu-id="142cd-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="142cd-113">Simpan log ke pilihan lokasi Anda, dan pasangkan ke permintaan layanan ini.</span><span class="sxs-lookup"><span data-stu-id="142cd-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="142cd-114">Sumber daya tambahan:</span><span class="sxs-lookup"><span data-stu-id="142cd-114">Additional resources:</span></span>

- [<span data-ttu-id="142cd-115">Cara mengkonfigurasi label untuk tanda visual untuk perlindungan informasi Azure</span><span class="sxs-lookup"><span data-stu-id="142cd-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="142cd-116">Tinjau dokumentasi perlindungan informasi Azure</span><span class="sxs-lookup"><span data-stu-id="142cd-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="142cd-117">Menggunakan label sensitivitas di aplikasi Office</span><span class="sxs-lookup"><span data-stu-id="142cd-117">Use sensitivity labels in Office apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

