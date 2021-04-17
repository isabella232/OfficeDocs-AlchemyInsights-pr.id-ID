---
title: Jenis langganan yang didukung
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
- "6675"
ms.openlocfilehash: dcf5855bff8725ea746196c1f07d689ce1797f8c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820685"
---
# <a name="supported-subscription-types"></a>Jenis langganan yang didukung

Tinjau jenis langganan yang didukung untuk melanjutkan.

[Jenis langganan yang didukung](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Transfer kepemilikan tagihan**

Portal Microsoft Azure sebagai [Admin Akun](https://ms.portal.azure.com/) dari akun tagihan yang memiliki langganan yang ingin Anda transfer.

- Cari di **Manajemen Biaya + Tagihan**. Pilih **Langganan** dari panel kiri. Bergantung pada akses, Anda mungkin perlu memilih cakupan tagihan dan kemudian **Langganan** atau **Langganan Azure**.
- Pilih Transfer kepemilikan tagihan untuk langganan yang ingin Anda transfer
- Masukkan alamat email pengguna yang merupakan administrator penagihan akun yang akan menjadi pemilik baru untuk langganan, lalu pilih **kirim permintaan transfer**
- Pengguna mendapatkan email dengan instruksi untuk meninjau permintaan transfer Anda. Untuk menyetujui permintaan transfer, pengguna memilih tautan dalam email dan mengikuti instruksinya.

Catatan: Jika Anda mentransfer kepemilikan tagihan langganan ke akun pengguna di penyewa Azure Active Directory lain, semua penetapan [kontrol akses berbasis peran (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) untuk mengelola sumber daya di langganan tersebut akan dihapus secara permanen. Hanya pemilik baru yang akan memiliki akses untuk mengelola sumber daya di langganan. Untuk informasi selengkapnya, lihat [Mentransfer langganan ke pengguna di penyewa Azure Active Directory lain](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Mentransfer Kepemilikan Langganan**

Prasyarat Transfer Kepemilikan Langganan akses berbasis peran (RBAC) untuk mengelola sumber daya dalam langganan kehilangan aksesnya. Untuk informasi selengkapnya tentang menambahkan langganan yang ada ke penyewa, lihat [Mengaitkan atau menambahkan langganan Azure ke Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Transfer Langganan dengan jumlah terutang yang sudah ada dari siklus penagihan saat ini tidak akan ditransfer ke instrumen pembayaran baru di akun baru. Satu-satunya informasi yang tersedia untuk pengguna di akun baru adalah biaya bulan lalu untuk langganan Anda. Penggunaan dan riwayat penagihan lainnya tidak ditransfer dengan langganan.
- Transfer kepemilikan tagihan langganan Perjanjian Enterprise (EA) saat ini hanya didukung di Portal Perjanjian Enterprise
- Mentransfer langganan berorientasi kredit seperti Visual Studio, BizSpark, Jaringan Mitra Microsoft ke pengguna baru harus memiliki lisensi Visual Studio/Jaringan mitra Microsoft untuk menerima permintaan transfer.
- Semua sumber daya seperti Komputer Virtual, disk, dan situs web berhasil ditransfer ke akun baru. Sumber daya berikut dapat terpengaruh dalam transfer langganan lintas penyewa:

**Azure AD Domain Services**

Azure Key Vault

- [Pengguna dan database terkait SQL](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) dapat terpengaruh, terutama jika pelanggan menggunakan autentikasi terkait Azure Active Directory
- **Layanan Aplikasi** yang dikonfigurasi dengan autentikasi Azure Active Directory dapat terpengaruh
- Akun **Visual Studio Team** Services yang tersambung ke langganan Azure dapat kehilangan akses untuk sementara jika langganan Azure yang terhubung dibatalkan

**Dokumen yang Disarankan**

Langkah-langkah setelah menerima kepemilikan tagihan:

- Untuk mempertahankan kepemilikan tagihan, tetapi mengubah jenis langganan Anda, lihat: [Mengalihkan langganan Azure ke penawaran lain](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Mentransfer langganan Visual Studio, Jaringan Mitra Microsoft (MPN), dan Dev/Test Prabayar](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Mentransfer kepemilikan tagihan langganan Perjanjian Enterprise (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [FAQ Transfer Kepemilikan](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Pemecahan masalah Transfer kepemilikan](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)