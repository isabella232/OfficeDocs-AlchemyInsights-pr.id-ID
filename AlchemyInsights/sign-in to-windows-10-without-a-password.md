---
title: Masuk ke Windows 10 tanpa menggunakan kata sandi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588284"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="5fb0a-102">Masuk ke Windows 10 tanpa menggunakan kata sandi</span><span class="sxs-lookup"><span data-stu-id="5fb0a-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="5fb0a-103">Untuk menghindari keharusan mengetikkan kata sandi pada startup Windows, sebaiknya gunakan salah satu opsi masuk aman Windows Hello, seperti PIN, pengenalan wajah, atau sidik jari, jika tersedia.</span><span class="sxs-lookup"><span data-stu-id="5fb0a-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="5fb0a-104">Jika Anda ingin menonaktifkan proses masuk yang aman, Lihat petunjuk "masuk secara otomatis ke Windows 10" di bawah.</span><span class="sxs-lookup"><span data-stu-id="5fb0a-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="5fb0a-105">**Mengamankan alternatif Windows Hello ke kata sandi akun**</span><span class="sxs-lookup"><span data-stu-id="5fb0a-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="5fb0a-106">Buka **pengaturan > akun > opsi masuk** (atau klik [di sini](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="5fb0a-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="5fb0a-107">Opsi masuk yang tersedia akan dicantumkan.</span><span class="sxs-lookup"><span data-stu-id="5fb0a-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="5fb0a-108">Misalnya:</span><span class="sxs-lookup"><span data-stu-id="5fb0a-108">For example:</span></span>

![Opsi masuk.](media/sign-in-options.png)

<span data-ttu-id="5fb0a-110">Klik atau ketuk salah satu opsi untuk mengonfigurasikannya.</span><span class="sxs-lookup"><span data-stu-id="5fb0a-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="5fb0a-111">Lain kali Anda memulai atau membuka kunci Windows, Anda akan dapat menggunakan opsi baru daripada kata sandi.</span><span class="sxs-lookup"><span data-stu-id="5fb0a-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="5fb0a-112">**Masuk secara otomatis ke Windows 10**</span><span class="sxs-lookup"><span data-stu-id="5fb0a-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="5fb0a-113">**Catatan**: masuk otomatis nyaman, tetapi memperkenalkan risiko keamanan, terutama jika PC Anda dapat diakses oleh beberapa orang.</span><span class="sxs-lookup"><span data-stu-id="5fb0a-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="5fb0a-114">Klik atau ketuk tombol **Start** di taskbar.</span><span class="sxs-lookup"><span data-stu-id="5fb0a-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="5fb0a-115">Ketik **netplwiz** dan tekan tombol Enter untuk membuka jendela akun pengguna.</span><span class="sxs-lookup"><span data-stu-id="5fb0a-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="5fb0a-116">Di **akun pengguna**, klik akun yang ingin Anda masuki secara otomatis saat Windows dimulai.</span><span class="sxs-lookup"><span data-stu-id="5fb0a-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="5fb0a-117">Hapus tanda centang pada kotak centang "pengguna harus memasukkan nama pengguna dan sandi untuk menggunakan komputer ini".</span><span class="sxs-lookup"><span data-stu-id="5fb0a-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Pengguna harus memasukkan pilihan username dan password.](media/users-must-enter-username.png)

5. <span data-ttu-id="5fb0a-119">Klik **OK**.</span><span class="sxs-lookup"><span data-stu-id="5fb0a-119">Click **OK**.</span></span> <span data-ttu-id="5fb0a-120">Anda akan diminta untuk memasukkan dan mengonfirmasi kata sandi untuk akun yang Anda pilih.</span><span class="sxs-lookup"><span data-stu-id="5fb0a-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="5fb0a-121">Klik **OK** untuk menyelesaikan.</span><span class="sxs-lookup"><span data-stu-id="5fb0a-121">Click **OK** to finish.</span></span> <span data-ttu-id="5fb0a-122">Lain kali Windows 10 dimulai, maka secara otomatis akan masuk ke account yang Anda pilih.</span><span class="sxs-lookup"><span data-stu-id="5fb0a-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
