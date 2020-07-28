---
title: Apple MDM push Certificate belum diatur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439381"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="d0371-102">Apple MDM push Certificate belum diatur</span><span class="sxs-lookup"><span data-stu-id="d0371-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="d0371-103">Apple MDM push Certificate (juga dikenal sebagai sertifikat Layanan pemberitahuan push Apple (APNS)) belum dikonfigurasi untuk langganan Anda.</span><span class="sxs-lookup"><span data-stu-id="d0371-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="d0371-104">Tanpa sertifikat push MDM Apple yang dikonfigurasi, Anda tidak dapat mendaftarkan dan mengelola perangkat iOS dan Mac OS.</span><span class="sxs-lookup"><span data-stu-id="d0371-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="d0371-105">Setelah Anda menambahkan sertifikat untuk Intune, pengguna dapat menginstal aplikasi portal perusahaan untuk mendaftarkan perangkat iOS.</span><span class="sxs-lookup"><span data-stu-id="d0371-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="d0371-106">Pilih **"Saya setuju."**</span><span class="sxs-lookup"><span data-stu-id="d0371-106">Select **"I agree."**</span></span> <span data-ttu-id="d0371-107">untuk memberikan izin kepada Microsoft untuk mengirim data ke Apple.</span><span class="sxs-lookup"><span data-stu-id="d0371-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="d0371-108">Pilih **Download CSR Anda** Intune penandatanganan sertifikat permintaan yang diperlukan untuk membuat Apple Mdm push Certificate.</span><span class="sxs-lookup"><span data-stu-id="d0371-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="d0371-109">File tersebut digunakan untuk meminta sertifikat hubungan kepercayaan dari portal sertifikat push Apple.</span><span class="sxs-lookup"><span data-stu-id="d0371-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="d0371-110">Pilih **buat Mdm push Certificate Anda** untuk membuka Apple push Certificates portal.</span><span class="sxs-lookup"><span data-stu-id="d0371-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="d0371-111">Masuk dengan ID Apple perusahaan Anda, lalu pilih **buat sertifikat**.</span><span class="sxs-lookup"><span data-stu-id="d0371-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="d0371-112">Pilih **Pilih file**, Jelajahi file permintaan penandatanganan sertifikat, lalu pilih **Unggah**.</span><span class="sxs-lookup"><span data-stu-id="d0371-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="d0371-113">Pada halaman konfirmasi, pilih **Download** untuk mendownload file Certificate (. pem), dan simpan file secara lokal.</span><span class="sxs-lookup"><span data-stu-id="d0371-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="d0371-114">**Catatan**: sertifikat ini DIKAITKAN dengan ID Apple yang digunakan untuk membuatnya.</span><span class="sxs-lookup"><span data-stu-id="d0371-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="d0371-115">Sebagai praktik terbaik, gunakan ID Apple perusahaan untuk tugas manajemen, dan pastikan kotak pesan dipantau oleh lebih dari satu orang atau dengan menggunakan daftar distribusi.</span><span class="sxs-lookup"><span data-stu-id="d0371-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="d0371-116">Jangan gunakan ID Apple pribadi.</span><span class="sxs-lookup"><span data-stu-id="d0371-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="d0371-117">Gunakan ID Apple yang sama untuk memperbarui Apple push Certificate setiap 12 bulan.</span><span class="sxs-lookup"><span data-stu-id="d0371-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="d0371-118">Masukkan ID Apple yang digunakan untuk membuat sertifikat push Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="d0371-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="d0371-119">Catat ID ini sebagai pengingat saat Anda perlu memperpanjang sertifikat.</span><span class="sxs-lookup"><span data-stu-id="d0371-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="d0371-120">Buka file Certificate (. pem), pilih **Open**, lalu pilih **upload**.</span><span class="sxs-lookup"><span data-stu-id="d0371-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="d0371-121">Dengan sertifikat push, Intune dapat mendaftarkan dan mengelola perangkat Apple.</span><span class="sxs-lookup"><span data-stu-id="d0371-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>