---
title: Gunakan TeamViewer untuk mengelola perangkat Intune dari jarak jauh
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555240"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="78b69-102">Gunakan TeamViewer untuk mengelola perangkat Intune dari jarak jauh</span><span class="sxs-lookup"><span data-stu-id="78b69-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="78b69-103">Perangkat yang dikelola oleh Intune dapat diberikan dari jarak jauh dengan menggunakan [TeamViewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="78b69-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="78b69-104">Untuk mengelola Intune menggunakan TeamViewer, gunakan langkah berikut:</span><span class="sxs-lookup"><span data-stu-id="78b69-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="78b69-105">Mulailah dengan mendapatkan kredensial dari TeamViewer untuk mengatur konektor TeamViewer di Intune.</span><span class="sxs-lookup"><span data-stu-id="78b69-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="78b69-106">Hal ini memungkinkan admin untuk memasukkan kredensial dalam TeamViewer Connector UI di bawah perangkat, operasi satu kali untuk menetapkan hubungan antara Intune dan layanan TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="78b69-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="78b69-107">**Bagian 1: mulai sesi dengan perangkat jarak jauh**</span><span class="sxs-lookup"><span data-stu-id="78b69-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="78b69-108">Di bawah **semua perangkat**, pilih perangkat yang ingin Anda gunakan untuk memulai sesi jarak jauh.</span><span class="sxs-lookup"><span data-stu-id="78b69-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="78b69-109">Dari **... Lebih lanjut**, pilih **sesi bantuan jarak jauh baru**.</span><span class="sxs-lookup"><span data-stu-id="78b69-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="78b69-110">Pilih **ya** untuk mengetahui bahwa Anda ingin membuat sesi jarak jauh.</span><span class="sxs-lookup"><span data-stu-id="78b69-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="78b69-111">Setelah permintaan "memulai sesi remote baru" diakui oleh layanan TeamViewer, Anda akan melihat opsi untuk **memulai bantuan jarak jauh** di bawah detail panel Ikhtisar (atau, penting) untuk perangkat.</span><span class="sxs-lookup"><span data-stu-id="78b69-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="78b69-112">Pilih **Lihat lebih** untuk memperluas panel dan menampilkan status bantuan jarak jauh.</span><span class="sxs-lookup"><span data-stu-id="78b69-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="78b69-113">Pilih **mulai sesi jarak jauh** untuk memulai sesi di sisi admin.</span><span class="sxs-lookup"><span data-stu-id="78b69-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="78b69-114">Pilih untuk mengunduh biner TeamViewer (Windows), dan pilih **Jalankan**.</span><span class="sxs-lookup"><span data-stu-id="78b69-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="78b69-115">**Catatan** Anda dapat mengabaikan halaman web browser yang dibuka ke situs web TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="78b69-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="78b69-116">Akui permintaan Aplikasi TeamViewer untuk melakukan perubahan pada perangkat (khusus Windows).</span><span class="sxs-lookup"><span data-stu-id="78b69-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="78b69-117">Aplikasi TeamViewer dimulai dan mencakup kode sesi untuk mengotentikasi koneksi dengan perangkat remote.</span><span class="sxs-lookup"><span data-stu-id="78b69-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="78b69-118">**Bagian 2: pada perangkat yang ditargetkan untuk sesi jarak jauh**</span><span class="sxs-lookup"><span data-stu-id="78b69-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="78b69-119">Buka portal perusahaan Intune.</span><span class="sxs-lookup"><span data-stu-id="78b69-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="78b69-120">Cari bendera pemberitahuan: "administrator TI Anda meminta kontrol perangkat ini untuk sesi bantuan jarak jauh," dan pilih pemberitahuan.</span><span class="sxs-lookup"><span data-stu-id="78b69-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="78b69-121">Pilih untuk mengunduh aplikasi TeamViewer, atau Akui download aplikasi TeamViewer dari App Store, lalu pilih **Run**.</span><span class="sxs-lookup"><span data-stu-id="78b69-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="78b69-122">**Catatan** Anda dapat mengabaikan halaman web browser yang dibuka ke situs web TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="78b69-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="78b69-123">Akui permintaan Aplikasi TeamViewer untuk melakukan perubahan pada perangkat (khusus Windows).</span><span class="sxs-lookup"><span data-stu-id="78b69-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="78b69-124">Aplikasi TeamViewer dimulai dan mencakup kode sesi untuk mengotentikasi koneksi dengan perangkat remote.</span><span class="sxs-lookup"><span data-stu-id="78b69-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="78b69-125">Popup bertanya apakah Anda ingin mengizinkan sesi untuk memulai.</span><span class="sxs-lookup"><span data-stu-id="78b69-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="78b69-126">**Catatan** Kode sesi yang dihasilkan oleh layanan TeamViewer hanya digunakan satu kali.</span><span class="sxs-lookup"><span data-stu-id="78b69-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="78b69-127">Jika sambungan terputus, Anda harus:</span><span class="sxs-lookup"><span data-stu-id="78b69-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="78b69-128">Tutup instance aplikasi TeamViewer di perangkat remote dan di Stasiun kerja admin.</span><span class="sxs-lookup"><span data-stu-id="78b69-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="78b69-129">Tutup portal perusahaan pada perangkat jauh.</span><span class="sxs-lookup"><span data-stu-id="78b69-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="78b69-130">Memulai baru "sesi bantuan remote baru" dari admin portal.</span><span class="sxs-lookup"><span data-stu-id="78b69-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="78b69-131">Membuka kembali portal perusahaan pada perangkat jauh untuk menerima pemberitahuan baru.</span><span class="sxs-lookup"><span data-stu-id="78b69-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="78b69-132">Unduh dan buka Aplikasi TeamViewer pada perangkat remote dan workstation admin, seperti sebelumnya.</span><span class="sxs-lookup"><span data-stu-id="78b69-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>