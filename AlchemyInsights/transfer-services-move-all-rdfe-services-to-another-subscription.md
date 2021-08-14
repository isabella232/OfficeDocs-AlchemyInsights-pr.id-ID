---
title: Layanan Transfer - Memindahkan semua layanan RDFE ke langganan lain
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
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940062"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Layanan Transfer - Memindahkan semua layanan RDFE ke langganan lain

**Pindahkan sumber daya**

Sumber daya Azure dapat dipindahkan ke langganan Azure atau grup sumber daya lain dalam langganan yang sama menggunakan portal Azure, Azure PowerShell, Azure CLI, atau API REST untuk memindahkan sumber daya.

Sebelum Anda bisa memindahkan sumber daya, lihat:

- [Daftar Periksa sebelum memindahkan sumber daya](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Layanan yang bisa dipindahkan](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Cara memvalidasi pemindahan](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Panduan pemindahan untuk layanan](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Untuk memindahkan sumber daya yang sudah ada ke grup atau langganan sumber daya lain, Anda dapat menggunakan:

- [Portal Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Tutorial: [Memindahkan sumber daya Azure ke grup atau langganan sumber daya lain](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Memecahkan masalah kesalahan dengan Azure Resource Manager**

Lihat artikel di bawah ini untuk mempelajari tentang beberapa kesalahan umum penyebaran Azure dan menerima informasi untuk mengatasinya. Jika tidak dapat menemukan kode kesalahan untuk kesalahan penyebaran, lihat [Menemukan kode kesalahan.](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)

- [Memecahkan masalah kesalahan penggunaan](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Memecahkan masalah pemindahan sumber daya Azure ke grup atau langganan sumber daya baru](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Perlu diperhatikan bahwa jika ingin memutakhirkan langganan Azure, seperti beralih dari gratis ke layanan berbayar saat Anda bepergian, Anda perlu mengonversi langganan.

- Untuk memutakhirkan uji coba gratis, lihat Mutakhirkan Uji Coba Gratis atau langganan [Microsoft Imagine Azure ke Bayar-Saat-Anda-Masuk.](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)
- Untuk mengubah akun berbayar saat Anda menggunakan, lihat Mengubah langganan [Azure Pay-As-You-Go ke penawaran lain.](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)

**Untuk menambahkan atau mengaitkan langganan Azure ke penyewa Azure Active Directory Anda:**

1. Masuk dan pilih langganan yang ingin Anda gunakan dari [halaman Langganan di portal Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Pilih **Ubah direktori.**
3. Tinjau peringatan yang muncul, lalu pilih **Ubah**.
4. Direktori diubah untuk langganan dan Anda akan mendapatkan pesan berhasil.
5. Gunakan *pengalih* Direktori untuk masuk ke direktori baru Anda. Mungkin membutuhkan waktu hingga 10 menit agar semuanya muncul dengan benar.

**Dokumen yang Disarankan**

- [Mentransfer kepemilikan langganan Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Memindahkan sumber daya ke grup atau langganan sumber daya baru](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Mengelola sumber daya menggunakan portal Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
