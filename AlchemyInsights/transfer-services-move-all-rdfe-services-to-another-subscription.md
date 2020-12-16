---
title: Layanan transfer-memindahkan semua layanan RDFE ke langganan lain
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692046"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="65028-102">Layanan transfer-memindahkan semua layanan RDFE ke langganan lain</span><span class="sxs-lookup"><span data-stu-id="65028-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="65028-103">**Memindahkan sumber daya**</span><span class="sxs-lookup"><span data-stu-id="65028-103">**Move resources**</span></span>

<span data-ttu-id="65028-104">Sumber daya Azure dapat dipindahkan ke langganan atau sumber daya lain Azure di bawah langganan yang sama menggunakan Azure portal, Azure PowerShell, Azure CLI, atau REST API untuk memindahkan sumber daya.</span><span class="sxs-lookup"><span data-stu-id="65028-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="65028-105">Sebelum Anda bisa memindahkan sumber daya, lihat:</span><span class="sxs-lookup"><span data-stu-id="65028-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="65028-106">Checklist sebelum memindahkan sumber daya</span><span class="sxs-lookup"><span data-stu-id="65028-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="65028-107">Layanan yang bisa dipindahkan</span><span class="sxs-lookup"><span data-stu-id="65028-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="65028-108">Cara memvalidasi perpindahan</span><span class="sxs-lookup"><span data-stu-id="65028-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="65028-109">Memindahkan panduan untuk Layanan</span><span class="sxs-lookup"><span data-stu-id="65028-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="65028-110">Untuk memindahkan sumber daya yang sudah ada ke grup atau langganan sumber daya lain, Anda bisa menggunakan:</span><span class="sxs-lookup"><span data-stu-id="65028-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="65028-111">Portal Azure</span><span class="sxs-lookup"><span data-stu-id="65028-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="65028-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="65028-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="65028-113">CLI Azure</span><span class="sxs-lookup"><span data-stu-id="65028-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="65028-114">API REST</span><span class="sxs-lookup"><span data-stu-id="65028-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="65028-115">Tutorial: [memindahkan sumber daya Azure ke grup atau langganan sumber daya lain](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="65028-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="65028-116">**Memecahkan masalah kesalahan dengan manajer sumber daya Azure**</span><span class="sxs-lookup"><span data-stu-id="65028-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="65028-117">Lihat artikel di bawah ini untuk mempelajari tentang beberapa kesalahan penyebaran Azure Umum dan menerima informasi untuk mengatasinya.</span><span class="sxs-lookup"><span data-stu-id="65028-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="65028-118">Jika tidak dapat menemukan kode kesalahan untuk penyebaran kesalahan, lihat [menemukan kode kesalahan](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="65028-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="65028-119">Memecahkan masalah kesalahan penyebaran</span><span class="sxs-lookup"><span data-stu-id="65028-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="65028-120">Memecahkan masalah pemindahan sumber daya Azure ke grup sumber daya atau langganan baru</span><span class="sxs-lookup"><span data-stu-id="65028-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="65028-121">Perhatikan bahwa jika Anda ingin memutakhirkan langganan Azure, seperti beralih dari gratis ke prabayar, Anda perlu mengonversi langganan Anda.</span><span class="sxs-lookup"><span data-stu-id="65028-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="65028-122">Untuk memutakhirkan uji coba gratis, lihat [memutakhirkan uji coba gratis atau langganan Microsoft Imagine Azure untuk membayar sesuai](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)permintaan.</span><span class="sxs-lookup"><span data-stu-id="65028-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="65028-123">Untuk mengubah akun prabayar, lihat [mengubah langganan Azure Pay-As-You-Go ke Penawaran yang berbeda](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="65028-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="65028-124">**Untuk menambahkan atau mengaitkan langganan Azure ke penyewa direktori aktif Azure Anda:**</span><span class="sxs-lookup"><span data-stu-id="65028-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="65028-125">Masuk dan pilih langganan yang ingin Anda gunakan dari [halaman langganan di Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="65028-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="65028-126">Pilih **Ubah direktori**.</span><span class="sxs-lookup"><span data-stu-id="65028-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="65028-127">Tinjau peringatan apa pun yang muncul, lalu pilih **Ubah**.</span><span class="sxs-lookup"><span data-stu-id="65028-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="65028-128">Direktori diubah untuk langganan dan Anda akan mendapatkan pesan yang berhasil.</span><span class="sxs-lookup"><span data-stu-id="65028-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="65028-129">Gunakan pengalih *direktori* untuk masuk ke direktori baru Anda.</span><span class="sxs-lookup"><span data-stu-id="65028-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="65028-130">Mungkin butuh waktu hingga 10 menit agar semuanya muncul dengan benar.</span><span class="sxs-lookup"><span data-stu-id="65028-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="65028-131">**Dokumen yang direkomendasikan**</span><span class="sxs-lookup"><span data-stu-id="65028-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="65028-132">Mentransfer kepemilikan langganan Azure</span><span class="sxs-lookup"><span data-stu-id="65028-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="65028-133">Memindahkan sumber daya ke grup sumber daya atau langganan baru</span><span class="sxs-lookup"><span data-stu-id="65028-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="65028-134">Mengelola sumber daya menggunakan Azure portal</span><span class="sxs-lookup"><span data-stu-id="65028-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
