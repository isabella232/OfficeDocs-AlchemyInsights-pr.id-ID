---
title: Tagihan untuk pembelian Instans reserved
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823078"
---
# <a name="billing-for-reserved-instance-purchase"></a>Tagihan untuk pembelian Instans reserved

Pembelian instans cadangan dibebankan ke metode pembayaran yang terkait dengan langganan yang Anda pilih pada waktu pembelian. Tipe langganan harus merupakan perjanjian perusahaan (nomor Penawaran: MS-AZR-0017P), Pay-As-You-Go (nomor Penawaran: MS-AZR-0003P), perjanjian pelanggan Microsoft atau CSP.

- Untuk langganan Enterprise, biaya dipotong dari saldo komitmen moneter pendaftaran atau dibebankan sebagai melebihi batas
- Untuk langganan prabayar, biaya akan ditagihkan ke metode pembayaran kartu kredit atau faktur pada langganan

**Membatalkan reservasi**

- **Layanan mandiri:** Anda dapat membatalkan atau menukarkan instans cadangan sendiri menggunakan [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Pilih reservasi dan klik pengembalian uang atau Exchange. Perhatikan bahwa Anda harus memiliki akses pemilik pada pesanan Pemesanan untuk bertukar atau mengembalikan dana. Akses hanya ke reservasi tidak memperbolehkan Anda melanjutkan dengan pengembalian uang atau Exchange. Tanyakan pemilik pesanan reservasi untuk memberi Anda akses pemilik ke pesanan Pemesanan
- **Kebijakan Exchange:** Anda bisa bertukar reservasi untuk reservasi lainnya dengan tipe yang sama – tidak ada **penalti** pada Exchange reservasi. Komitmen total dengan reservasi baru harus lebih besar dari jumlah jumlah pengembalian dana Pemesanan yang ditukar dan pembayaran bulanan mendatang (jika ada)
- **Kebijakan pengembalian dana:** Jumlah pengembalian dana dan pembayaran yang dibatalkan tidak dapat melebihi $50.000 USD dalam 12 bulan bergulir. **Saat ini kami tidak mengenakan denda** atas pengembalian dana, namun dapat membebankan biaya pada pengembalian dana mendatang

**Pengecualian:** Kapabilitas Exchange dan Batalkan layanan mandiri tidak tersedia untuk pelanggan perjanjian perusahaan pemerintah AS

- Dukungan **api/PS/CLI** tidak tersedia untuk pembatalan dan pengembalian dana [layanan mandiri dan pengembalian dana untuk reservasi Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Kapabilitas Exchange dan Batalkan layanan mandiri tidak tersedia untuk pelanggan perjanjian perusahaan pemerintah AS. Tipe langganan pemerintah AS lainnya termasuk Pay-As-You-Go dan CSP didukung

Pelajari selengkapnya: [bagaimana pengembalian dan transaksi Exchange diproses](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) Pelajari selengkapnya: [kebijakan Exchange dan pengembalian dana](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) pertanyaan lain: [kunjungi dokumen contoh Reserved](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Bertukar contoh Reserved yang sudah ada (layanan mandiri)**

Anda dapat bertukar reservasi untuk reservasi lainnya dengan tipe yang sama. Anda juga dapat mengembalikan dana reservasi, hingga $50.000 USD per tahun, jika Anda tidak membutuhkannya lagi. Kapabilitas Exchange dan Batalkan layanan mandiri tidak tersedia untuk pelanggan perjanjian perusahaan pemerintah AS. Tipe langganan pemerintah AS lainnya termasuk Pay-As-You-Go dan CSP didukung. Anda harus memiliki akses pemilik pada pesanan Pemesanan untuk menukarkan atau mengembalikan kembali Pemesanan yang sudah ada.

Langkah-langkah berikut ini akan memandu prosedur untuk menyelesaikan transaksi

1. masuk ke [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)Anda. Pilih reservasi yang ingin Anda kembalikan danklik **Exchange** 2. Pilih produk VM yang ingin Anda beli dan ketikkan kuantitas. Pastikan bahwa total pembelian baru lebih dari total hasil yang [menentukan ukuran yang tepat sebelum Anda membeli](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3. tinjau dan selesaikan transaksi

**Pengembalian dana untuk instans cadangan**

Untuk mengembalikan dana reservasi, masuk ke **detail reservasi** dan klik **Refund**

**Nilai pengembalian dana Pro:**

**Contoh Pro-Ration dan persyaratan minimum untuk pengembalian dana dan Exchange** Contoh reservasi dimuka:

- Anda membeli istilah RI untuk $120 pada tanggal 1 Januari
- Pada tanggal 7 April Anda ingin mengembalikan atau menukarkan reservasi ini
- Karena reservasi telah aktif untuk 97 hari, Anda akan mendapatkan (1-97/365) * $120 kembali. (yaitu $88,1). Saat ini tidak ada denda untuk pengembalian dana
- Jika bertukar, pembelian baru Anda harus lebih besar dari $88,1
- Tidak ada penalti pada pengembalian dana saat ini

**Contoh reservasi paket tagihan:**

- Anda membeli istilah satu tahun RI untuk $10 per bulan
- Pada tanggal 7 April Anda ingin mengembalikan atau menukarkan reservasi ini
- Sejak pembayaran terakhir terjadi 7 hari, Anda akan mendapatkan (1-7/31) * $10. (yaitu $7,74)
- Pembayaran yang akan dibatalkan adalah $80. Saat ini tidak ada denda untuk pengembalian dana
- Pembatalan ini akan mengurangi $87,74 dari Anda batas pengembalian dana $50.000
- Jika bertukar, nilai total pembelian baru harus lebih besar dari $87,74

**Tidak dapat melihat faktur untuk periode tagihan terakhir**

Beberapa kemungkinan alasan Anda tidak melihat faktur:

- Anda memiliki jumlah kredit bulanan dengan langganan yang tidak melebihi atau Anda memiliki uji coba gratis. Faktur hanya dihasilkan jika Anda berutang uang
- Tidak lebih dari 30 hari dari hari langganan Anda ke Azure
- Faktur belum dibuat. Tunggu hingga akhir periode penagihan
- Jika Anda bukan administrator akun, faktur yang lebih lama mungkin tidak tersedia untuk Anda

**Mengunduh faktur Anda dari Azure portal (. pdf)**

- Pilih langganan Anda dari halaman [langganan](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) di Azure Portal sebagai [pengguna dengan akses ke faktur](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Pilih **faktur**
- Klik **Unduh faktur** untuk menampilkan salinan faktur PDF Anda. Jika dikatakan **tidak tersedia** , lihat [mengapa saya tidak melihat faktur untuk periode tagihan terakhir?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Menerima faktur Anda dalam email (. pdf)**

- Pilih langganan Anda dari halaman [langganan](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) . Klik **faktur** lalu kirim faktur saya
- Klik **pilih** dan terima ketentuan. Anda harus memilih untuk setiap metode berlangganan yang Anda miliki

Catatan: jika Anda tidak mendapatkan email setelah mengikuti langkah-langkah tersebut, pastikan alamat email Anda sudah benar di [preferensi komunikasi pada profil Anda](https://account.windowsazure.com/profile)

**Mengunduh data penggunaan Anda dari portal Azure**

- Masuk ke [pusat akun Azure](https://account.windowsazure.com/Subscriptions) sebagai [admin akun](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Pilih langganan yang Anda inginkan dan informasi penggunaan faktur
- Memilih **Riwayat tagihan**
- Pilih **Tampilkan pernyataan saat ini** untuk melihat perkiraan biaya Anda pada saat perkiraan tersebut dihasilkan
- Pilih **penggunaan unduhan** untuk mengunduh data penggunaan harian sebagai file CSV. Jika Anda melihat dua versi yang tersedia, Unduh versi 2

Pertanyaan lain: [kunjungi dokumen contoh Reserved](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Dokumen yang direkomendasikan**

- [Dasar-dasar tagihan](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Memahami cara diskon contoh Reserved diterapkan](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Mengunduh atau menampilkan faktur penagihan Azure dan data penggunaan harian Anda](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Memahami cara diskon contoh Reserved diterapkan](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Memahami penggunaan Instans Reserved untuk langganan bayar sesuai pemakaian Anda](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Memahami penggunaan Instans Reserved untuk pendaftaran perusahaan Anda](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Biaya perangkat lunak Windows tidak disertakan dengan instans cadangan](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Contoh Reserved dalam program mitra Cloud Central Solution Provider (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)