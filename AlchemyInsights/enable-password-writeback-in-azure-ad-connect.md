---
title: Aktifkan tulis balik kata sandi di Azure AD Connect
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
- "9002933"
- "5615"
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093358"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="d3673-102">Aktifkan tulis balik kata sandi di Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="d3673-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="d3673-103">Untuk mengaktifkan tulis balik pengaturan ulang kata sandi mandiri, aktifkan terlebih dahulu opsi tulis balik di Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="d3673-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="d3673-104">Dari server Azure AD Connect Anda, lakukan langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="d3673-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="d3673-105">Masuk ke server Azure AD Connect Anda dan mulai panduan konfigurasi **Azure AD Connect**.</span><span class="sxs-lookup"><span data-stu-id="d3673-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="d3673-106">Pada halaman **Selamat Datang**, klik **Konfigurasi**.</span><span class="sxs-lookup"><span data-stu-id="d3673-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="d3673-107">Pada halaman **Tugas tambahan**, pilih **Kustomisasi opsi sinkronisasi**, lalu klik **Lanjut**.</span><span class="sxs-lookup"><span data-stu-id="d3673-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="d3673-108">Pada halaman **Sambungkan ke Azure AD**, masukkan kredensial administrator global untuk penyewa Azure Anda, lalu klik **Lanjut**.</span><span class="sxs-lookup"><span data-stu-id="d3673-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="d3673-109">Pada halaman **Sambungkan direktori** dan pemfilteran **Domain/OU**, klik **Lanjut**.</span><span class="sxs-lookup"><span data-stu-id="d3673-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="d3673-110">Pada halaman **Fitur opsional**, pilih kotak di sebelah **Tulis balik kata sandi** dan klik **Lanjut**.</span><span class="sxs-lookup"><span data-stu-id="d3673-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="d3673-111">Pada halaman **Siap untuk mengonfigurasi**, klik **Konfigurasi** dan tunggu prosesnya selesai.</span><span class="sxs-lookup"><span data-stu-id="d3673-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="d3673-112">Saat Anda melihat konfigurasi selesai, klik **Keluar**.</span><span class="sxs-lookup"><span data-stu-id="d3673-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="d3673-113">Dengan tulis balik kata sandi diaktifkan di Azure AD Connect, konfigurasikan SSPR Azure AD untuk tulis balik.</span><span class="sxs-lookup"><span data-stu-id="d3673-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="d3673-114">Untuk mengaktifkan tulis balik kata sandi di SSPR, lakukan langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="d3673-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="d3673-115">Masuk ke portal Microsoft Azure dengan menggunakan akun administrator global.</span><span class="sxs-lookup"><span data-stu-id="d3673-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="d3673-116">Cari dan pilih **Azure Active Directory**, klik **Reset kata sandi**, lalu klik **Integrasi lokal**.</span><span class="sxs-lookup"><span data-stu-id="d3673-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="d3673-117">Atur opsi untuk **Tulis ulang kata sandi ke direktori lokal Anda?** ke **Ya**.</span><span class="sxs-lookup"><span data-stu-id="d3673-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="d3673-118">Atur opsi untuk **Izinkan pengguna untuk membuka kunci akun tanpa mereset kata sandi?** ke **Ya**.</span><span class="sxs-lookup"><span data-stu-id="d3673-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="d3673-119">Jika sudah siap, klik **Simpan**.</span><span class="sxs-lookup"><span data-stu-id="d3673-119">When ready, click **Save**.</span></span>

<span data-ttu-id="d3673-120">Untuk informasi selengkapnya, lihat [Mengaktifkan tulis balik pengaturan ulang kata sandi mandiri Azure Active Directory ke lingkungan lokal](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="d3673-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="d3673-121">Saat administrator mereset kata sandi pengguna di Portal Microsoft Azure, jika pengguna tersebut gabungan atau hash kata sandi disinkronkan, kata sandi tersebut akan ditulis ulang ke lokal.</span><span class="sxs-lookup"><span data-stu-id="d3673-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="d3673-122">Fungsionalitas ini memerlukan Lisensi Azure Premium (P1 atau P2) dan saat ini tidak didukung di portal Admin Office.</span><span class="sxs-lookup"><span data-stu-id="d3673-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
