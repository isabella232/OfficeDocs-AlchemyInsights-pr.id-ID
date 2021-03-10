---
title: Masalah mereset kata sandi
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694378"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="acc66-102">Masalah mereset kata sandi</span><span class="sxs-lookup"><span data-stu-id="acc66-102">Problems resetting password</span></span>

<span data-ttu-id="acc66-103">Berikut ini adalah beberapa masalah yang mungkin Anda hadapi saat mereset kata sandi dan solusi yang memungkinkan:</span><span class="sxs-lookup"><span data-stu-id="acc66-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="acc66-104">**Saya mengalami masalah dengan penyetelan ulang kata sandi yang tidak tercakup dalam kategori lain**</span><span class="sxs-lookup"><span data-stu-id="acc66-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="acc66-105">Pastikan Anda memiliki wewenang untuk mengatur ulang kata sandi.</span><span class="sxs-lookup"><span data-stu-id="acc66-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="acc66-106">Hanya global, kata sandi, dan administrator pengguna yang bisa mereset kata sandi pengguna.</span><span class="sxs-lookup"><span data-stu-id="acc66-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="acc66-107">Administrator global juga dapat mengatur ulang kata sandi administrator istimewa lainnya.</span><span class="sxs-lookup"><span data-stu-id="acc66-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="acc66-108">Pastikan bahwa Anda memahami persyaratan Lisensi:</span><span class="sxs-lookup"><span data-stu-id="acc66-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="acc66-109">Anda harus memiliki setidaknya satu lisensi yang ditetapkan di organisasi Anda</span><span class="sxs-lookup"><span data-stu-id="acc66-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="acc66-110">Pengguna awan saja-SKU Office 365 (O365) berbayar apa pun, atau Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="acc66-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="acc66-111">Pengguna awan dan/atau di tempat-Azure AD Premium P1 atau P2, mobilitas perusahaan + keamanan (EMS), atau mengamankan perusahaan produktif (SPE)</span><span class="sxs-lookup"><span data-stu-id="acc66-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="acc66-112">Untuk membaca selengkapnya tentang persyaratan lisensi Lihat artikel [persyaratan lisensi untuk reset kata sandi layanan mandiri AZURE AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="acc66-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="acc66-113">**Saya mengalami masalah dalam menguji kebijakan penyetelan ulang kata sandi yang saya atur**</span><span class="sxs-lookup"><span data-stu-id="acc66-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="acc66-114">Kebijakan yang baru diterapkan dapat memakan waktu beberapa menit untuk mengulangi seluruh pusat data dan titik akhir.</span><span class="sxs-lookup"><span data-stu-id="acc66-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="acc66-115">Jarak fisik dari pusat data juga akan mempengaruhi seberapa cepat perubahan diterapkan.</span><span class="sxs-lookup"><span data-stu-id="acc66-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="acc66-116">Uji dengan pengguna akhir, bukan administrator, dan percobaan dengan sekelompok kecil pengguna.</span><span class="sxs-lookup"><span data-stu-id="acc66-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="acc66-117">Kebijakan yang dikonfigurasi di Azure portal hanya berlaku untuk pengguna akhir, bukan administrator.</span><span class="sxs-lookup"><span data-stu-id="acc66-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="acc66-118">Microsoft memberlakukan kebijakan penyetelan ulang kata sandi default yang kuat untuk setiap peran administrator Azure (contoh: administrator global, administrator Meja bantuan, administrator kata sandi, dsb.)</span><span class="sxs-lookup"><span data-stu-id="acc66-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="acc66-119">Pelajari selengkapnya tentang [kebijakan untuk administrator](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span><span class="sxs-lookup"><span data-stu-id="acc66-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="acc66-120">**Saya ingin menggunakan pengaturan ulang kata sandi tapi saya tidak ingin membuat pengguna saya mendaftarkan Info keamanan tambahan**</span><span class="sxs-lookup"><span data-stu-id="acc66-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="acc66-121">Pra-isi data untuk pengguna Anda sehingga mereka tidak harus!</span><span class="sxs-lookup"><span data-stu-id="acc66-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="acc66-122">-Sebagai administrator Anda bisa mengatur properti telepon dan email untuk pengguna Anda sebelum meluncurkan pengaturan ulang kata sandi ke organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="acc66-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="acc66-123">Anda dapat melakukan ini menggunakan API, PowerShell, atau Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="acc66-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="acc66-124">Informasi selengkapnya di sini:</span><span class="sxs-lookup"><span data-stu-id="acc66-124">More information here:</span></span>
- [<span data-ttu-id="acc66-125">Menyebarkan penyetelan ulang kata sandi tanpa mengharuskan pengguna untuk mendaftar</span><span class="sxs-lookup"><span data-stu-id="acc66-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="acc66-126">Data apa yang digunakan oleh reset kata sandi</span><span class="sxs-lookup"><span data-stu-id="acc66-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="acc66-127">**Tombol reset kata sandi berwarna abu-abu**</span><span class="sxs-lookup"><span data-stu-id="acc66-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="acc66-128">Anda tidak diizinkan untuk mereset kata sandi pengguna ini.</span><span class="sxs-lookup"><span data-stu-id="acc66-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="acc66-129">Hanya global, kata sandi, dan administrator pengguna yang bisa mereset kata sandi pengguna.</span><span class="sxs-lookup"><span data-stu-id="acc66-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="acc66-130">Administrator global juga dapat mengatur ulang kata sandi administrator istimewa lainnya.</span><span class="sxs-lookup"><span data-stu-id="acc66-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="acc66-131">**Saya tidak melihat Blade tata ulang kata sandi**</span><span class="sxs-lookup"><span data-stu-id="acc66-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="acc66-132">Anda tidak diberi wewenang untuk mengatur ulang kata sandi.</span><span class="sxs-lookup"><span data-stu-id="acc66-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="acc66-133">Hanya global, kata sandi, dan administrator pengguna yang bisa mereset kata sandi pengguna.</span><span class="sxs-lookup"><span data-stu-id="acc66-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="acc66-134">Administrator global juga dapat mengatur ulang kata sandi administrator istimewa lainnya.</span><span class="sxs-lookup"><span data-stu-id="acc66-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="acc66-135">**Saya tidak melihat Blade integrasi lokal dalam pengaturan ulang kata sandi**</span><span class="sxs-lookup"><span data-stu-id="acc66-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="acc66-136">Bilah integrasi lokal hanya muncul di lingkungan hibrid-artinya Anda menggunakan tulis balik kata sandi untuk memanipulasi kata sandi pengguna di tempat.</span><span class="sxs-lookup"><span data-stu-id="acc66-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="acc66-137">Anda tidak melihat pisau ini jika:</span><span class="sxs-lookup"><span data-stu-id="acc66-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="acc66-138">Anda tidak menggunakan tulis balik kata sandi</span><span class="sxs-lookup"><span data-stu-id="acc66-138">You are not using password writeback</span></span>
    - <span data-ttu-id="acc66-139">Ada masalah dengan instalasi/konektivitas tulis balik kata sandi Anda</span><span class="sxs-lookup"><span data-stu-id="acc66-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="acc66-140">Ada masalah dengan instalasi/konektivitas Azure AD Connect Anda</span><span class="sxs-lookup"><span data-stu-id="acc66-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="acc66-141">Untuk langkah pemecahan masalah lainnya untuk masalah dengan tulis balik kata sandi, lihat bagian [memecahkan masalah tulis balik kata sandi](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="acc66-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="acc66-142">**Saya tidak tahu cara mengatur ulang kata sandi pengguna**</span><span class="sxs-lookup"><span data-stu-id="acc66-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="acc66-143">Masuk ke Azure Portal sebagai admin yang sesuai.</span><span class="sxs-lookup"><span data-stu-id="acc66-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="acc66-144">Masuk ke bilah pengguna dan grup, pilih **semua pengguna**.</span><span class="sxs-lookup"><span data-stu-id="acc66-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="acc66-145">Pilih pengguna dari daftar.</span><span class="sxs-lookup"><span data-stu-id="acc66-145">Select a user from the list.</span></span>
1. <span data-ttu-id="acc66-146">Untuk pengguna yang dipilih, pilih **gambaran umum**, lalu di bilah perintah, klik **reset kata sandi**.</span><span class="sxs-lookup"><span data-stu-id="acc66-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="acc66-147">Ikuti instruksi di layar.</span><span class="sxs-lookup"><span data-stu-id="acc66-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="acc66-148">Hanya mereset yang dilakukan melalui Azure portal mendukung tulis balik kata sandi.</span><span class="sxs-lookup"><span data-stu-id="acc66-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="acc66-149">**Saya mengatur ulang kata sandi pengguna lokal dari portal admin Office 365 atau aplikasi seluler Office 365 tapi pengguna masih belum dapat masuk**</span><span class="sxs-lookup"><span data-stu-id="acc66-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="acc66-150">Tulis balik kata sandi tidak didukung di portal ini.</span><span class="sxs-lookup"><span data-stu-id="acc66-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="acc66-151">Mengatur ulang kata sandi pengguna lagi di portal Azure-portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="acc66-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

