---
title: Mengapa tombol Tambahkan anggaran dinonaktifkan untuk saya?
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
- "9003547"
- "6464"
ms.openlocfilehash: 1263662184948ed1e77e3abacd17babf4aa033ed1ecec29b4c4afc26d6da56f0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "53954674"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Mengapa tombol Tambahkan anggaran dinonaktifkan untuk saya?

Untuk membuat anggaran, Anda memerlukan salah satu izin berikut ini:

- Grup Manajemen, Langganan, Lingkup Grup Sumber Daya
- Kontributor Manajemen Biaya
- Pemilik
- Kontributor
- Enterprise Customer Only: Enrollment, Department, Account Scopes
- Admin Pendaftaran (atur anggaran pada Lingkup pendaftaran)
- Admin Departemen (atur anggaran dalam lingkup Departemen)
- Pemilik Akun (atur anggaran pada Lingkup akun)
- Hanya Perjanjian Pelanggan Modern: Akun Tagihan, Profil Tagihan, Lingkup Bagian Faktur
- Pembuat langganan Azure

**Saya membuat anggaran saat biaya untuk bulan ini sudah lewat anggaran. Mengapa saya tidak menerima pemberitahuan?**  
Jika Anda telah melampaui ambang biaya tertentu saat membuat anggaran pemberitahuan itu tidak akan fire. Begitu siklus baru dimulai, jika Anda melanggar ambang batas itu pemberitahuan akan terlihat.

**Kapan saya harus menerima pemberitahuan setelah melampaui salah satu ambang batas pemberitahuan anggaran yang ditentukan?**  
Anggaran dievaluasi setiap 4 jam. Diperlukan setidaknya 8 jam hingga data penggunaan mencapai sistem anggaran. Dengan mengingat hal ini, peringatan akan memakan waktu hingga 12 jam agar tidak terjadi pemadaman setelah melampaui ambang batas.

**Mengapa tombol Tanggal mulai dinonaktifkan saat saya memilih periode reset bulan atau Tagihan?**  
Anggaran diratakan dengan bulan kalender atau periode tagihan saat ini (dalam hal Bulan Tagihan dipilih). Oleh karena itu, kami telah mengisi nilai ini untuk Anda.

**Mengapa saya tidak melihat grafik biaya dalam pengalaman pembuatan anggaran?**  
Kami memerlukan minimal 2 bulan data biaya sebelum menyajikan grafik untuk membantu Anda membuat anggaran.

**Mengapa saya tidak dapat menetapkan anggaran terhadap langganan yang baru saya buat?**  
Setelah pembuatan langganan, data akan memerlukan waktu 24-48 jam untuk diproses sebelum mengatur anggaran terhadap langganan.

**Sumber Daya API Anggaran**

- [Anggaran API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): Menyediakan operasi untuk membuat dan memperbarui anggaran. Dengan MENGGUNAKAN API Anggaran, Anda bisa mengatur ambang anggaran dan mengonfigurasi beberapa pemberitahuan agar fire saat Anda mendekati ambang batas itu. Peringatan dapat memicu email atau Grup Tindakan Azure untuk melakukan otomatisasi. Catatan: Pemfilteran untuk API ini tidak selaras dengan Pemfilteran / dimensi API Kueri.
- [Anggaran API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): Membuat anggaran dengan kapabilitas pemfilteran biaya yang lebih besar daripada v1. Pemfilteran meratakan dengan kontrak yang digunakan di API Kueri dan Dimensi kami. Ini adalah API anggaran yang direkomendasikan untuk digunakan ke depannya.
- [Dimensi](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): Menyediakan operasi untuk mendapatkan dimensi yang didukung untuk penggunaan Anda di bawah berbagai lingkup. Menggunakan API Dimensi, Anda dapat mengambil daftar dimensi yang dapat digunakan sebagai input untuk menghasilkan kueri dengan API Kueri.
- [Kueri](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): Menyediakan operasi untuk mendapatkan agregat biaya dan penggunaan data berdasarkan kueri yang Anda berikan. Dengan MENGGUNAKAN API Kueri, Anda bisa menentukan pemfilteran, pengurutan dan mengelompokkan semua dimensi yang tersedia (yang diakses dari API Dimensi).

**Biaya yang Diperkirakan**

**Kenapa saya tidak melihat perkiraan untuk biaya saya dalam Analisis Biaya?**  
Ada beberapa alasan mengapa proyeksi perkiraan mungkin hilang bagi Anda dalam Analisis Biaya, beberapa di antaranya adalah sebagai berikut:

1. Jika data biaya Anda lebih kecil dari 10 hari, bagan perkiraan tidak akan dimuat. Model memerlukan setidaknya 10 hari dari data biaya terbaru untuk proyeksi akurat
2. Jika Anda telah memilih tanggal bersejarah, bagan perkiraan tidak akan terlihat. Silakan pilih rentang tanggal dengan tanggal di masa mendatang agar bagan perkiraan ditampilkan
3. Jika akun Anda memiliki beberapa mata uang, bagan perkiraan hanya akan memperkirakan biaya untuk 'Semua biaya dalam USD'

**Mengapa perubahan perkiraan tidak berubah saat saya membuat perubahan ke sumber daya saya?**  
Model perkiraan memerlukan beberapa hari untuk mempertimbangkan perubahan dalam akun dan tidak membuat proyeksi langsung berdasarkan perubahan dalam sumber daya  
Untuk langkah yang lebih besar dalam meningkatkan atau mengurangi sumber daya, model akan memakan waktu sedikit lebih lama untuk menyesuaikan perubahan ini agar sesuai dengan kebutuhan

**Mengapa peningkatan perkiraan setelah saya melakukan pemesanan atau pembelian Marketplace?**  
Model perkiraan mempertimbangkan 'Biaya Aktual' Anda dan tidak bertanggung jawab atas penggunaan dan pembelian secara terpisah. Untuk pembelian satu kali, model akan mengurangi proyeksi setelah 10 hari untuk memperhitungkan peningkatan biaya secara tiba-tiba

**Saya ingin melihat perkiraan untuk dimensi tunggal (misalnya. Meter)**  
Perkiraan saat ini mendukung proyeksi biaya total dan bukan untuk meter individual. Karenanya, saat 'Dikelompokkan menurut' dimensi, proyeksi akan menjadi total dari semua item dalam dimensi tersebut

**Dokumen yang Disarankan**

- [Apa itu Manajemen Biaya Azure?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Praktik terbaik Azure Cost Management](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Menganalisis biaya dan pengeluaran Anda](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Menjelajahi dan menganalisis biaya dengan analisis Biaya](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Manajemen Biaya Azure: Harga](https://azure.microsoft.com/services/cost-management/#pricing)
- [Meninjau biaya dalam analisis biaya](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Tutorial video: Membuat anggaran di portal Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Prasyarat untuk menampilkan dan mengkustomisasi anggaran](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Membuat dan mengelola anggaran](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Mengonfigurasi otomatisasi dengan API Grup Tindakan dan Anggaran Azure](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Menggunakan pemberitahuan biaya untuk memantau penggunaan dan pengeluaran](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Praktik terbaik Manajemen Biaya](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Video tutorial**

- [Membuat anggaran di portal Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Mengelola biaya dengan API Anggaran dan Grup Tindakan](https://go.microsoft.com/fwlink/?linkid=2147038)