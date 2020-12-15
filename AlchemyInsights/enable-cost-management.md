---
title: Aktifkan manajemen biaya
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677738"
---
# <a name="enable-cost-management"></a><span data-ttu-id="751d4-102">Aktifkan manajemen biaya</span><span class="sxs-lookup"><span data-stu-id="751d4-102">Enable cost management</span></span>

<span data-ttu-id="751d4-103">**Apa artinya ' biaya dinonaktifkan untuk organisasi Anda '?**</span><span class="sxs-lookup"><span data-stu-id="751d4-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="751d4-104">Organisasi yang menggunakan perjanjian Enterprise (EA) atau akun Microsoft Customer Agreement (MCA) dapat menonaktifkan akses ke informasi biaya dan informasi harga.</span><span class="sxs-lookup"><span data-stu-id="751d4-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="751d4-105">Setelah masuk ke Azure portal, mereka bisa menggunakan api penagihan untuk secara sistematis mendapatkan faktur (sekali disertakan dalam) dan detail penggunaan.</span><span class="sxs-lookup"><span data-stu-id="751d4-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="751d4-106">**Cara memperbolehkan pengguna tambahan untuk mengakses faktur**</span><span class="sxs-lookup"><span data-stu-id="751d4-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="751d4-107">Masuk ke **bilah langganan** di Azure portal.</span><span class="sxs-lookup"><span data-stu-id="751d4-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="751d4-108">Pilih **faktur** lalu **akses ke faktur**.</span><span class="sxs-lookup"><span data-stu-id="751d4-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="751d4-109">Aktifkan akses, diikuti dengan menyimpan perubahan, untuk memperbolehkan pengguna di peran cakupan langganan untuk mengunduh faktur.</span><span class="sxs-lookup"><span data-stu-id="751d4-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="751d4-110">Administrator akun juga dapat mengonfigurasi untuk mengirim faktur melalui email.</span><span class="sxs-lookup"><span data-stu-id="751d4-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="751d4-111">Untuk mempelajari selengkapnya, lihat [mendapatkan faktur Anda dalam email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="751d4-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="751d4-112">**Cara menambahkan pengguna ke peran pembaca tagihan**</span><span class="sxs-lookup"><span data-stu-id="751d4-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="751d4-113">Masuk ke **bilah langganan** di Azure portal.</span><span class="sxs-lookup"><span data-stu-id="751d4-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="751d4-114">Pilih **kontrol akses (iam)** lalu klik **Tambahkan**.</span><span class="sxs-lookup"><span data-stu-id="751d4-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="751d4-115">Pilih **pembaca tagihan** di halaman **Pilih peran** .</span><span class="sxs-lookup"><span data-stu-id="751d4-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="751d4-116">Ketikkan email pengguna yang ingin Anda undang, lalu klik **OK** untuk mengirim undangan.</span><span class="sxs-lookup"><span data-stu-id="751d4-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="751d4-117">Ikuti instruksi yang disediakan di email undangan untuk masuk sebagai pembaca tagihan.</span><span class="sxs-lookup"><span data-stu-id="751d4-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="751d4-118">Untuk informasi selengkapnya, lihat [memberikan akses ke tagihan](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="751d4-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="751d4-119">**Dokumen yang direkomendasikan**</span><span class="sxs-lookup"><span data-stu-id="751d4-119">**Recommended documents**</span></span>

- [<span data-ttu-id="751d4-120">Mengaktifkan DA dan AO tampilan melalui portal EA</span><span class="sxs-lookup"><span data-stu-id="751d4-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="751d4-121">Biaya yang disertakan dalam manajemen biaya</span><span class="sxs-lookup"><span data-stu-id="751d4-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="751d4-122">Penawaran yang didukung Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="751d4-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="751d4-123">Meninjau biaya dalam analisis biaya</span><span class="sxs-lookup"><span data-stu-id="751d4-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="751d4-124">Menyediakan akses ke informasi tagihan</span><span class="sxs-lookup"><span data-stu-id="751d4-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="751d4-125">Memeriksa akses ke perjanjian pelanggan Microsoft</span><span class="sxs-lookup"><span data-stu-id="751d4-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






