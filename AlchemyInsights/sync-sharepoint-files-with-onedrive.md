---
title: Memecahkan masalah “Buka dengan Explorer” di SharePoint Online
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/7/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: afee367e250357b20b77f0ea5dfe66d68967eb2a
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270711"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="09058-102">Memecahkan masalah “Buka dengan Explorer” di SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="09058-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="09058-103">Perintah Buka dengan Explorer akan membuka instans Windows Explorer lokal yang menampilkan struktur folder di server yang menghosting situs SharePoint.</span><span class="sxs-lookup"><span data-stu-id="09058-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="09058-104">Dengan kata lain, sebaiknya [sinkronkan file SharePoint dengan klien sinkronisasi OneDrive baru](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> yang menyediakan [File Sesuai Permintaan](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) karena layanan ini memberikan akses lokal ke file Anda dan menawarkan kinerja terbaik.</span><span class="sxs-lookup"><span data-stu-id="09058-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="09058-105">Jika memilih untuk menggunakan tampilan Explorer dan bukan menggunakan klien sinkronisasi OneDrive yang baru, pastikan Anda mengikuti langkah-langkah dan praktik terbaik dalam artikel di bawah ini:</span><span class="sxs-lookup"><span data-stu-id="09058-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="09058-106">Cara menggunakan perintah "Buka dengan Explorer" untuk menyelesaikan masalah di SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="09058-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- [<span data-ttu-id="09058-107">Menyalin atau memindahkan file pustaka menggunakan Buka dengan Explorer</span><span class="sxs-lookup"><span data-stu-id="09058-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> [!Note]  
> <span data-ttu-id="09058-108">Tombol **Buka dengan Explorer** tidak muncul dalam pengalaman pustaka yang baru.</span><span class="sxs-lookup"><span data-stu-id="09058-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="09058-109">Klik menu menurun **Tampilan** di bagian kanan atas (nama menu menurun berubah menurut tampilan Anda saat ini), lalu klik **Tampilkan di File Explorer**.</span><span class="sxs-lookup"><span data-stu-id="09058-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
>
 ><span data-ttu-id="09058-110">Buka dengan Explorer di SharePoint menggunakan kontrol ActiveX sehingga hanya didukung di Internet Explorer 10 atau 11.</span><span class="sxs-lookup"><span data-stu-id="09058-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="09058-111">Buka dengan Explorer tidak dapat digunakan di Windows dengan Microsoft Edge, Google Chrome, Mozilla Firefox, atau pada platform Mac.</span><span class="sxs-lookup"><span data-stu-id="09058-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="09058-112">Karena alasan ini, opsi Tampilan Explorer mungkin berwarna abu-abu.</span><span class="sxs-lookup"><span data-stu-id="09058-112">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
> - <span data-ttu-id="09058-113">[Mengapa tombol pita SharePoint tidak tersedia atau berwarna abu-abu](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span><span class="sxs-lookup"><span data-stu-id="09058-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

