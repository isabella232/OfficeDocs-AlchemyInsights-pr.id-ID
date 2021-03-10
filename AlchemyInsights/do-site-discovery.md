---
title: Melakukan pencarian situs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693485"
---
# <a name="do-site-discovery"></a>Melakukan pencarian situs

Jika organisasi masih menggunakan aplikasi dan paket web warisan untuk menggunakan mode Internet Explorer (yang dilakukan oleh sebagian besar pelanggan), maka Anda harus melakukan beberapa penemuan situs tambahan.

**Anda telah menerapkan versi Microsoft Edge yang lebih lama**

Jika Anda sudah mengonfigurasi daftar situs perusahaan Anda untuk bekerja untuk versi warisan Microsoft Edge, maka penemuan situs Anda hampir selesai. Satu hal yang mungkin perlu Anda lakukan adalah menambahkan situs netral.

Situs netral biasanya adalah situs yang menyediakan masuk tunggal (SSO). Jika Anda masuk ke situs netral dari Microsoft Edge, maka Anda ingin tetap menggunakan Microsoft Edge untuk mengautentikasi. Jika Anda masuk ke situs netral dalam mode Internet Explorer, maka Anda ingin tetap menggunakan mode Internet Explorer untuk mengautentikasi.

Identifikasi SSO atau situs netral lainnya yang Anda gunakan dan tambahkan ke daftar situs perusahaan Anda.

**Internet Explorer adalah browser default Anda**

Jika Anda hanya menggunakan Internet Explorer sekarang, Anda mungkin tidak mengetahui situs mana yang telah dimutakhirkan ke standar web modern dan yang masih memerlukan Internet Explorer. Anda akan ingin menemukan dan menambahkan situs ini ke daftar situs perusahaan sehingga Anda bisa menggunakan mode Internet Explorer hanya untuk situs tersebut.

> [!NOTE]
> [Penemuan situs perusahaan](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) menemukan situs yang mungkin memerlukan mode Internet Explorer. Hal ini dapat mengumpulkan data pada komputer yang menjalankan Windows Internet Explorer 8 melalui Internet Explorer 11 di Windows 10, Windows 8,1, atau Windows 7.

**Menganalisis data**

Setelah Anda mengumpulkan data situs, kami merekomendasikan proses empat langkah berikut ini untuk menganalisis data:
1. Urutkan data menurut domain, lalu menurut URL.
2. Tentukan batas aplikasi untuk mengonfigurasi mode Internet Explorer. Anda ingin menyertakan semua situs dan kontrol web yang menentukan aplikasi tersebut, tetapi Anda tidak ingin menyertakan situs dan kontrol tambahan. Beberapa situs mungkin sesederhana *https://contoso.com/app1* sementara yang lain mungkin mengharuskan Anda untuk menentukan beberapa situs dan halaman.
3. Uji aplikasi untuk memverifikasi bahwa aplikasi tidak berfungsi secara native. Banyak situs akan menawarkan konten modern saat mereka mendeteksi browser modern dan hanya menawarkan konten warisan saat mereka mendeteksi Internet Explorer.
4. Tambahkan aplikasi ke daftar situs perusahaan Anda jika pengujian gagal.

> [!NOTE]
> Sebagai praktik terbaik, Kelompokkan semua situs yang terdiri dari aplikasi. Dengan cara ini, saat Anda memutakhirkan aplikasi, lebih mudah untuk menghapus seluruh situs dari mode Internet Explorer dan mulai menggunakan browser modern untuk aplikasi tersebut.

Setelah Anda selesai dengan penemuan situs dan Anda telah menganalisis data, Anda siap untuk mulai melihat strategi saluran Anda.

