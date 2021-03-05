---
title: Sinkronisasi kata sandi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482037"
---
# <a name="password-synchronization"></a><span data-ttu-id="0fc34-102">Sinkronisasi kata sandi</span><span class="sxs-lookup"><span data-stu-id="0fc34-102">Password synchronization</span></span>

<span data-ttu-id="0fc34-103">**Sinkronisasi hash kata sandi tidak berfungsi sama sekali**</span><span class="sxs-lookup"><span data-stu-id="0fc34-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="0fc34-104">Beberapa masalah umum yang dihadapi pelanggan ketika sinkronisasi hash kata sandi tidak berfungsi:</span><span class="sxs-lookup"><span data-stu-id="0fc34-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="0fc34-105">Akun direktori aktif yang digunakan oleh Azure AD Connect untuk berkomunikasi dengan direktori aktif di tempat tidak diberikan **replikasi perubahan direktori** dan **replikasi perubahan direktori semua** izin, yang diperlukan untuk sinkronisasi kata sandi-Anda perlu memperbaikinya dengan memberikan izin ini ke akun direktori aktif.</span><span class="sxs-lookup"><span data-stu-id="0fc34-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="0fc34-106">Sinkronisasi hash kata sandi dinonaktifkan setelah administrator mengubah metode Sign-In pengguna dari **sinkronisasi kata sandi** ke opsi lain seperti **Federasi dengan AD FS** dalam panduan Azure AD Connect-Anda bisa memperbaikinya dengan mengaktifkan ulang fitur **sinkronisasi hash kata sandi** dalam panduan Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="0fc34-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="0fc34-107">Masalah konektivitas dengan direktori aktif di tempat.</span><span class="sxs-lookup"><span data-stu-id="0fc34-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="0fc34-108">Misalnya, beberapa pengontrol domain tidak dapat diakses oleh Azure AD Connect, atau port yang [diperlukan](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) diblokir oleh firewall-Anda harus memperbaikinya dengan memastikan bahwa konektivitas antara server Azure AD Connect dan direktori aktif di tempat berfungsi dengan benar.</span><span class="sxs-lookup"><span data-stu-id="0fc34-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="0fc34-109">Server Azure AD Connect sedang berada dalam mode pementasan, yang akan menyebabkan server tidak bisa menggunakan hash kata sandi-untuk memecahkan masalah, ikuti langkah-langkah yang diuraikan dalam [memecahkan masalah sinkronisasi kata sandi dengan sinkronisasi AZURE AD Connect-tidak ada kata sandi yang disinkronkan](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="0fc34-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="0fc34-110">**Sinkronisasi hash kata sandi tidak berfungsi untuk beberapa pengguna saya**</span><span class="sxs-lookup"><span data-stu-id="0fc34-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="0fc34-111">Jika Anda melihat bahwa hash kata sandi tidak disinkronkan untuk pengguna, gunakan tugas **pemecahan masalah** di Azure AD Connect untuk menyelidiki dan mengatasi masalah tersebut.</span><span class="sxs-lookup"><span data-stu-id="0fc34-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="0fc34-112">Melakukan tugas berikut:</span><span class="sxs-lookup"><span data-stu-id="0fc34-112">Perform the following tasks:</span></span>

    <span data-ttu-id="0fc34-113">untuk.</span><span class="sxs-lookup"><span data-stu-id="0fc34-113">a.</span></span> [<span data-ttu-id="0fc34-114">Menjalankan tugas pemecahan masalah dalam panduan</span><span class="sxs-lookup"><span data-stu-id="0fc34-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="0fc34-115">b.</span><span class="sxs-lookup"><span data-stu-id="0fc34-115">b.</span></span> [<span data-ttu-id="0fc34-116">Menggunakan cmdlet pemecahan masalah untuk menyelidiki masalah sinkronisasi hash kata sandi untuk penggunaan tertentu</span><span class="sxs-lookup"><span data-stu-id="0fc34-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="0fc34-117">Objek pengguna Active Directory lokal diaktifkan untuk opsi **pengguna harus mengubah kata sandi pada logon berikutnya** .</span><span class="sxs-lookup"><span data-stu-id="0fc34-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="0fc34-118">Ketika opsi ini diaktifkan, pengguna diberi kata sandi sementara dan akan diminta untuk mengubah kata sandi pada logon berikutnya.</span><span class="sxs-lookup"><span data-stu-id="0fc34-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="0fc34-119">Azure AD Connect tidak menyinkronkan kata sandi sementara ke Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0fc34-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="0fc34-120">Untuk mengatasi masalah di atas, lakukan salah satu tugas berikut:</span><span class="sxs-lookup"><span data-stu-id="0fc34-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="0fc34-121">Minta pengguna untuk masuk ke aplikasi di tempat (misalnya, desktop Windows) dan ubah kata sandinya.</span><span class="sxs-lookup"><span data-stu-id="0fc34-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="0fc34-122">Kata sandi baru akan disinkronkan ke Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0fc34-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="0fc34-123">Memiliki administrator yang memperbarui kata sandi pengguna tanpa mengaktifkan opsi **pengguna harus mengubah kata sandi pada logon berikutnya**, dan berbagi kata sandi baru dengan pengguna.</span><span class="sxs-lookup"><span data-stu-id="0fc34-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="0fc34-124">Objek pengguna direktori aktif lokal **tidak dikonfigurasi dengan benar** untuk sinkronisasi objek atau sinkronisasi kata sandi.</span><span class="sxs-lookup"><span data-stu-id="0fc34-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="0fc34-125">Untuk memecahkan masalah ini, ikuti langkah-langkah yang diuraikan dalam [memecahkan sinkronisasi hash kata sandi dengan sinkronisasi AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="0fc34-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







