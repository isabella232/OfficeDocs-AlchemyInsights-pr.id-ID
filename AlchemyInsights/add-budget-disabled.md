---
title: Mengapa tombol Tambahkan anggaran dinonaktifkan untuk saya?
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
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807411"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Mengapa tombol Tambahkan anggaran dinonaktifkan untuk saya?

Untuk membuat anggaran, Anda memerlukan salah satu izin berikut ini:

- Grup manajemen, langganan, lingkup grup sumber daya
- Kontributor manajemen biaya
- Owner
- Penyebab
- Pelanggan perusahaan saja: pendaftaran, Departemen, lingkup akun
- Admin pendaftaran (Atur anggaran di lingkup pendaftaran)
- Admin Departemen (Atur anggaran pada lingkup departemen)
- Pemilik akun (Atur anggaran di lingkup akun)
- Perjanjian pelanggan modern saja: akun tagihan, profil tagihan, lingkup bagian faktur
- Pembuat langganan Azure

**Saya membuat anggaran bila biaya untuk bulan ini sudah lebih murah. Mengapa saya tidak menerima pemberitahuan?**  
Jika Anda telah melampaui ambang batas biaya yang diberikan saat Anda membuat anggaran yang tidak akan digunakan untuk peringatan. Setelah siklus baru dimulai, jika Anda melanggar batas, maka pemberitahuan akan diaktifkan.

**Kapan saya harus menerima pemberitahuan setelah saya melebihi satu dari ambang pemberitahuan anggaran yang ditentukan?**  
Anggaran dievaluasi setiap 4 jam. Memerlukan minimal 8 jam untuk data penggunaan untuk mencapai sistem anggaran. Dengan ini, pemberitahuan mungkin memerlukan waktu hingga 12 jam setelah Anda melebihi batas.

**Mengapa tombol tanggal mulai dinonaktifkan saat saya memilih periode reset bulan atau tagihan bulan?**  
Anggaran diratakan pada bulan kalender saat ini atau periode penagihan saat ini (jika bulan tagihan dipilih). Oleh karena itu, kami telah mengisi nilai ini untuk Anda.

**Mengapa saya tidak melihat grafik biaya saya dalam pengalaman pembuatan anggaran?**  
Kami membutuhkan minimal 2 bulan biaya data sebelum kami bisa membuat grafik untuk membantu Anda dengan pembuatan anggaran.

**Mengapa saya tidak dapat menetapkan anggaran terhadap langganan yang baru saja saya buat?**  
Setelah pembuatan langganan, data memerlukan waktu 24-48 jam untuk memproses sebelum menetapkan anggaran terhadapnya.

**Sumber daya API anggaran**

- [Budget api v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): menyediakan operasi untuk membuat dan memperbarui anggaran. Menggunakan API anggaran, Anda bisa mengatur ambang batas anggaran dan mengonfigurasi beberapa pemberitahuan agar diaktifkan saat Anda mendekati ambang batas tersebut. Pemberitahuan bisa memicu email atau grup tindakan Azure untuk melakukan otomatisasi. Catatan: pemfilteran untuk API ini tidak selaras dengan pemfilteran/dimensi API kueri.
- [Budget api v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): membuat anggaran dengan kemampuan pemfilteran biaya yang lebih besar dari v1. Pemfilteran menyelaraskan ke kontrak yang digunakan dalam kueri dan api dimensi kami. Ini adalah API anggaran yang dianjurkan untuk digunakan maju.
- [Dimensi](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): menyediakan operasi untuk mendapatkan dimensi yang didukung untuk penggunaan Anda di bawah berbagai lingkup. Menggunakan API dimensi, Anda bisa mengambil daftar dimensi yang bisa digunakan sebagai input untuk menghasilkan kueri dengan API kueri.
- [Kueri](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): menyediakan operasi untuk mendapatkan data biaya dan penggunaan agregat berdasarkan kueri yang Anda sediakan. Menggunakan API kueri, Anda bisa menentukan pemfilteran yang diinginkan, mengurutkan dan mengelompokkan pada semua dimensi yang tersedia (yang diakses dari API dimensi).

**Perkiraan biaya**

**Mengapa saya tidak melihat perkiraan untuk biaya saya dalam analisis biaya?**  
Ada beberapa alasan mengapa proyeksi perkiraan mungkin hilang bagi Anda dalam analisis biaya, beberapa di antaranya adalah sebagai berikut:

1. Jika data biaya Anda kurang dari 10 hari, bagan perkiraan tidak akan dimuat. Model memerlukan setidaknya 10 hari dari data biaya terbaru untuk proyeksi yang akurat
2. Jika Anda telah memilih tanggal bersejarah, bagan perkiraan tidak akan terlihat. Pilih rentang tanggal dengan tanggal mendatang untuk bagan perkiraan yang akan ditampilkan
3. Jika akun Anda memiliki beberapa mata uang, bagan perkiraan hanya akan biaya proyek untuk ' semua biaya dalam USD '

**Mengapa perkiraan tidak berubah ketika saya membuat perubahan pada sumber daya saya?**  
Model perkiraan memerlukan beberapa hari untuk memperhitungkan perubahan dalam akun dan tidak membuat proyeksi langsung berdasarkan perubahan dalam sumber daya  
Untuk langkah yang lebih besar dari peningkatan atau penurunan sumber daya, model akan memakan waktu yang sedikit lebih lama untuk menyesuaikan dengan perubahan ini untuk memperhitungkan anomali

**Mengapa perkiraan saya meningkat setelah saya melakukan pembelian reservasi atau Marketplace?**  
Model perkiraan mempertimbangkan ' biaya aktual ' dan tidak memperhitungkan penggunaan dan pembelian secara terpisah. Untuk pembelian satu kali, model akan mengurangi proyeksi setelah 10 hari untuk memperhitungkan kenaikan mendadak dalam biaya

**Saya ingin melihat perkiraan untuk satu dimensi (misalnya. Ketinggian**  
Perkiraan saat ini mendukung Total proyeksi biaya dan bukan untuk masing-masing meter. Oleh karena itu, ketika ' dikelompokkan menurut ' sebuah dimensi, proyeksi akan untuk total semua item dalam dimensi

**Dokumen yang direkomendasikan**

- [Apa itu manajemen biaya Azure?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Praktik terbaik manajemen biaya Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Menganalisis biaya dan pengeluaran Anda](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Menjelajahi dan menganalisis biaya dengan analisis biaya](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Manajemen biaya Azure: Pricing](https://azure.microsoft.com/services/cost-management/#pricing)
- [Meninjau biaya dalam analisis biaya](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Tutorial video: membuat anggaran di portal Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Prasyarat untuk menampilkan dan mengkustomisasi anggaran](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Membuat dan mengelola anggaran](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Mengonfigurasi otomatisasi dengan grup tindakan Azure dan API anggaran](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Menggunakan pemberitahuan biaya untuk memantau penggunaan dan pengeluaran](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Praktik terbaik manajemen biaya](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Video tutorial**

- [Membuat anggaran di portal Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Mengelola biaya dengan API dan grup tindakan anggaran](https://go.microsoft.com/fwlink/?linkid=2147038)