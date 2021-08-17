---
title: Tagihan untuk pembelian Instans Khusus
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 00565470de388165e64c45879c22fd5064b4adc695151edaf58878f38a481ff2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104023"
---
# <a name="billing-for-reserved-instance-purchase"></a>Tagihan untuk pembelian Instans Khusus

Pembelian instans khusus dikenakan pada metode pembayaran yang terikat pada langganan yang Anda pilih pada saat pembelian. Tipe langganan harus merupakan perjanjian perusahaan (nomor penawaran: MS-AZR-0017P), Pay-As-You-Go (nomor penawaran: MS-AZR-0003P), Perjanjian Pelanggan Microsoft, atau CSP.

- Untuk langganan perusahaan, biaya dikurangi dari saldo komitmen moneter pendaftaran atau biaya sebagai overage
- Untuk langganan Pay-As-You-Go, biaya akan ditagihkan ke metode pembayaran kartu kredit atau faktur pada langganan

**Membatalkan Pemesanan**

- **Layanan mandiri:** Anda dapat membatalkan atau menukar sendiri instans yang dipesan menggunakan [portal Microsoft Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Pilih pemesanan dan klik pengembalian dana atau penukaran. Perlu diketahui bahwa Anda harus memiliki akses pemilik pada Perintah Pemesanan untuk menukar atau mengajukan pengembalian dana. Anda tidak akan bisa melanjutkan pengajuan pengembalian dana atau penukaran dengan akses hanya ke Pemesanan. Minta pemilik Perintah Pemesanan untuk memberi Anda akses pemilik ke Perintah Pemesanan.
- **Kebijakan penukaran:** Anda dapat menukar pemesanan dengan pemesanan lain dengan tipe yang sama – **tidak ada penalti** pada penukaran pemesanan. Total komitmen pemesanan baru harus lebih besar daripada jumlah pengembalian dana pemesanan yang ditukar dan pembayaran bulanan yang akan datang (jika ada).
- **Kebijakan pengembalian dana:** Jumlah pengembalian dana dan pembayaran mendatang yang dibatalkan tidak boleh melampaui $50.000 USD dalam periode berkelanjutan 12 bulan. Saat ini, kami **tidak mengenakan penalti apa pun** pada pengembalian dana, tetapi mungkin mengenakannya pada pengembalian dana di masa mendatang

**Pengecualian:** Kemampuan penukaran dan pembatalan layanan mandiri tidak tersedia untuk pelanggan Perjanjian Enterprise Pemerintah Amerika Serikat

- Dukungan **API / PS / CLI** tidak tersedia untuk pembatalan dan pengembalian dana [Penukaran dan pengembalian dana layanan mandiri untuk Pemesanan Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Kemampuan penukaran dan pembatalan layanan mandiri tidak tersedia untuk pelanggan Perjanjian Enterprise Pemerintah Amerika Serikat. Tipe langganan Pemerintah Amerika Serikat lainnya, termasuk Prabayar dan Penyedia Solusi Cloud, didukung

Pelajari selengkapnya : Bagaimana transaksi pengembalian dan [penukaran diproses](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) Pelajari selengkapnya : kebijakan [Exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) dan Pengembalian Dana Pertanyaan lain: [Kunjungi dokumen contoh khusus](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Menukar instans dipesan yang sudah ada (Layanan mandiri)**

Anda dapat menukar pemesanan menjadi pemesanan lain dengan tipe yang sama. Anda juga dapat mengajukan pengembalian dana pemesanan, hingga $50.000 USD per tahun, jika tidak memerlukannya lagi. Kemampuan penukaran dan pembatalan layanan mandiri tidak tersedia untuk pelanggan Perjanjian Enterprise Pemerintah Amerika Serikat. Tipe langganan Pemerintah Amerika Serikat lainnya, termasuk Prabayar dan Penyedia Solusi Cloud, didukung. Anda harus memiliki akses pemilik pada Perintah Pemesanan untuk menukar atau mengajukan pengembalian dana pemesanan yang sudah ada.

Langkah-langkah berikut akan memandu prosedur untuk menyelesaikan transaksi

1.Masuk ke [portal Azure Anda](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Pilih pemesanan yang ingin Anda kembalikan dan **klik Exchange** 2.Pilih produk VM yang ingin dibeli, lalu ketikkan kuantitas. Pastikan bahwa total pembelian baru lebih dari total pengembalian Tentukan [ukuran yang tepat sebelum Anda membeli.](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3.Meninjau dan menyelesaikan transaksi

**Pengembalian dana untuk instans yang dipesan**

Untuk mendapatkan pengembalian dana pemesanan, masuk ke **Detail Pemesanan**, lalu klik **Pengembalian Dana**

**Pengembalian dana prorata:**

**Pro-ration dan contoh persyaratan minimum untuk pengembalian dana dan penukaran** Contoh reservasi di muka:

- Anda membeli RI jangka satu tahun seharga $120 pada 1 Januari
- Pada 7 April, Anda ingin mengajukan pengembalian dana atau menukar pemesanan ini
- Karena pemesanan sudah berlangsung 97 hari, Anda akan mendapatkan kembali (1-97/365) * $120. (yaitu $88,1). Saat ini, tidak ada penalti pada pengembalian dana
- Jika menukar, pembelian baru harus lebih besar daripada $88,1
- Saat ini, tidak ada penalti pada pengembalian dana

**Contoh pemesanan paket tagihan:**

- Anda membeli RI jangka satu tahun seharga $10 per bulan
- Pada 7 April, Anda ingin mengajukan pengembalian dana atau menukar pemesanan ini
- Karena pembayaran terakhir terjadi 7 hari, Anda akan mendapatkan kembali (1-7/31) * $10. (yaitu $7,74)
- Pembayaran mendatang yang dibatalkan adalah $ 80. Saat ini, tidak ada penalti pada pengembalian dana
- Pembatalan ini akan mengurangi $87,74 dari batas pengembalian dana Anda sebesar $50.000
- Jika menukar, nilai total pembelian baru harus lebih besar daripada $87,74

**Tidak dapat melihat faktur untuk periode tagihan terakhir**

Beberapa kemungkinan alasan Anda tidak melihat faktur:

- Anda memiliki jumlah kredit bulanan dengan langganan yang belum Anda melebihi atau Anda memiliki Uji Coba Gratis. Faktur hanya dibuat jika Anda harus menerima uang
- Kurang dari 30 hari sejak Anda berlangganan Azure
- Faktur belum dibuat. Tunggu hingga akhir periode tagihan
- Jika Anda bukan Administrator Akun, faktur yang lebih lama mungkin tidak tersedia untuk Anda

**Unduh faktur Anda dari portal Azure (.pdf)**

- Pilih langganan Anda [dari halaman Langganan](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) di portal Azure sebagai pengguna dengan akses ke [faktur](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- **Pilih Faktur**
- Klik **Unduh Faktur** untuk menampilkan salinan faktur PDF Anda. Jika tertulis **Tidak tersedia**, lihat [Mengapa saya tidak melihat faktur untuk periode penagihan terakhir?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).

**Menerima faktur Anda dalam email (.pdf)**

- Pilih langganan Anda [dari halaman](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Langganan. Klik **Faktur lalu** Emailkan faktur saya
- Klik **setujui** dan terima persyaratannya. Anda harus memilih setiap langganan yang Anda miliki

Catatan: Jika Anda tidak mendapatkan email setelah mengikuti langkah-langkah tersebut, pastikan alamat email Anda sudah benar dalam [preferensi komunikasi di profil Anda](https://account.windowsazure.com/profile)

**Unduh data penggunaan Anda dari portal Azure**

- Masuk ke [Pusat Akun Azure](https://account.windowsazure.com/Subscriptions) sebagai Admin [Akun](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Pilih langganan yang ingin Anda gunakan faktur dan informasi penggunaan
- Pilih **Riwayat Tagihan**
- Pilih **Tampilkan Pernyataan** Saat Ini untuk melihat perkiraan biaya Anda saat perkiraan dihasilkan
- Pilih **Unduh Penggunaan** untuk mengunduh data penggunaan harian sebagai file CSV. Jika Anda melihat dua versi tersedia, unduh versi 2

Pertanyaan lain: [Kunjungi dokumen instans yang dipesan](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Dokumen yang Disarankan**

- [Dasar-dasar tagihan](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Memahami cara diskon Instans Cadangan diterapkan](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Unduh atau tampilkan faktur tagihan dan data penggunaan harian Azure Anda](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Memahami cara diskon Instans Cadangan diterapkan](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Memahami penggunaan Instans Cadangan untuk langganan Bayar-Saat-Anda-Masuk](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Memahami penggunaan Instans Khusus untuk pendaftaran Enterprise Anda](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows lunak khusus yang tidak disertakan dengan instans Khusus](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Instans Cadangan dalam program Pusat Penyedia Solusi Cloud Mitra (CSP, Reserved Instances in Partner Central Penyedia Solusi Cloud)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)