---
title: Cara menambahkan atau menghapus delegasi di Outlook untuk Windows
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
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573579"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="cb735-102">Cara menambahkan atau menghapus delegasi di Outlook untuk Windows</span><span class="sxs-lookup"><span data-stu-id="cb735-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="cb735-103">Untuk menambahkan delegasi di Outlook untuk Windows:</span><span class="sxs-lookup"><span data-stu-id="cb735-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="cb735-104">Klik tab **file** yang diikuti dengan **pengaturan akun**, lalu pilih **akses delegasi**.</span><span class="sxs-lookup"><span data-stu-id="cb735-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="cb735-105">Klik **Tambahkan**.</span><span class="sxs-lookup"><span data-stu-id="cb735-105">Click on **Add**.</span></span> <span data-ttu-id="cb735-106">Jika **Add** tidak muncul, koneksi aktif mungkin tidak ada antara Outlook dan Exchange.</span><span class="sxs-lookup"><span data-stu-id="cb735-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="cb735-107">Bilah status Outlook menampilkan status koneksi.</span><span class="sxs-lookup"><span data-stu-id="cb735-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="cb735-108">Ketikkan nama orang yang ingin Anda tetapkan sebagai delegasi Anda, atau Cari dan pilih nama dalam daftar hasil pencarian.</span><span class="sxs-lookup"><span data-stu-id="cb735-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="cb735-109">Delegasi harus merupakan orang di daftar alamat global (GAL) organisasi Anda.</span><span class="sxs-lookup"><span data-stu-id="cb735-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="cb735-110">Klik **Tambahkan** diikuti dengan **OK**.</span><span class="sxs-lookup"><span data-stu-id="cb735-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="cb735-111">Dalam kotak dialog **izin delegasi** , terima pengaturan izin default atau pilih tingkat akses kustom untuk folder Exchange.</span><span class="sxs-lookup"><span data-stu-id="cb735-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="cb735-112">Jika delegasi memerlukan izin untuk bekerja hanya dengan permintaan dan respons Rapat, pengaturan izin default seperti **delegasi menerima salinan pesan terkait Rapat yang dikirimkan kepada saya** sudah cukup.</span><span class="sxs-lookup"><span data-stu-id="cb735-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="cb735-113">Anda dapat membiarkan pengaturan izin **kotak masuk** **tidak ada**.</span><span class="sxs-lookup"><span data-stu-id="cb735-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="cb735-114">Permintaan dan respons Rapat akan langsung masuk ke kotak masuk delegasi.</span><span class="sxs-lookup"><span data-stu-id="cb735-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="cb735-115">Secara default, delegasi diberikan izin **editor (dapat membaca, membuat, dan mengubah item)** ke folder **kalender** Anda.</span><span class="sxs-lookup"><span data-stu-id="cb735-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="cb735-116">Saat delegasi merespons ke Rapat atas nama Anda, delegasi tersebut secara otomatis ditambahkan ke folder **kalender** Anda.</span><span class="sxs-lookup"><span data-stu-id="cb735-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="cb735-117">Untuk mengirim pesan untuk memberi tahu delegasi izin yang diubah, pilih kotak centang **secara otomatis mengirim pesan untuk mendelegasikan ringkasan izin ini** .</span><span class="sxs-lookup"><span data-stu-id="cb735-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="cb735-118">Jika Anda ingin, pilih kotak centang **delegasi dapat melihat item pribadi saya** .</span><span class="sxs-lookup"><span data-stu-id="cb735-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="cb735-119">Pengaturan ini mempengaruhi semua folder Exchange.</span><span class="sxs-lookup"><span data-stu-id="cb735-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="cb735-120">Ini mencakup semua email, kontak, kalender, tugas, catatan, dan folder jurnal.</span><span class="sxs-lookup"><span data-stu-id="cb735-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="cb735-121">Tidak ada cara untuk memberi akses ke item pribadi dalam folder tertentu saja.</span><span class="sxs-lookup"><span data-stu-id="cb735-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="cb735-122">Pilih **OK**.</span><span class="sxs-lookup"><span data-stu-id="cb735-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="cb735-123">Pesan yang dikirim dengan izin Kirim atas nama menyertakan delegasi dan nama Anda di samping **dari**.</span><span class="sxs-lookup"><span data-stu-id="cb735-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="cb735-124">Saat pesan dikirim dengan izin Kirim sebagai, hanya nama Anda yang muncul.</span><span class="sxs-lookup"><span data-stu-id="cb735-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="cb735-125">Setelah Anda menambahkan seseorang sebagai delegasi, mereka bisa menambahkan kotak surat Exchange Anda ke profil Outlook mereka.</span><span class="sxs-lookup"><span data-stu-id="cb735-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="cb735-126">Untuk instruksi, lihat [mengelola email dan item kalender orang lain](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span><span class="sxs-lookup"><span data-stu-id="cb735-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="cb735-127">Untuk menghapus delegasi di Outlook untuk Windows:</span><span class="sxs-lookup"><span data-stu-id="cb735-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="cb735-128">Klik tab **file** .</span><span class="sxs-lookup"><span data-stu-id="cb735-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="cb735-129">Klik **pengaturan akun** yang diikuti oleh **akses delegasi**.</span><span class="sxs-lookup"><span data-stu-id="cb735-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="cb735-130">Pilih nama delegasi yang ingin Anda ubah izinnya, lalu klik **Hapus** diikuti dengan **OK**.</span><span class="sxs-lookup"><span data-stu-id="cb735-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
