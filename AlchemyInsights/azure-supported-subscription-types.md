---
title: Tipe langganan yang didukung
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
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807565"
---
# <a name="supported-subscription-types"></a>Tipe langganan yang didukung

Tinjau tipe langganan yang didukung untuk melanjutkan lebih lanjut.

[Tipe langganan yang didukung](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Mentransfer kepemilikan tagihan**

Azure Portal sebagai [admin akun](https://ms.portal.azure.com/) tagihan yang memiliki langganan yang ingin Anda transfer

- Cari **biaya manajemen + tagihan** . Pilih **langganan** dari panel kiri. Bergantung pada akses, Anda mungkin perlu memilih lingkup tagihan lalu **langganan** atau **langganan Azure** .
- Pilih transfer kepemilikan tagihan untuk langganan yang ingin Anda transfer
- Masukkan alamat email pengguna yang merupakan administrator tagihan akun yang akan menjadi pemilik baru untuk langganan lalu pilih **Kirim permintaan transfer**
- Pengguna mendapatkan email dengan instruksi untuk meninjau permintaan transfer Anda. Untuk menyetujui permintaan transfer, pengguna akan memilih link dalam email dan mengikuti instruksi.

Catatan: jika Anda mentransfer kepemilikan tagihan langganan Anda ke akun pengguna di penyewa Azure AD lainnya, semua penetapan [Access Control (RBAC) berbasis peran](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) untuk mengelola sumber daya dalam langganan dihapus secara permanen. Hanya pemilik baru yang akan memiliki akses untuk mengelola sumber daya dalam metode berlangganan. Untuk informasi selengkapnya, lihat [mentransfer langganan ke pengguna di penyewa AZURE AD lainnya](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Transfer kepemilikan langganan**

Pengalihan kepemilikan langganan (RBAC) persyaratan akses ke mengelola sumber daya di langganan akan hilang. Untuk informasi selengkapnya tentang menambahkan langganan yang sudah ada ke penyewa, lihat [mengaitkan atau menambahkan langganan Azure ke Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Transfer langganan dengan jumlah yang sudah ada yang sudah ada dari siklus penagihan saat ini tidak akan ditransfer ke instrumen pembayaran baru dalam akun baru. Satu-satunya informasi yang tersedia untuk pengguna di akun baru adalah biaya bulan lalu untuk langganan Anda. Sisa Riwayat penggunaan dan tagihan tidak ditransfer dengan metode berlangganan.
- Transfer kepemilikan tagihan dari langganan Enterprise Agreement (EA) saat ini hanya didukung di portal perjanjian Enterprise saja
- Mentransfer langganan berorientasi kredit seperti Visual Studio, BizSpark, Jaringan mitra Microsoft ke pengguna baru memerlukan lisensi jaringan mitra Visual Studio/Microsoft untuk menerima permintaan transfer
- Semua sumber daya seperti mesin virtual, disk, dan transfer situs web ke akun baru berhasil. Sumber daya berikut ini dapat terpengaruh dalam transfer langganan antarpenyewa:

**Layanan domain Azure AD**

Kubah kunci Azure

- [Pengguna dan database terkait SQL](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) bisa terpengaruh, terutama jika pelanggan menggunakan autentikasi terkait Azure Active Directory
- **Layanan aplikasi** yang dikonfigurasikan dengan autentikasi Azure Active Directory dapat terpengaruh
- **Tim Visual Studio** Akun layanan yang tersambung ke langganan Azure mungkin akan kehilangan akses sementara saat langganan Azure yang tersambung dibatalkan

**Dokumen yang direkomendasikan**

Langkah setelah menerima kepemilikan tagihan:

- Untuk mempertahankan kepemilikan tagihan, namun mengubah tipe langganan Anda, lihat: [mengalihkan langganan Azure Anda ke Penawaran lain](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Mentransfer Visual Studio, Jaringan mitra Microsoft (MPN) dan membayar saat Anda menggunakan langganan dev/uji](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Mentransfer kepemilikan tagihan dari langganan Enterprise Agreement (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Tanya Jawab Umum kepemilikan transfer](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Memecahkan masalah pengalihan kepemilikan](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)