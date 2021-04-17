---
title: Melakukan migrasi dari AIP ke MIP/Unified Labeling di Pusat Kepatuhan
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
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825374"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="023da-102">Melakukan migrasi dari AIP ke MIP/Unified Labeling di Pusat Kepatuhan</span><span class="sxs-lookup"><span data-stu-id="023da-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="023da-103">Untuk melakukan migrasi dari label AIP ke Label Terpadu di pusat Keamanan dan Kepatuhan, lakukan hal berikut:</span><span class="sxs-lookup"><span data-stu-id="023da-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="023da-104">**Mengaktifkan proteksi dari portal Azure**</span><span class="sxs-lookup"><span data-stu-id="023da-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="023da-105">Jika Anda belum melakukannya, buka jendela browser baru dan [masuk ke portal Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="023da-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="023da-106">Navigasikan ke **blade Perlindungan Informasi Azure.**</span><span class="sxs-lookup"><span data-stu-id="023da-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="023da-107">Misalnya, pada menu hub, klik Semua **layanan dan** mulai mengetik **Informasi** dalam kotak Filter.</span><span class="sxs-lookup"><span data-stu-id="023da-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="023da-108">Pilih **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="023da-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="023da-109">Jika Anda belum mengakses blade Perlindungan Informasi Azure sebelumnya, [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) lihat langkah tambahan satu kali untuk menambahkan blade ini ke portal.</span><span class="sxs-lookup"><span data-stu-id="023da-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="023da-110">Untuk membuka blade Perlindungan Informasi Azure, Anda harus memiliki paket [Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) atau paket Office 365 yang menyertakan Manajemen Hak.</span><span class="sxs-lookup"><span data-stu-id="023da-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="023da-111">Jika Anda memiliki salah satu langganan ini namun melihat pesan bahwa langganan yang valid tidak dapat ditemukan, hubungi [Dukungan Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) atau gunakan saluran dukungan standar Anda.</span><span class="sxs-lookup"><span data-stu-id="023da-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="023da-112">Temukan **opsi** menu Kelola, dan pilih Aktivasi **proteksi**.</span><span class="sxs-lookup"><span data-stu-id="023da-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="023da-113">Klik **Aktifkan**, lalu konfirmasi tindakan Anda.</span><span class="sxs-lookup"><span data-stu-id="023da-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="023da-114">Ketika aktivasi selesai, bilah informasi **menampilkan Aktivasi selesai dengan sukses**.</span><span class="sxs-lookup"><span data-stu-id="023da-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="023da-115">**Melakukan migrasi label Perlindungan Informasi Azure ke Pusat Keamanan Office 365 & Kepatuhan**</span><span class="sxs-lookup"><span data-stu-id="023da-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="023da-116">Pastikan Anda masuk sebagai pengguna dengan izin Administrator Global.</span><span class="sxs-lookup"><span data-stu-id="023da-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="023da-117">Navigasikan ke **blade Perlindungan Informasi Azure.**</span><span class="sxs-lookup"><span data-stu-id="023da-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="023da-118">Dari **opsi** menu Kelola, pilih **Label terpadu**.</span><span class="sxs-lookup"><span data-stu-id="023da-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="023da-119">Di **blade Perlindungan Informasi Azure - Labeling** terpadu, klik **Aktifkan,** lalu ikuti instruksi online.</span><span class="sxs-lookup"><span data-stu-id="023da-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="023da-120">**Catatan**: Verifikasi bahwa Anda memiliki izin yang tepat sebelum mengaktifkan Migrasi Pusat & Kepatuhan.</span><span class="sxs-lookup"><span data-stu-id="023da-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="023da-121">Lihat artikel berikut ini untuk informasi selengkapnya:</span><span class="sxs-lookup"><span data-stu-id="023da-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="023da-122">Apakah Anda perlu menjadi admin global untuk mengonfigurasi Perlindungan Informasi Azure, atau dapatkah saya mendelegasikan kepada administrator lain?</span><span class="sxs-lookup"><span data-stu-id="023da-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="023da-123">Informasi penting tentang peran administratif setelah melakukan migrasi ke Pusat & Kepatuhan.</span><span class="sxs-lookup"><span data-stu-id="023da-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="023da-124">Untuk informasi selengkapnya tentang migrasi AIP ke Label Terpadu ke Pusat Keamanan dan Kepatuhan, lihat [Memigrasikan label](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="023da-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
