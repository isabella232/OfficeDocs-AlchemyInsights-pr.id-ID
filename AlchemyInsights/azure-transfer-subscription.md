---
title: Mentransfer kepemilikan tagihan Azure
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
- "9003560"
- "6849"
ms.openlocfilehash: 803d0105ad2bbaf2b18cea6aa556b6af5e09cb2d41812d4747aa703e6e7d7780
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036099"
---
# <a name="transfer-azure-billing-ownership"></a>Mentransfer kepemilikan tagihan Azure

Masuk ke [portal Azure](https://portal.azure.com/) sebagai administrator akun tagihan yang memiliki langganan yang ingin Anda transfer. Jika Anda tidak yakin apakah Anda merupakan administrator, atau jika Anda perlu menentukan siapa, lihat [Menentukan administrator tagihan akun](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Cari _Manajemen Biaya + Tagihan_.
1. Pilih **Langganan** dari panel kiri. Bergantung pada akses, Anda mungkin perlu memilih cakupan tagihan kemudian **Langganan** atau **langganan Azure**.
1. Pilih **Transfer kepemilikan tagihan** untuk langganan yang ingin Anda transfer.
1. Masukkan alamat email pengguna yang merupakan administrator tagihan akun yang akan menjadi pemilik baru untuk langganan kemudian pilih **kirim permintaan transfer**.
1. Pengguna mendapatkan email dengan instruksi untuk meninjau permintaan transfer Anda. Untuk menyetujui permintaan transfer, pengguna memilih tautan dalam email dan mengikuti instruksinya.

Perhatikan bahwa jika Anda mentransfer kepemilikan tagihan langganan ke akun pengguna di penyewa Azure AD lain, semua penetapan [kontrol akses berbasis peran (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) untuk mengelola sumber daya di langganan akan dihapus secara permanen. Hanya pemilik baru yang akan memiliki akses untuk mengelola sumber daya di langganan. Untuk informasi selengkapnya tentang cara mengubah direktori untuk langganan, lihat [Mentransfer langganan ke pengguna di penyewa Azure AD lain](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Dampak penting pada faktur**_: jika Anda telah mentransfer kepemilikan tagihan untuk langganan Azure, biaya Anda akan dikenakan secara prorata. Anda akan dapat mengakses faktur sesuai hal berikut:  

1. Pilih langganan Anda dari  [halaman Langganan](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) di portal Azure sebagai [pengguna yang memiliki akses ke faktur](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support), lalu pilih **Faktur**.
1. Klik **Unduh Faktur** untuk menampilkan salinan faktur PDF Anda. Jika tertulis _Tidak tersedia_, lihat [Mengapa saya tidak melihat faktur untuk periode tagihan terakhir?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).
1. Anda juga dapat menampilkan penggunaan sehari-hari dengan mengklik **periode tagihan** untuk mendapatkan PDF faktur dan salinan file penggunaan harian mendetail (.CSV). Untuk informasi selengkapnya, lihat [Mendapatkan faktur dan data penggunaan](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Dokumen yang Disarankan**

- [Mentransfer kepemilikan langganan Azure untuk ke lain](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Tentang mentransfer kepemilikan tagihan untuk langganan Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Mentransfer langganan Visual Studio, Microsoft Partner Network (MPN), dan pengembangan/uji Prabayar](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [FAQ Transfer Kepemilikan](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Pemecahan masalah Transfer kepemilikan](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
