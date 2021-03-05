---
title: Mengonfigurasi Layanan penyediaan
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482870"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="4bbd7-102">Mengonfigurasi Layanan penyediaan</span><span class="sxs-lookup"><span data-stu-id="4bbd7-102">Configuring the Provision service</span></span>

<span data-ttu-id="4bbd7-103">Untuk penyediaan pengguna otomatis agar berfungsi, Azure AD memerlukan kredensial yang valid yang memungkinkan untuk menyambungkan ke Workday Web Services API.</span><span class="sxs-lookup"><span data-stu-id="4bbd7-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="4bbd7-104">Selain itu, tombol uji koneksi pada hari kerja ke aplikasi penyediaan pengguna AD juga memvalidasi jika dapat tersambung ke agen bawaan Azure AD Connect yang terkait dengan domain AD.</span><span class="sxs-lookup"><span data-stu-id="4bbd7-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="4bbd7-105">Jika Azure portal mengembalikan kesalahan saat menyimpan kredensial, ikuti langkah-langkah di bawah ini:</span><span class="sxs-lookup"><span data-stu-id="4bbd7-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="4bbd7-106">Konfirmasi bahwa Anda telah mengonfigurasi akun pengguna sistem integrasi kerja seperti yang dinyatakan dalam bagian tutorial [mengonfigurasikan pengguna sistem integrasi di workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="4bbd7-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="4bbd7-107">Konfirmasi bahwa layanan agen Azure AD Connect bawaan sudah aktif dan berjalan di server Windows lokal Anda menggunakan konsol Manajemen Layanan.</span><span class="sxs-lookup"><span data-stu-id="4bbd7-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="4bbd7-108">Anda juga bisa memeriksa status agen di portal Azure dengan mengklik tombol Tampilkan agen lokal.</span><span class="sxs-lookup"><span data-stu-id="4bbd7-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="4bbd7-109">Pastikan bahwa Anda memasukkan nilai untuk bidang "nama pengguna Workday" menggunakan nama username@workday-penyewa format.</span><span class="sxs-lookup"><span data-stu-id="4bbd7-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="4bbd7-110">Jika nama kerja-penyewa tidak hilang, maka hari kerja autentikasi gagal.</span><span class="sxs-lookup"><span data-stu-id="4bbd7-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="4bbd7-111">Jika Anda mengonfigurasi integrasi dengan penyewa implementasi hari kerja, perhatikan jam henti terjadwal dari penyewa hari kerja Anda.</span><span class="sxs-lookup"><span data-stu-id="4bbd7-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="4bbd7-112">Workday telah menjadwalkan waktu untuk penyewa pelaksanaannya selama akhir pekan (biasanya dari Jumat sore hingga Sabtu pagi) dan kegagalan konektivitas selama jendela downtime ini adalah masalah umum yang diselesaikan secara otomatis segera setelah penyewa pelaksana kembali online.</span><span class="sxs-lookup"><span data-stu-id="4bbd7-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="4bbd7-113">Dalam kasus yang jarang, Anda mungkin juga melihat kesalahan ini jika kata sandi pengguna sistem integrasi berubah karena refresh penyewa atau jika akun tersebut dalam status dikunci atau kedaluwarsa.</span><span class="sxs-lookup"><span data-stu-id="4bbd7-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="4bbd7-114">Periksa status pengguna sistem integrasi dengan administrator Workday Anda.</span><span class="sxs-lookup"><span data-stu-id="4bbd7-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="4bbd7-115">Untuk detail selengkapnya tentang mengonfigurasi workday untuk penyediaan otomatis, lihat [Tutorial: mengonfigurasi workday untuk penyediaan pengguna otomatis](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="4bbd7-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
