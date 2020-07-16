---
title: Memecahkan masalah pemuatan gambar di Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148290"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="71aba-102">Memecahkan masalah pemuatan gambar di Yammer</span><span class="sxs-lookup"><span data-stu-id="71aba-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="71aba-103">Ketika masalah terjadi dengan foto dan file preview di heboh, memecahkan masalah dengan memeriksa apakah masalah ini terjadi untuk semua pengguna, apakah itu terjadi pada perangkat mobile, dan jika dapat direproduksi ketika meng-upload lampiran.</span><span class="sxs-lookup"><span data-stu-id="71aba-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="71aba-104">**Masalah foto profil**</span><span class="sxs-lookup"><span data-stu-id="71aba-104">**Profile photo issues**</span></span>  

<span data-ttu-id="71aba-105">Jika pengguna akhir masuk ke heboh melalui Microsoft 365, mereka harus mengubah profil mereka, termasuk foto profil mereka.</span><span class="sxs-lookup"><span data-stu-id="71aba-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="71aba-106">Jika pengguna tidak diizinkan untuk membuat pembaruan profil, admin dapat melakukan pembaruan untuk pengguna.</span><span class="sxs-lookup"><span data-stu-id="71aba-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="71aba-107">Untuk informasi lebih lanjut, lihat [Lihat dan perbarui profil Anda di Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="71aba-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="71aba-108">Untuk info tentang pengeditan profil, termasuk foto profil, lihat [mengubah profil dan pengaturan Yammer](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="71aba-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="71aba-109">Foto profil yang diperbarui disinkronkan secara berbeda dengan atribut profil.</span><span class="sxs-lookup"><span data-stu-id="71aba-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="71aba-110">Pengguna harus masuk untuk memulai sinkronisasi foto profil mereka.</span><span class="sxs-lookup"><span data-stu-id="71aba-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="71aba-111">Untuk info, lihat [adalah gambar profil pengguna yang diperbarui dari Office 365 ke Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span><span class="sxs-lookup"><span data-stu-id="71aba-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="71aba-112">Untuk info tentang siklus hidup pengguna untuk heboh, lihat [mengelola heboh pengguna di seluruh siklus hidup mereka dari Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span><span class="sxs-lookup"><span data-stu-id="71aba-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="71aba-113">Untuk rincian tentang bagaimana sinkronisasi gambar profil bekerja di Microsoft 365, lihat [informasi tentang sinkronisasi gambar profil di microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="71aba-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="71aba-114">**Pratinjau dokumen dan masalah thumbnail gambar**</span><span class="sxs-lookup"><span data-stu-id="71aba-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="71aba-115">Ketika berkas atau gambar yang dikirim ke Yammer, pratinjau mungkin tidak ditampilkan karena:</span><span class="sxs-lookup"><span data-stu-id="71aba-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="71aba-116">Berkas rusak dan tidak dapat diproses.</span><span class="sxs-lookup"><span data-stu-id="71aba-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="71aba-117">Berkas belum baru-baru ini diunggah ke SharePoint online, atau heboh memiliki metadata tidak valid untuk alasan lain.</span><span class="sxs-lookup"><span data-stu-id="71aba-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="71aba-118">URL yang diperlukan untuk memuat gambar pratinjau diblokir.</span><span class="sxs-lookup"><span data-stu-id="71aba-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="71aba-119">Pratinjau file dihapus oleh pengguna sebelum posting.</span><span class="sxs-lookup"><span data-stu-id="71aba-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="71aba-120">Masalah layanan dicegah pratinjau yang dihasilkan.</span><span class="sxs-lookup"><span data-stu-id="71aba-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="71aba-121">**Catatan** Pratinjau untuk tautan dan unggahan file mungkin berperilaku berbeda.</span><span class="sxs-lookup"><span data-stu-id="71aba-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="71aba-122">Link ke file di internet atau link yang memerlukan otentikasi tambahan mungkin tidak ditampilkan dengan benar.</span><span class="sxs-lookup"><span data-stu-id="71aba-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="71aba-123">Untuk informasi lebih lanjut, lihat [melampirkan file atau gambar ke pesan heboh](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span><span class="sxs-lookup"><span data-stu-id="71aba-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 