---
title: Membatalkan reservasi
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
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807570"
---
# <a name="cancelling-reservation"></a>Membatalkan reservasi

- **Layanan mandiri:** Anda dapat membatalkan atau menukarkan instans cadangan sendiri menggunakan [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Pilih reservasi dan klik pengembalian uang atau Exchange. Perhatikan bahwa Anda harus memiliki akses pemilik pada pesanan Pemesanan untuk bertukar atau mengembalikan dana. Akses hanya ke reservasi tidak memperbolehkan Anda melanjutkan dengan pengembalian uang atau Exchange. Tanyakan pemilik pesanan reservasi untuk memberi Anda akses pemilik ke pesanan Pemesanan
- **Kebijakan Exchange:** Anda bisa bertukar reservasi untuk reservasi lainnya dengan tipe yang sama – tidak ada **penalti** pada Exchange reservasi. Komitmen total dengan reservasi baru harus lebih besar dari jumlah jumlah pengembalian dana Pemesanan yang ditukar dan pembayaran bulanan mendatang (jika ada)
- **Kebijakan pengembalian dana:** Jumlah pengembalian dana dan pembayaran yang dibatalkan tidak dapat melebihi $50.000 USD dalam 12 bulan bergulir. **Saat ini kami tidak mengenakan denda** atas pengembalian dana, namun dapat membebankan biaya pada pengembalian dana mendatang  
    **Pengecualian:** Kapabilitas Exchange dan Batalkan layanan mandiri tidak tersedia untuk pelanggan perjanjian perusahaan pemerintah AS
- Dukungan **api/PS/CLI** tidak tersedia untuk pembatalan dan pengembalian dana [layanan mandiri dan pengembalian dana untuk reservasi Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Kapabilitas Exchange dan Batalkan layanan mandiri tidak tersedia untuk pelanggan perjanjian perusahaan pemerintah AS. Tipe langganan pemerintah AS lainnya termasuk Pay-As-You-Go dan CSP didukung

Pelajari selengkapnya: [bagaimana pengembalian dan transaksi Exchange diproses](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Pelajari selengkapnya: [kebijakan Exchange dan pengembalian dana](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Pertanyaan lain: [kunjungi dokumen contoh Reserved](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Bertukar contoh Reserved yang sudah ada (layanan mandiri)**

Anda dapat bertukar reservasi untuk reservasi lainnya dengan tipe yang sama. Anda juga dapat mengembalikan dana reservasi, hingga $50.000 USD per tahun, jika Anda tidak membutuhkannya lagi. Kapabilitas Exchange dan Batalkan layanan mandiri tidak tersedia untuk pelanggan perjanjian perusahaan pemerintah AS. Tipe langganan pemerintah AS lainnya termasuk Pay-As-You-Go dan CSP didukung. Anda harus memiliki akses pemilik pada pesanan Pemesanan untuk menukarkan atau mengembalikan kembali Pemesanan yang sudah ada.

Langkah-langkah berikut ini akan memandu prosedur untuk menyelesaikan transaksi

1. Masuk ke [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)Anda. Pilih reservasi yang ingin Anda kembalikan dan klik **Exchange**
2. Pilih produk VM yang ingin Anda beli dan ketikkan kuantitas. Pastikan bahwa total pembelian baru lebih dari total hasil yang [menentukan ukuran yang tepat sebelum Anda membeli](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Meninjau dan menyelesaikan transaksi

**Pengembalian dana untuk instans cadangan**

Untuk mengembalikan dana reservasi, masuk ke **detail reservasi** dan klik **Refund**

**Nilai pengembalian dana Pro:**

**Contoh Pro-Ration dan persyaratan minimum untuk pengembalian dana dan Exchange**  
Contoh reservasi dimuka:

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

**Dokumen yang direkomendasikan**

- [Bagaimana pengembalian dan transaksi Exchange diproses](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Kebijakan Exchange dan pengembalian dana](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)