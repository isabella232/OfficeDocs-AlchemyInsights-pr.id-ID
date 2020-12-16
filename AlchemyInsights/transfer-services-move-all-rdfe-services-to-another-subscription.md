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
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Layanan transfer-memindahkan semua layanan RDFE ke langganan lain

**Memindahkan sumber daya**

Sumber daya Azure dapat dipindahkan ke langganan atau sumber daya lain Azure di bawah langganan yang sama menggunakan Azure portal, Azure PowerShell, Azure CLI, atau REST API untuk memindahkan sumber daya.

Sebelum Anda bisa memindahkan sumber daya, lihat:

- [Checklist sebelum memindahkan sumber daya](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Layanan yang bisa dipindahkan](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Cara memvalidasi perpindahan](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Memindahkan panduan untuk Layanan](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Untuk memindahkan sumber daya yang sudah ada ke grup atau langganan sumber daya lain, Anda bisa menggunakan:

- [Portal Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [CLI Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [API REST](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Tutorial: [memindahkan sumber daya Azure ke grup atau langganan sumber daya lain](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Memecahkan masalah kesalahan dengan manajer sumber daya Azure**

Lihat artikel di bawah ini untuk mempelajari tentang beberapa kesalahan penyebaran Azure Umum dan menerima informasi untuk mengatasinya. Jika tidak dapat menemukan kode kesalahan untuk penyebaran kesalahan, lihat [menemukan kode kesalahan](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Memecahkan masalah kesalahan penyebaran](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Memecahkan masalah pemindahan sumber daya Azure ke grup sumber daya atau langganan baru](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Perhatikan bahwa jika Anda ingin memutakhirkan langganan Azure, seperti beralih dari gratis ke prabayar, Anda perlu mengonversi langganan Anda.

- Untuk memutakhirkan uji coba gratis, lihat [memutakhirkan uji coba gratis atau langganan Microsoft Imagine Azure untuk membayar sesuai](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)permintaan.
- Untuk mengubah akun prabayar, lihat [mengubah langganan Azure Pay-As-You-Go ke Penawaran yang berbeda](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Untuk menambahkan atau mengaitkan langganan Azure ke penyewa direktori aktif Azure Anda:**

1. Masuk dan pilih langganan yang ingin Anda gunakan dari [halaman langganan di Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Pilih **Ubah direktori**.
3. Tinjau peringatan apa pun yang muncul, lalu pilih **Ubah**.
4. Direktori diubah untuk langganan dan Anda akan mendapatkan pesan yang berhasil.
5. Gunakan pengalih *direktori* untuk masuk ke direktori baru Anda. Mungkin butuh waktu hingga 10 menit agar semuanya muncul dengan benar.

**Dokumen yang direkomendasikan**

- [Mentransfer kepemilikan langganan Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Memindahkan sumber daya ke grup sumber daya atau langganan baru](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Mengelola sumber daya menggunakan Azure portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
