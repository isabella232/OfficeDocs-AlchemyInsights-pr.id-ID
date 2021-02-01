---
title: Masalah dengan kredensial
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063678"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="51b6e-102">Masalah dengan kredensial</span><span class="sxs-lookup"><span data-stu-id="51b6e-102">Issues with credentials</span></span>

<span data-ttu-id="51b6e-103">[Platform identitas Microsoft dan aliran kredensial klien 2,0 OAuth](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) menjelaskan cara program langsung terhadap aliran hibah kredensial klien OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="51b6e-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="51b6e-104">**Bagaimana cara mengelola kredensial kata sandi atau sertifikat aplikasi?**</span><span class="sxs-lookup"><span data-stu-id="51b6e-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="51b6e-105">Di Azure CLI, Anda bisa menggunakan [kredensial aplikasi AZ AD](https://docs.microsoft.com/cli/azure/ad/app/credential) untuk menghapus, membuat daftar, atau mereset kata sandi atau kredensial sertifikat aplikasi.</span><span class="sxs-lookup"><span data-stu-id="51b6e-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="51b6e-106">**Bagaimana cara pengguna mereset kata sandi mereka?**</span><span class="sxs-lookup"><span data-stu-id="51b6e-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="51b6e-107">Pengguna harus [mendaftar untuk mereset kata sandi layanan mandiri](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) sebelum mereka bisa mereset kata sandinya.</span><span class="sxs-lookup"><span data-stu-id="51b6e-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="51b6e-108">Setelah pengguna mendaftar, mereka bisa mengikuti instruksi dalam artikel ini untuk mereset kata sandinya: [mereset kata sandi kantor atau sekolah Anda](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span><span class="sxs-lookup"><span data-stu-id="51b6e-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="51b6e-109">**Bagaimana cara pengguna mengubah kata sandi mereka?**</span><span class="sxs-lookup"><span data-stu-id="51b6e-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="51b6e-110">Pengguna dapat mengikuti langkah-langkah dalam artikel ini untuk mengubah kata sandinya: [cara mengubah kata sandi Anda](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span><span class="sxs-lookup"><span data-stu-id="51b6e-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="51b6e-111">Mereka juga bisa [mengelola kata sandi aplikasi untuk verifikasi dua langkah](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span><span class="sxs-lookup"><span data-stu-id="51b6e-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="51b6e-112">**Pengguna saya mendapatkan pesan kesalahan saat mengubah atau mengatur ulang kata sandi**</span><span class="sxs-lookup"><span data-stu-id="51b6e-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="51b6e-113">Link ini akan memberikan informasi tentang masalah umum yang dapat muncul saat pengguna mencoba mereset kata sandinya: [masalah umum dan solusinya](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="51b6e-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="51b6e-114">**Saya mengalami masalah mereset kata sandi pengguna**</span><span class="sxs-lookup"><span data-stu-id="51b6e-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="51b6e-115">Pastikan Anda memiliki wewenang untuk mengatur ulang kata sandi.</span><span class="sxs-lookup"><span data-stu-id="51b6e-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="51b6e-116">*Hanya global, kata sandi, dan administrator pengguna yang bisa mereset kata sandi pengguna.*</span><span class="sxs-lookup"><span data-stu-id="51b6e-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="51b6e-117">Administrator global juga dapat mengatur ulang kata sandi administrator istimewa lainnya.</span><span class="sxs-lookup"><span data-stu-id="51b6e-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="51b6e-118">Pastikan Anda memahami persyaratan Lisensi:</span><span class="sxs-lookup"><span data-stu-id="51b6e-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="51b6e-119">Anda harus memiliki setidaknya satu lisensi yang ditetapkan di organisasi Anda:</span><span class="sxs-lookup"><span data-stu-id="51b6e-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="51b6e-120">**Pengguna awan saja** -SKU Office 365 (O365) berbayar apa pun, atau Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="51b6e-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="51b6e-121">**Pengguna awan dan/atau di** tempat-Azure AD Premium P1 atau P2, mobilitas perusahaan + keamanan (EMS), atau mengamankan perusahaan produktif (SPE)</span><span class="sxs-lookup"><span data-stu-id="51b6e-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="51b6e-122">Untuk mempelajari selengkapnya tentang persyaratan lisensi, lihat [persyaratan lisensi untuk pengaturan ulang kata sandi layanan mandiri AZURE AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span><span class="sxs-lookup"><span data-stu-id="51b6e-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="51b6e-123">Untuk mengatur ulang kata sandi pengguna, temukan pengguna di Azure AD.</span><span class="sxs-lookup"><span data-stu-id="51b6e-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="51b6e-124">Lalu, pada bilah gambaran umum untuk pengguna tersebut, klik tombol "Atur ulang kata sandi."</span><span class="sxs-lookup"><span data-stu-id="51b6e-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="51b6e-125">**Tombol reset kata sandi berwarna abu-abu**</span><span class="sxs-lookup"><span data-stu-id="51b6e-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="51b6e-126">Anda tidak diizinkan untuk mereset kata sandi pengguna **ini** .</span><span class="sxs-lookup"><span data-stu-id="51b6e-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="51b6e-127">*Hanya global, kata sandi, dan administrator pengguna yang bisa mereset kata sandi pengguna.*</span><span class="sxs-lookup"><span data-stu-id="51b6e-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="51b6e-128">Administrator global juga dapat mengatur ulang kata sandi administrator istimewa lainnya.</span><span class="sxs-lookup"><span data-stu-id="51b6e-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="51b6e-129">**Saya tidak melihat Blade tata ulang kata sandi**</span><span class="sxs-lookup"><span data-stu-id="51b6e-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="51b6e-130">Anda tidak diberi wewenang untuk mengatur ulang kata sandi.</span><span class="sxs-lookup"><span data-stu-id="51b6e-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="51b6e-131">*Hanya global, kata sandi, dan administrator pengguna yang bisa mereset kata sandi pengguna.*</span><span class="sxs-lookup"><span data-stu-id="51b6e-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="51b6e-132">Administrator global juga dapat mengatur ulang kata sandi administrator istimewa lainnya.</span><span class="sxs-lookup"><span data-stu-id="51b6e-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="51b6e-133">**Saya tidak melihat Blade integrasi lokal dalam pengaturan ulang kata sandi**</span><span class="sxs-lookup"><span data-stu-id="51b6e-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="51b6e-134">Bilah integrasi lokal hanya muncul di lingkungan hibrid-artinya Anda menggunakan tulis balik kata sandi untuk memanipulasi kata sandi pengguna di tempat.</span><span class="sxs-lookup"><span data-stu-id="51b6e-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="51b6e-135">Anda tidak melihat pisau ini jika:</span><span class="sxs-lookup"><span data-stu-id="51b6e-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="51b6e-136">Anda tidak menggunakan tulis balik kata sandi</span><span class="sxs-lookup"><span data-stu-id="51b6e-136">You are not using password writeback</span></span>
  - <span data-ttu-id="51b6e-137">Ada masalah dengan instalasi/konektivitas tulis balik kata sandi Anda</span><span class="sxs-lookup"><span data-stu-id="51b6e-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="51b6e-138">Ada masalah dengan instalasi/konektivitas Azure AD Connect Anda</span><span class="sxs-lookup"><span data-stu-id="51b6e-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="51b6e-139">Untuk langkah pemecahan masalah lainnya untuk masalah dengan tulis balik kata sandi, lihat [memecahkan masalah tulis balik kata sandi](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="51b6e-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="51b6e-140">**Saya tidak tahu cara mengatur ulang kata sandi pengguna**</span><span class="sxs-lookup"><span data-stu-id="51b6e-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="51b6e-141">Masuk ke Azure Portal sebagai admin yang sesuai.</span><span class="sxs-lookup"><span data-stu-id="51b6e-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="51b6e-142">Masuk ke bilah **pengguna dan grup** , pilih **semua pengguna**.</span><span class="sxs-lookup"><span data-stu-id="51b6e-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="51b6e-143">Pilih pengguna dari daftar.</span><span class="sxs-lookup"><span data-stu-id="51b6e-143">Select a user from the list.</span></span>
4. <span data-ttu-id="51b6e-144">Untuk pengguna yang dipilih, pilih **gambaran umum**, lalu di bilah perintah, pilih **reset kata sandi**.</span><span class="sxs-lookup"><span data-stu-id="51b6e-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="51b6e-145">Pilih tombol **reset kata sandi** dan ikuti instruksi di layar.</span><span class="sxs-lookup"><span data-stu-id="51b6e-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="51b6e-146">Hanya mereset yang dilakukan melalui **Azure portal** mendukung tulis balik kata sandi.</span><span class="sxs-lookup"><span data-stu-id="51b6e-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="51b6e-147">**Saya mengatur ulang kata sandi pengguna lokal dari portal admin Office 365 atau aplikasi seluler Office 365 tapi pengguna masih belum dapat masuk**</span><span class="sxs-lookup"><span data-stu-id="51b6e-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="51b6e-148">Tulis balik kata sandi tidak didukung di portal ini.</span><span class="sxs-lookup"><span data-stu-id="51b6e-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="51b6e-149">Atur ulang kata sandi pengguna lagi di portal Azure.</span><span class="sxs-lookup"><span data-stu-id="51b6e-149">Reset the user's password again in the Azure portal.</span></span>
