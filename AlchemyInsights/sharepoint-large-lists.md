---
title: Daftar besar SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720136"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="0b8e7-102">Bekerja dengan daftar dan pustaka yang besar di SharePoint</span><span class="sxs-lookup"><span data-stu-id="0b8e7-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="0b8e7-103">Daftar dan pustaka SharePoint dapat berisi hingga 30.000.000 item, tetapi ketika mereka memiliki lebih dari 5.000 item, Anda mungkin melihat kesalahan ambang tampilan daftar ketika Anda mencoba bekerja dengan mereka.</span><span class="sxs-lookup"><span data-stu-id="0b8e7-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="0b8e7-104">Ambang batas ini ada untuk mempertahankan kinerja layanan.</span><span class="sxs-lookup"><span data-stu-id="0b8e7-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="0b8e7-105">Ambang batas ini tidak dapat diubah.</span><span class="sxs-lookup"><span data-stu-id="0b8e7-105">It can't be changed.</span></span> <span data-ttu-id="0b8e7-106">Untuk menghindari memukul ambang batas ini:</span><span class="sxs-lookup"><span data-stu-id="0b8e7-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="0b8e7-107">**Gunakan modern**</span><span class="sxs-lookup"><span data-stu-id="0b8e7-107">**Use modern**</span></span>

<span data-ttu-id="0b8e7-108">Tampilan yang memperlihatkan banyak item bekerja paling baik dalam pengalaman modern.</span><span class="sxs-lookup"><span data-stu-id="0b8e7-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="0b8e7-109">[Gunakan pengalaman modern](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) untuk menghindari kesalahan yang mungkin Anda lihat dalam pengalaman klasik.</span><span class="sxs-lookup"><span data-stu-id="0b8e7-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="0b8e7-110">**Menambahkan indeks**</span><span class="sxs-lookup"><span data-stu-id="0b8e7-110">**Add indexes**</span></span>

<span data-ttu-id="0b8e7-111">Saat Anda memfilter atau mengurutkan menurut kolom yang tidak memiliki indeks, Anda mungkin melihat pesan kesalahan.</span><span class="sxs-lookup"><span data-stu-id="0b8e7-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="0b8e7-112">[Tambahkan indeks](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) secara manual dari **pengaturan daftar** di menu pengaturan, lalu **kolom terindeks**.</span><span class="sxs-lookup"><span data-stu-id="0b8e7-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="0b8e7-113">**Mengedit tampilan daftar**</span><span class="sxs-lookup"><span data-stu-id="0b8e7-113">**Edit the list view**</span></span>

<span data-ttu-id="0b8e7-114">Jika terjadi kesalahan saat bekerja dengan daftar besar, [Edit tampilan daftar Anda](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="0b8e7-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="0b8e7-115">Empat perubahan berikut ini akan menghapus kesalahan ambang tampilan daftar.</span><span class="sxs-lookup"><span data-stu-id="0b8e7-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="0b8e7-116">Buat keempat perubahan untuk menghapus semua kesalahan.</span><span class="sxs-lookup"><span data-stu-id="0b8e7-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="0b8e7-117">Jika Anda masih mengalami kesalahan, lihat [mengelola daftar dan pustaka yang besar](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="0b8e7-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="0b8e7-118">Pilih **tidak ada** dari kedua **urutan pertama menurut kolom** lalu **Urutkan menurut kolom**.</span><span class="sxs-lookup"><span data-stu-id="0b8e7-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="0b8e7-119">Pilih **tidak ada** dari **grup pertama menurut kolom,** **lalu Kelompokkan menurut kolom**.</span><span class="sxs-lookup"><span data-stu-id="0b8e7-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="0b8e7-120">Pilih **tidak ada** untuk semua kolom di bagian **Total** .</span><span class="sxs-lookup"><span data-stu-id="0b8e7-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="0b8e7-121">Batalkan pilihan semua kecuali satu kolom untuk ditampilkan dari bagian **kolom** .</span><span class="sxs-lookup"><span data-stu-id="0b8e7-121">Deselect all but one column for display from the **Columns** section.</span></span>

