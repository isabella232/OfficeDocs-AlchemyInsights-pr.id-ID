---
title: Masuk ke Windows 10 tanpa menggunakan kata sandi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719956"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="54f36-102">Masuk ke Windows 10 tanpa menggunakan kata sandi</span><span class="sxs-lookup"><span data-stu-id="54f36-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="54f36-103">Untuk menghindari keharusan mengetikkan kata sandi di startup Windows, kami menyarankan agar Anda menggunakan salah satu opsi masuk Windows Hello yang aman, seperti PIN, pengenalan wajah, atau sidik jari, jika tersedia.</span><span class="sxs-lookup"><span data-stu-id="54f36-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="54f36-104">Jika Anda benar-benar ingin menonaktifkan aman masuk, lihat instruksi "masuk otomatis ke Windows 10" di bawah ini.</span><span class="sxs-lookup"><span data-stu-id="54f36-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="54f36-105">**Mengamankan Windows Hello alternatif untuk kata sandi akun**</span><span class="sxs-lookup"><span data-stu-id="54f36-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="54f36-106">Masuk ke **pengaturan > akun > opsi masuk** (atau klik [di sini](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="54f36-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="54f36-107">Opsi masuk yang tersedia akan dicantumkan.</span><span class="sxs-lookup"><span data-stu-id="54f36-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="54f36-108">Misalnya:</span><span class="sxs-lookup"><span data-stu-id="54f36-108">For example:</span></span>

![Opsi masuk.](media/sign-in-options.png)

<span data-ttu-id="54f36-110">Klik atau ketuk salah satu opsi untuk mengonfigurasinya.</span><span class="sxs-lookup"><span data-stu-id="54f36-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="54f36-111">Saat berikutnya Anda memulai atau membuka kunci Windows, Anda akan dapat menggunakan opsi baru, bukan kata sandi.</span><span class="sxs-lookup"><span data-stu-id="54f36-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="54f36-112">**Masuk secara otomatis ke Windows 10**</span><span class="sxs-lookup"><span data-stu-id="54f36-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="54f36-113">**Catatan**: masuk otomatis mudah, namun memperkenalkan risiko keamanan, terutama jika PC Anda dapat diakses oleh beberapa orang.</span><span class="sxs-lookup"><span data-stu-id="54f36-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="54f36-114">Klik atau ketuk tombol **mulai** di taskbar.</span><span class="sxs-lookup"><span data-stu-id="54f36-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="54f36-115">Ketik **netplwiz** dan tekan tombol Enter untuk membuka jendela akun pengguna.</span><span class="sxs-lookup"><span data-stu-id="54f36-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="54f36-116">Di **akun pengguna**, klik akun yang ingin Anda masuki secara otomatis saat Windows dimulai.</span><span class="sxs-lookup"><span data-stu-id="54f36-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="54f36-117">Kosongkan kotak centang "pengguna harus memasukkan nama pengguna dan kata sandi untuk menggunakan komputer ini".</span><span class="sxs-lookup"><span data-stu-id="54f36-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Pengguna harus memasukkan opsi nama pengguna dan kata sandi.](media/users-must-enter-username.png)

5. <span data-ttu-id="54f36-119">Klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="54f36-119">Click **OK**.</span></span> <span data-ttu-id="54f36-120">Anda akan diminta untuk memasukkan dan mengonfirmasi kata sandi untuk akun yang Anda pilih.</span><span class="sxs-lookup"><span data-stu-id="54f36-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="54f36-121">Klik **OK** untuk menyelesaikan.</span><span class="sxs-lookup"><span data-stu-id="54f36-121">Click **OK** to finish.</span></span> <span data-ttu-id="54f36-122">Saat berikutnya Windows 10 dimulai, akan otomatis masuk ke akun yang Anda pilih.</span><span class="sxs-lookup"><span data-stu-id="54f36-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
