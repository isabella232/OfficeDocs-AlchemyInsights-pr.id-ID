---
title: Tagihan untuk pembelian Instans Cadangan
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
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820325"
---
# <a name="billing-for-reserved-instance-purchase"></a>Tagihan untuk pembelian Instans Cadangan

Pembelian instans cadangan dikenakan biaya ke metode pembayaran yang terikat dengan langganan yang Anda pilih pada saat pembelian. Tipe langganan harus merupakan perjanjian perusahaan (nomor penawaran: MS-AZR-0017P), Pay-As-You-Go (nomor penawaran: MS-AZR-0003P), Perjanjian Pelanggan Microsoft atau CSP.

- Untuk langganan perusahaan, biaya akan dikurangi dari saldo komitmen keuangan pendaftaran atau dikenakan sebagai overage
- Untuk langganan Pay-As-You-Go, biaya akan ditagih ke metode pembayaran kartu kredit atau faktur pada langganan tersebut

**Membatalkan Reservasi**

- **Layanan mandiri:** Anda dapat membatalkan atau menukar instans khusus Anda sendiri [menggunakan portal Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Pilih reservasi dan klik pengembalian dana atau penukaran. Perhatikan bahwa Anda harus memiliki akses pemilik pada Pesanan Pemesanan untuk melakukan penukaran atau pengembalian dana. Akses hanya ke Reservasi tidak akan mengizinkan Anda melanjutkan pengembalian dana atau penukaran. Mintalah pemilik Pesanan Reservasi untuk memberi Anda akses pemilik ke Pesanan Reservasi
- **Kebijakan Exchange:** Anda dapat menukarkan reservasi untuk pemesanan lain dengan tipe yang sama – tidak **ada perubahan pada** perubahan reservasi. Total komitmen dengan reservasi baru harus lebih besar dari jumlah pengembalian dana reservasi exchange dan pembayaran bulanan di masa mendatang (jika ada)
- **Kebijakan pengembalian dana:** Jumlah pengembalian dana dan pembayaran mendatang yang dibatalkan tidak boleh melebihi $50.000 USD dalam jendela pengembalian 12 bulan. Saat ini **kami tidak sedang melakukan pemesanan untuk pengembalian dana,** tetapi dapat membebankan biaya pada pengembalian dana mendatang

**Pengecualian:** Pertukaran layanan mandiri dan membatalkan kapabilitas tidak tersedia untuk pelanggan Perjanjian Perusahaan Pemerintah AS

- **DUKUNGAN API / PS / CLI** tidak tersedia untuk pembatalan dan pengembalian dana Pertukaran layanan mandiri dan pengembalian [dana untuk Azure Reservations](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Kemampuan pertukaran dan pembatalan layanan mandiri tidak tersedia untuk pelanggan Perjanjian Perusahaan Pemerintah AS. Tipe langganan Pemerintah AS lainnya termasuk Pay-As-You-Go dan CSP didukung

Pelajari selengkapnya : [Bagaimana transaksi pengembalian dan penukaran diproses](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) Pelajari selengkapnya : Kebijakan Exchange dan [Pengembalian](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) DanaTanya jawab lain: Kunjungi dokumen [instans khusus](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Bertukar instans khusus yang sudah ada (Layanan mandiri)**

Anda dapat menukarkan reservasi untuk pemesanan lain dengan tipe yang sama. Anda juga dapat mengembalikan dana reservasi hingga $50.000 USD per tahun, jika tidak lagi memerlukannya. Kemampuan pertukaran dan pembatalan layanan mandiri tidak tersedia untuk pelanggan Perjanjian Perusahaan Pemerintah AS. Tipe langganan Pemerintah AS lainnya termasuk Bayar-Saat-Lalu dan CSP didukung. Anda harus memiliki akses pemilik pada Pesanan Reservasi untuk menukar atau mengembalikan dana reservasi yang sudah ada.

Langkah-langkah berikut akan memandu prosedur untuk menyelesaikan transaksi

1.Masuk ke [portal Azure Anda](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Pilih pemesanan yang ingin Anda kembalikan dan klik **Exchange** 2.Pilih produk VM yang ingin dibeli, lalu ketikkan kuantitas. Pastikan bahwa total pembelian baru lebih dari total pengembalian Tentukan [ukuran yang tepat sebelum Anda membeli.](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3.Meninjau dan menyelesaikan transaksi

**Pengembalian dana untuk instans cadangan**

Untuk mengembalikan dana reservasi, buka Detail **Reservasi, lalu** klik Pengembalian **Dana**

**Pengembalian dana pro-rata:**

**Pro-ration dan contoh persyaratan minimum untuk pengembalian dana dan penukaran** Contoh reservasi di muka:

- Anda membeli RI jangka waktu satu tahun seharga $120 pada 1 Januari
- Pada tanggal 7 April, Anda ingin mengembalikan dana atau menukarkan reservasi ini
- Karena reservasi telah ada selama 97 hari, Anda akan mendapatkan (1-97/365) * $120 kembali. (misalnya $88,1). Saat ini belum ada informasi terkait pengembalian dana
- Jika exchanging, pembelian baru Anda harus lebih besar dari $88,1
- Belum ada keseringaan terkait pengembalian dana saat ini

**Contoh reservasi paket tagihan:**

- Anda membeli RI jangka waktu satu tahun seharga $10 per bulan
- Pada tanggal 7 April, Anda ingin mengembalikan dana atau menukarkan reservasi ini
- Sejak pembayaran terakhir terjadi 7 hari, Anda akan mendapatkan (1-7/31) * $10 kembali. (misalnya $7,74)
- Pembayaran yang akan datang dibatalkan adalah $ 80. Saat ini belum ada informasi terkait pengembalian dana
- Pembatalan ini akan dikurangi $87,74 jika Anda adalah batas pengembalian dana $50.000
- Jika berubah, nilai total pembelian baru akan lebih besar dari $87,74

**Tidak dapat melihat faktur untuk periode tagihan terakhir**

Beberapa kemungkinan alasan Anda tidak melihat faktur:

- Anda memiliki jumlah kredit bulanan dengan langganan yang belum Anda melebihi atau Anda memiliki Uji Coba Gratis. Faktur hanya dibuat jika Anda harus menerima uang
- Kurang dari 30 hari sejak Anda berlangganan Azure
- Faktur belum dibuat. Tunggu hingga akhir periode tagihan
- Jika Anda bukan Administrator Akun, faktur yang lebih lama mungkin tidak tersedia untuk Anda

**Unduh faktur dari portal Azure (.pdf)**

- Pilih langganan Anda [dari halaman Langganan](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) di portal Azure sebagai pengguna dengan akses ke [faktur](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- **Pilih Faktur**
- Klik **Unduh Faktur** untuk menampilkan salinan faktur PDF Anda. Jika **tersedia, lihat** [Mengapa saya tidak melihat faktur untuk periode tagihan terakhir?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

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

Pertanyaan lain: [Kunjungi dokumen instans khusus](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Dokumen yang Disarankan**

- [Dasar-dasar tagihan](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Memahami cara diskon Instans Cadangan diterapkan](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Unduh atau tampilkan faktur tagihan dan data penggunaan harian Azure Anda](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Memahami cara diskon Instans Cadangan diterapkan](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Memahami penggunaan Instans Cadangan untuk langganan Bayar-Saat-Anda-Masuk](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Memahami penggunaan Instans Khusus untuk pendaftaran Enterprise Anda](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Biaya perangkat lunak Windows tidak disertakan dengan instans Khusus](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Instans Khusus dalam program Penyedia Solusi Awan Pusat Mitra (CSP, Central Cloud Solution Provider)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)