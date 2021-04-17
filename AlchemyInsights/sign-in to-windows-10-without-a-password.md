---
title: Masuk ke Windows 10 tanpa menggunakan kata sandi
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830549"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="14052-102">Masuk ke Windows 10 tanpa menggunakan kata sandi</span><span class="sxs-lookup"><span data-stu-id="14052-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="14052-103">Untuk menghindari harus mengetikkan kata sandi pada startup Windows, kami menyarankan Anda menggunakan salah satu opsi masuk aman Windows Hello, seperti PIN, pengenalan wajah, atau sidik jari, jika tersedia.</span><span class="sxs-lookup"><span data-stu-id="14052-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="14052-104">Jika Anda benar-benar ingin menonaktifkan akses masuk yang aman, lihat instruksi "Masuk secara otomatis ke Windows 10" di bawah ini.</span><span class="sxs-lookup"><span data-stu-id="14052-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="14052-105">**Mengamankan alternatif Windows Hello dengan kata sandi akun**</span><span class="sxs-lookup"><span data-stu-id="14052-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="14052-106">Masuk ke **Pengaturan > Akun > opsi Masuk (atau** klik di [sini](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="14052-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="14052-107">Opsi masuk yang tersedia akan dicantumkan.</span><span class="sxs-lookup"><span data-stu-id="14052-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="14052-108">Misalnya:</span><span class="sxs-lookup"><span data-stu-id="14052-108">For example:</span></span>

![Opsi masuk.](media/sign-in-options.png)

<span data-ttu-id="14052-110">Klik atau ketuk salah satu opsi untuk mengonfigurasinya.</span><span class="sxs-lookup"><span data-stu-id="14052-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="14052-111">Saat berikutnya Anda memulai atau membuka kunci Windows, Anda akan bisa menggunakan opsi baru sebagai ganti kata sandi.</span><span class="sxs-lookup"><span data-stu-id="14052-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="14052-112">**Masuk ke Windows 10 secara otomatis**</span><span class="sxs-lookup"><span data-stu-id="14052-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="14052-113">**Catatan**: Masuk otomatis mudah, tetapi menghadirkan risiko keamanan, terutama jika PC Anda dapat diakses oleh beberapa orang.</span><span class="sxs-lookup"><span data-stu-id="14052-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="14052-114">Klik atau ketuk **tombol** Mulai di Taskbar.</span><span class="sxs-lookup"><span data-stu-id="14052-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="14052-115">Ketik **netplwiz** dan tekan tombol Enter untuk membuka jendela Akun Pengguna.</span><span class="sxs-lookup"><span data-stu-id="14052-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="14052-116">Di **Akun Pengguna,** klik akun yang ingin Anda masuki secara otomatis saat Windows dimulai.</span><span class="sxs-lookup"><span data-stu-id="14052-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="14052-117">Kosongkan kotak centang "Pengguna harus memasukkan nama pengguna dan kata sandi untuk menggunakan komputer ini".</span><span class="sxs-lookup"><span data-stu-id="14052-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Pengguna harus memasukkan nama pengguna dan opsi kata sandi.](media/users-must-enter-username.png)

5. <span data-ttu-id="14052-119">Klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="14052-119">Click **OK**.</span></span> <span data-ttu-id="14052-120">Anda akan diminta untuk memasukkan dan mengonfirmasi kata sandi untuk akun yang dipilih.</span><span class="sxs-lookup"><span data-stu-id="14052-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="14052-121">Klik **OK** untuk menyelesaikannya.</span><span class="sxs-lookup"><span data-stu-id="14052-121">Click **OK** to finish.</span></span> <span data-ttu-id="14052-122">Di waktu berikutnya Windows 10 dimulai, Windows 10 akan masuk secara otomatis ke akun yang Anda pilih.</span><span class="sxs-lookup"><span data-stu-id="14052-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
