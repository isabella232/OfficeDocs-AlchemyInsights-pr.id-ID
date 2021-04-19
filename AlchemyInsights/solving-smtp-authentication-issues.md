---
title: Mengatasi masalah autentikasi SMTP
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
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826418"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="c330a-102">Mengatasi masalah autentikasi SMTP</span><span class="sxs-lookup"><span data-stu-id="c330a-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="c330a-103">Jika mendapatkan kesalahan 5.7.57 atau 5.7.3 ketika mencoba mengirim email SMTP dan mengautentikasi dengan klien atau aplikasi, ada beberapa hal yang harus Anda periksa:</span><span class="sxs-lookup"><span data-stu-id="c330a-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="c330a-104">Pengiriman SMTP terautentikasi mungkin dinonaktifkan di penyewa Anda, atau di kotak surat yang coba Anda gunakan (periksa kedua pengaturan).</span><span class="sxs-lookup"><span data-stu-id="c330a-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="c330a-105">Untuk membaca selengkapnya, lihat [Mengaktifkan atau menonaktifkan pengiriman SMTP klien terautentikasi.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)</span><span class="sxs-lookup"><span data-stu-id="c330a-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="c330a-106">Periksa apakah [Default Keamanan Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) diaktifkan untuk penyewa Anda; jika diaktifkan, autentikasi SMTP yang menggunakan autentikasi dasar (juga dikenal sebagai warisan; hal ini akan menggunakan nama pengguna dan kata sandi) akan gagal.</span><span class="sxs-lookup"><span data-stu-id="c330a-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
