---
title: Migrasi dari AIP ke MIP/pelabelan terpadu di pusat kepatuhan
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
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674329"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="07438-102">Migrasi dari AIP ke MIP/pelabelan terpadu di pusat kepatuhan</span><span class="sxs-lookup"><span data-stu-id="07438-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="07438-103">Untuk melakukan migrasi dari label AIP ke pelabelan terpadu di pusat keamanan dan kepatuhan, lakukan hal berikut:</span><span class="sxs-lookup"><span data-stu-id="07438-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="07438-104">**Mengaktifkan proteksi dari portal Azure**</span><span class="sxs-lookup"><span data-stu-id="07438-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="07438-105">Jika Anda belum melakukannya, buka jendela browser baru dan [masuk ke Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="07438-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="07438-106">Navigasikan ke bilah **proteksi informasi Azure** .</span><span class="sxs-lookup"><span data-stu-id="07438-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="07438-107">Misalnya, pada menu hub, klik **semua layanan** dan mulai mengetik **informasi** dalam kotak filter.</span><span class="sxs-lookup"><span data-stu-id="07438-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="07438-108">Pilih **proteksi informasi Azure**.</span><span class="sxs-lookup"><span data-stu-id="07438-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="07438-109">Jika Anda belum mengakses bilah proteksi informasi Azure sebelumnya, lihat [langkah-langkah tambahan](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) satu kali untuk menambahkan bilah ini ke portal.</span><span class="sxs-lookup"><span data-stu-id="07438-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="07438-110">Untuk membuka bilah proteksi informasi Azure, Anda harus memiliki [Paket Premium proteksi informasi Azure](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) atau paket Office 365 yang menyertakan manajemen hak.</span><span class="sxs-lookup"><span data-stu-id="07438-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="07438-111">Jika Anda memiliki salah satu langganan ini tetapi melihat pesan bahwa langganan yang valid tidak dapat ditemukan, [Hubungi dukungan Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) atau gunakan saluran dukungan standar Anda.</span><span class="sxs-lookup"><span data-stu-id="07438-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="07438-112">Temukan opsi **Kelola** menu, dan pilih **aktivasi proteksi**.</span><span class="sxs-lookup"><span data-stu-id="07438-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="07438-113">Klik **Aktifkan**, lalu konfirmasikan tindakan Anda.</span><span class="sxs-lookup"><span data-stu-id="07438-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="07438-114">Ketika aktivasi selesai, bilah informasi menampilkan **aktivasi selesai dengan sukses**.</span><span class="sxs-lookup"><span data-stu-id="07438-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="07438-115">**Migrasi label proteksi informasi Azure ke pusat kepatuhan & keamanan Office 365**</span><span class="sxs-lookup"><span data-stu-id="07438-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="07438-116">Pastikan Anda masuk sebagai pengguna dengan izin administrator global.</span><span class="sxs-lookup"><span data-stu-id="07438-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="07438-117">Navigasikan ke bilah **proteksi informasi Azure** .</span><span class="sxs-lookup"><span data-stu-id="07438-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="07438-118">Dari opsi menu **Kelola** , pilih **label terpadu**.</span><span class="sxs-lookup"><span data-stu-id="07438-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="07438-119">Pada **pelindung informasi Azure-pisau pelabelan terpadu** , klik **Aktifkan** dan ikuti instruksi online.</span><span class="sxs-lookup"><span data-stu-id="07438-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="07438-120">**Catatan**: verifikasi bahwa Anda memiliki izin yang sesuai sebelum mengaktifkan migrasi keamanan & Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="07438-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="07438-121">Lihat artikel berikut ini untuk informasi selengkapnya:</span><span class="sxs-lookup"><span data-stu-id="07438-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="07438-122">Apakah Anda perlu menjadi admin global untuk mengonfigurasi proteksi informasi Azure, atau Bisakah saya mendelegasikan ke administrator lain?</span><span class="sxs-lookup"><span data-stu-id="07438-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="07438-123">Informasi penting tentang peran administratif setelah bermigrasi ke pusat kepatuhan & keamanan.</span><span class="sxs-lookup"><span data-stu-id="07438-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="07438-124">Untuk informasi selengkapnya tentang RAKUTEN Insight untuk Unified pelabelan migrasi ke pusat keamanan dan kepatuhan, lihat [memindahkan label](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="07438-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
