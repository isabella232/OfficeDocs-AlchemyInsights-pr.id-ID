---
title: Aturan pengurangan permukaan serangan
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676446"
---
# <a name="attack-surface-reduction-rules"></a>Aturan pengurangan permukaan serangan

Tidak termasuk file atau folder yang dapat mengurangi tingkat proteksi yang diberikan oleh aturan pengurangan serangan permukaan. File yang diblokir oleh aturan diperbolehkan untuk berjalan, dan tidak ada laporan atau kejadian yang direkam. Pengecualian berlaku untuk semua aturan yang mengizinkan pengecualian.

Pengecualian ASR menggunakan sintaks yang sama Antivirus Pertahanan Microsoft pengecualian. Untuk detailnya, [lihat Mengonfigurasi dan memvalidasi pengecualian Antivirus Pertahanan Microsoft dipindai.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus) Untuk menghindari masalah, [tinjau Kesalahan umum untuk dihindari ketika menetapkan pengecualian](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).

Tidak semua aturan ASR mendukung pengecualian. Untuk memvalidasi jika aturan Anda mendukung pengecualian, lihat tabel [Aturan pengurangan permukaan serangan](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

## <a name="attack-surface-reduction-rules"></a>Aturan pengurangan permukaan serangan

Permukaan serangan organisasi Anda mencakup semua tempat di mana penyerang bisa membahayakan perangkat atau jaringan organisasi. Mengurangi tingkat serangan Anda berarti melindungi perangkat dan jaringan organisasi, yang meninggalkan penyerang dengan lebih sedikit cara untuk melakukan serangan. Mengonfigurasi aturan pengurangan permukaan serangan di Pertahanan Microsoft untuk Titik Akhir dapat membantu.

Untuk informasi selengkapnya, lihat:

- [Memetakan GUID aturan ASR ke nama](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- Persyaratan aturan ASR:
    - [Windows 10 Pro, versi 1709 atau lebih baru](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise, versi 1709 atau lebih baru](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server, versi 1803 (Saluran Semi Tahunan) atau yang lebih baru](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Identifikasi pengecualian yang benar untuk diterapkan

1. Cari ID kejadian 1121 atau 1122 dalam log Microsoft-Windows-Pertahanan Windows/Operational.

1. Evaluasi skenario dan konteks blokir dan konfirmasi bahwa skenario ini perlu dibuka blokirnya.

1. Baca nilai Jalur dalam detail kejadian, yang merupakan nilai yang menentukan pengecualian.
    - Buat pengecualian tersebut sedada mungkin.
    - Terapkan wildcard jika diperlukan (misalnya, ganti Variabel pengguna).

1. Terapkan pengecualian sesuai kebutuhan penggunaan Anda. Untuk detailnya, [lihat Mengustomisasi aturan pengurangan serangan permukaan.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)

## <a name="exclusion-is-not-honored"></a>Pengecualian tidak dilakukan

1. Tentukan apakah aturan mendukung pengecualian. Untuk detailnya, [lihat Aturan pengurangan serangan permukaan.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

1. Tinjau pengecualian yang diterapkan dan verifikasi dengan data kejadian kesalahan ketik atau salah interpretasi wildcard. Untuk informasi selengkapnya, lihat [Tipe pengecualian yang didukung](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. jika dampak aturan terlalu tinggi, pertimbangkan untuk memindahkan aturan (kembali) ke mode Audit untuk melakukan validasi lebih lanjut. Untuk detailnya, [lihat Menguji cara fitur Titik Akhir pertahanan Microsoft berfungsi dalam mode audit.](/microsoft-365/security/defender-endpoint/audit-windows-defender)

1. Mengumpulkan data dukungan untuk membuka kasus dukungan dengan menggunakan perintah ini:
    
   ** MDEClientAnalyzer.cmd -v**

    Untuk informasi selengkapnya, [lihat Masalah mesin onboarding ke Pertahanan Microsoft untuk Titik Akhir](issues-with-onboarding-machines.md).
