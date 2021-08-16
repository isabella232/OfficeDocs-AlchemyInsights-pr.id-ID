---
title: Melakukan penemuan situs
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
ms.openlocfilehash: 4653fdef7e9226f05809d56e9a445cd1da35b0578c088bea72252a281d4527d2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030761"
---
# <a name="do-site-discovery"></a>Melakukan penemuan situs

Jika organisasi Anda masih menggunakan aplikasi web warisan dan rencana untuk menggunakan mode Internet Explorer (yang sebagian besar pelanggan lakukan), Anda harus melakukan beberapa penemuan situs tambahan.

**Anda telah menggunakan versi uji coba yang lebih Microsoft Edge**

Jika Anda telah mengonfigurasi Daftar Situs Perusahaan Anda agar bekerja untuk versi warisan Microsoft Edge, maka penemuan situs Anda hampir selesai. Satu hal yang mungkin perlu Anda lakukan adalah menambahkan situs netral.

Situs netral biasanya situs yang menyediakan akses masuk tunggal (SSO). Jika masuk ke situs netral dari Microsoft Edge, Anda ingin tetap berada di situs Microsoft Edge mengautentikasi. Jika masuk ke situs netral dalam mode Internet Explorer, Anda perlu tetap menggunakan mode Internet Explorer untuk mengautentikasi.

Identifikasi setiap SSO atau situs netral lainnya yang Anda gunakan dan tambahkan ke Daftar Situs Perusahaan Anda.

**Internet Explorer adalah browser default Anda**

Jika Anda hanya menggunakan Internet Explorer sekarang, Anda mungkin tidak tahu situs mana yang telah dimutakhirkan ke standar web modern dan yang masih memerlukan Internet Explorer. Anda pasti ingin menemukan dan menambahkan situs ini ke Daftar Situs Perusahaan sehingga Anda bisa menggunakan mode Internet Explorer hanya untuk situs tersebut.

> [!NOTE]
> [Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) menemukan situs yang mungkin memerlukan mode Internet Explorer. Alat tersebut dapat mengumpulkan data di komputer yang menjalankan Windows Internet Explorer 8 melalui Internet Explorer 11 di Windows 10, Windows 8.1, Windows 7.

**Menganalisis data**

Setelah Anda mengumpulkan data situs, kami menyarankan proses empat langkah berikut ini untuk menganalisis data:
1. Urutkan data menurut domain, lalu menurut URL.
2. Menetapkan batas sebuah aplikasi untuk dikonfigurasikan untuk mode Internet Explorer. Anda ingin menyertakan semua situs dan kontrol web yang menentukan aplikasi, tapi Anda tidak ingin menyertakan situs dan kontrol tambahan. Beberapa situs mungkin sesederhana *https://contoso.com/app1* yang lain mungkin mengharuskan Anda menentukan beberapa situs dan halaman.
3. Uji aplikasi untuk memverifikasi bahwa aplikasi itu tidak berfungsi aslinya. Banyak situs akan menawarkan konten modern ketika mendeteksi browser modern dan hanya menawarkan konten warisan saat mendeteksi Internet Explorer.
4. Tambahkan aplikasi ke Daftar Situs Perusahaan Anda jika pengujian gagal.

> [!NOTE]
> Sebagai praktik terbaik, kelompokkan semua situs yang terdiri dari aplikasi. Dengan cara ini, saat Anda memutakhirkan aplikasi, akan lebih mudah untuk menghapus seluruh situs dari mode Internet Explorer dan mulai menggunakan browser modern untuk aplikasi tersebut.

Setelah selesai dengan penemuan situs dan telah menganalisis data, Anda siap untuk mulai melihat strategi saluran Anda.

