---
title: Memecahkan masalah sertifikat penandatanganan SAML
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
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693424"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="182a9-102">Memecahkan masalah sertifikat penandatanganan SAML</span><span class="sxs-lookup"><span data-stu-id="182a9-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="182a9-103">Untuk mengatasi masalah sertifikat penandatanganan SAML, lakukan langkah-langkah berikut ini:</span><span class="sxs-lookup"><span data-stu-id="182a9-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="182a9-104">Saat Anda menambahkan aplikasi Enterprise yang mendukung SSO, Azure akan menghasilkan sertifikat yang disebut [sertifikat penandatanganan SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span><span class="sxs-lookup"><span data-stu-id="182a9-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="182a9-105">Sertifikat ini memiliki tanggal kedaluwarsa 3 tahun.</span><span class="sxs-lookup"><span data-stu-id="182a9-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="182a9-106">Untuk mengubah tanggal kedaluwarsa sertifikat Anda, lihat [Mengustomisasi tanggal kedaluwarsa sertifikat Federasi Anda dan memindahkannya ke sertifikat baru](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span><span class="sxs-lookup"><span data-stu-id="182a9-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="182a9-107">Azure akan menggunakan sertifikat ini untuk menandatangani token SAML yang diminta oleh aplikasi dan mengirimkannya ke aplikasi untuk SSO yang berhasil.</span><span class="sxs-lookup"><span data-stu-id="182a9-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="182a9-108">Agar ini selesai, Unduh sertifikat dari Azure portal dan kirimkan ke vendor aplikasi untuk menyelesaikan proses SSO.</span><span class="sxs-lookup"><span data-stu-id="182a9-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="182a9-109">Setelah proses ini selesai, aplikasi Anda akan mempercayai sertifikat ini dan semua token SAML yang ditandatangani oleh sertifikat ini akan diterima oleh aplikasi.</span><span class="sxs-lookup"><span data-stu-id="182a9-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="182a9-110">Jika sertifikat ini kedaluwarsa, buat sertifikat baru, perbarui ke vendor aplikasi, lalu lakukan yang aktif di sisi Azure.</span><span class="sxs-lookup"><span data-stu-id="182a9-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="182a9-111">Untuk informasi selengkapnya, lihat [memperpanjang sertifikat yang akan segera kedaluwarsa](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span><span class="sxs-lookup"><span data-stu-id="182a9-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="182a9-112">Jika sertifikat kedaluwarsa, pengguna tidak akan diblokir.</span><span class="sxs-lookup"><span data-stu-id="182a9-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="182a9-113">[Tambahkan alamat email untuk pemberitahuan](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) yang akan diterima sebelum sertifikat saat ini kedaluwarsa.</span><span class="sxs-lookup"><span data-stu-id="182a9-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="182a9-114">Langkah-4 adalah yang opsional.</span><span class="sxs-lookup"><span data-stu-id="182a9-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="182a9-115">Mengubah opsi penandatanganan sertifikat SAML aplikasi dan algoritme penandatanganan sertifikat.</span><span class="sxs-lookup"><span data-stu-id="182a9-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="182a9-116">Untuk informasi selengkapnya, lihat [mengubah opsi penandatanganan sertifikat dan algoritma penandatanganan](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="182a9-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

