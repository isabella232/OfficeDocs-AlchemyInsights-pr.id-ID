---
title: Membatalkan Pemesanan
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
- "9003552"
- "6817"
ms.openlocfilehash: 8d0a6a37a244e817472c3949109481a30d80328b7353806905e05c547e196ea0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931236"
---
# <a name="cancelling-reservation"></a>Membatalkan Pemesanan

- **Layanan mandiri:** Anda dapat membatalkan atau menukar sendiri instans yang dipesan menggunakan [portal Microsoft Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Pilih pemesanan dan klik pengembalian dana atau penukaran. Perlu diketahui bahwa Anda harus memiliki akses pemilik pada Perintah Pemesanan untuk menukar atau mengajukan pengembalian dana. Anda tidak akan bisa melanjutkan pengajuan pengembalian dana atau penukaran dengan akses hanya ke Pemesanan. Minta pemilik Perintah Pemesanan untuk memberi Anda akses pemilik ke Perintah Pemesanan.
- **Kebijakan penukaran:** Anda dapat menukar pemesanan dengan pemesanan lain dengan tipe yang sama – **tidak ada penalti** pada penukaran pemesanan. Total komitmen pemesanan baru harus lebih besar daripada jumlah pengembalian dana pemesanan yang ditukar dan pembayaran bulanan yang akan datang (jika ada).
- **Kebijakan pengembalian dana:** Jumlah pengembalian dana dan pembayaran mendatang yang dibatalkan tidak boleh melampaui $50.000 USD dalam periode berkelanjutan 12 bulan. Saat ini, kami **tidak mengenakan penalti apa pun** pada pengembalian dana, tetapi mungkin mengenakannya pada pengembalian dana di masa mendatang  
    **Pengecualian:** Kemampuan penukaran dan pembatalan layanan mandiri tidak tersedia untuk pelanggan Perjanjian Enterprise Pemerintah Amerika Serikat
- Dukungan **API / PS / CLI** tidak tersedia untuk pembatalan dan pengembalian dana [Penukaran dan pengembalian dana layanan mandiri untuk Pemesanan Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Kemampuan penukaran dan pembatalan layanan mandiri tidak tersedia untuk pelanggan Perjanjian Enterprise Pemerintah Amerika Serikat. Tipe langganan Pemerintah Amerika Serikat lainnya, termasuk Prabayar dan Penyedia Solusi Cloud, didukung

Pelajari selengkapnya: [Cara transaksi pengembalian dan penukaran diproses](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Pelajari selengkapnya: [Kebijakan Penukaran dan Pengembalian dana](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Pertanyaan lain: [Kunjungi dokumen instans yang dipesan](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Menukar instans dipesan yang sudah ada (Layanan mandiri)**

Anda dapat menukar pemesanan menjadi pemesanan lain dengan tipe yang sama. Anda juga dapat mengajukan pengembalian dana pemesanan, hingga $50.000 USD per tahun, jika tidak memerlukannya lagi. Kemampuan penukaran dan pembatalan layanan mandiri tidak tersedia untuk pelanggan Perjanjian Enterprise Pemerintah Amerika Serikat. Tipe langganan Pemerintah Amerika Serikat lainnya, termasuk Prabayar dan Penyedia Solusi Cloud, didukung. Anda harus memiliki akses pemilik pada Perintah Pemesanan untuk menukar atau mengajukan pengembalian dana pemesanan yang sudah ada.

Langkah-langkah berikut akan memandu prosedur untuk menyelesaikan transaksi

1. Masuk ke [portal Microsoft Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Pilih pemesanan yang ingin dikembalikan dananya, lalu klik **Tukar**
2. Pilih produk VM yang ingin dibeli dan ketik jumlah. Pastikan total pembelian baru lebih besar daripada total pengembalian [Tentukan ukuran yang benar sebelum Anda membeli](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Tinjau dan selesaikan transaksi

**Pengembalian dana untuk instans yang dipesan**

Untuk mendapatkan pengembalian dana pemesanan, masuk ke **Detail Pemesanan**, lalu klik **Pengembalian Dana**

**Pengembalian dana prorata:**

**Contoh persyaratan minimum dan prorata untuk pengembalian dana dan penukaran**  
Contoh pemesanan di muka:

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

**Dokumen yang Disarankan**

- [Cara transaksi pengembalian dan penukaran diproses](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Kebijakan Penukaran dan Pengembalian dana](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)