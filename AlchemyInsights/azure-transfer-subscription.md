---
title: Mentransfer kepemilikan tagihan Azure
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
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922078"
---
# <a name="transfer-azure-billing-ownership"></a>Mentransfer kepemilikan tagihan Azure

Masuk ke [Azure portal](https://portal.azure.com/) sebagai administrator akun tagihan yang memiliki langganan yang ingin Anda transfer. Jika tidak yakin apakah Anda dan administrator, atau jika Anda perlu menentukan siapa, lihat [menentukan administrator tagihan akun](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

- Cari **biaya manajemen + tagihan**.
- Pilih **langganan** dari panel kiri. Bergantung pada akses, Anda mungkin perlu memilih lingkup tagihan lalu **langganan** atau **langganan Azure**.
- Pilih **transfer kepemilikan tagihan** untuk langganan yang ingin Anda transfer
- Masukkan alamat email pengguna yang merupakan administrator tagihan akun yang akan menjadi pemilik baru untuk langganan lalu pilih **Kirim permintaan transfer**
- Pengguna mendapatkan email dengan instruksi untuk meninjau permintaan transfer Anda. Untuk menyetujui permintaan transfer, pengguna akan memilih link dalam email dan mengikuti instruksi.

**Catatan** : jika Anda mentransfer kepemilikan tagihan langganan Anda ke akun pengguna di penyewa Azure AD lainnya, semua penetapan [Access Control (RBAC) berbasis peran](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)untuk mengelola sumber daya dalam langganan dihapus secara permanen. Hanya pemilik baru yang akan memiliki akses untuk mengelola sumber daya dalam metode berlangganan. Untuk informasi selengkapnya, lihat [mentransfer langganan ke pengguna di penyewa AZURE AD lainnya](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Dokumen yang direkomendasikan**

- [Mentransfer kepemilikan tagihan Azure langganan ke akun lain](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Tentang mentransfer kepemilikan tagihan untuk langganan Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Mentransfer Visual Studio, Jaringan mitra Microsoft (MPN) dan membayar saat Anda menggunakan langganan dev/uji](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Tanya Jawab Umum kepemilikan transfer](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Memecahkan masalah pengalihan kepemilikan](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
