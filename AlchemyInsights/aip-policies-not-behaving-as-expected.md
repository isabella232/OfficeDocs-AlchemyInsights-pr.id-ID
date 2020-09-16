---
title: 'AIP: kebijakan tidak berperilaku seperti yang diharapkan'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663192"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="01279-102">AIP: kebijakan tidak berperilaku seperti yang diharapkan</span><span class="sxs-lookup"><span data-stu-id="01279-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="01279-103">Perlindungan informasi Azure: kebijakan tidak berperilaku seperti yang diharapkan, lihat berikut ini untuk panduan yang direkomendasikan untuk berbagai masalah kebijakan:</span><span class="sxs-lookup"><span data-stu-id="01279-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="01279-104">Jika Anda mengalami masalah dengan tanda visual, silakan Tinjau [Kapan tanda visual diterapkan](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="01279-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="01279-105">Jika Anda mengalami masalah dengan pelabelan otomatis, silakan Tinjau [cara mengonfigurasi ketentuan untuk klasifikasi otomatis dan yang direkomendasikan untuk proteksi informasi Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) dan [apa yang dicari tipe informasi sensitif](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="01279-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="01279-106">Jika Anda mengalami masalah dengan proteksi Native/Pfile, silakan Tinjau [konfigurasi file api](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="01279-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="01279-107">Periksa apakah Anda menggunakan kebijakan lingkup yang tidak dikonfigurasi dengan benar: [cara mengonfigurasi kebijakan perlindungan informasi Azure untuk pengguna tertentu dengan menggunakan kebijakan lingkup](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="01279-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="01279-108">Jika label otomatis tidak berfungsi untuk Outlook saat melampirkan dokumen berlabel, pastikan bahwa DRMEncryptProperty tidak ditentukan seperti yang diuraikan di sini: [pengaturan registri IRM untuk keamanan](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="01279-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="01279-109">Jika Anda masih mengalami masalah, silakan kumpulkan log klien proteksi informasi Azure dan lampirkan log yang diekspor ke tiket ini.</span><span class="sxs-lookup"><span data-stu-id="01279-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="01279-110">Buka dokumen Office atau buat email baru di Outlook.</span><span class="sxs-lookup"><span data-stu-id="01279-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="01279-111">Klik **proteksi/kepekaan**  >  **bantuan dan umpan balik**.</span><span class="sxs-lookup"><span data-stu-id="01279-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="01279-112">Klik **ekspor log**.</span><span class="sxs-lookup"><span data-stu-id="01279-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="01279-113">Simpan log ke pilihan lokasi Anda, lalu Lampirkan ke permintaan layanan ini.</span><span class="sxs-lookup"><span data-stu-id="01279-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="01279-114">Sumber daya tambahan:</span><span class="sxs-lookup"><span data-stu-id="01279-114">Additional resources:</span></span>

- [<span data-ttu-id="01279-115">Cara mengonfigurasikan label untuk tanda visual untuk proteksi informasi Azure</span><span class="sxs-lookup"><span data-stu-id="01279-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="01279-116">Meninjau dokumentasi perlindungan informasi Azure</span><span class="sxs-lookup"><span data-stu-id="01279-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="01279-117">Menggunakan label sensitivitas dalam aplikasi Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="01279-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

