---
title: Mengelola daftar alamat global dan buku alamat offline organisasi
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: c6ad2fcb85ef68c42cea11ebe0d1564e957b4720
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51794835"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="cc899-102">Mengelola daftar alamat global (GAL) dan buku alamat offline (OAB) organisasi</span><span class="sxs-lookup"><span data-stu-id="cc899-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="cc899-103">Daftar alamat global (GAL) adalah daftar objek yang didukung email (semua tipe penerima yang dapat menerima email) dalam organisasi.</span><span class="sxs-lookup"><span data-stu-id="cc899-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="cc899-104">Satu GAL dibuat secara otomatis di setiap organisasi.</span><span class="sxs-lookup"><span data-stu-id="cc899-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="cc899-105">Anda dapat membuat GAL tambahan untuk memisahkan pengguna berdasarkan organisasi atau lokasi, tetapi satu pengguna hanya dapat melihat dan menggunakan satu GAL pada satu waktu.</span><span class="sxs-lookup"><span data-stu-id="cc899-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="cc899-106">Beberapa klien email, seperti Outlook untuk Windows, mengunduh GAL untuk penggunaan offline.</span><span class="sxs-lookup"><span data-stu-id="cc899-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="cc899-107">Hal ini dikenal dengan buku alamat offline (OAB).</span><span class="sxs-lookup"><span data-stu-id="cc899-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="cc899-108">Di Exchange online, OAB hanya diperbarui satu kali setiap 8 jam, lalu klien harus mengunduhnya untuk memperbarui salinan OAB lokal.</span><span class="sxs-lookup"><span data-stu-id="cc899-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="cc899-109">Setiap perubahan penerima harus terlihat di GAL terlebih dahulu sebelum nantinya muncul di OAB.</span><span class="sxs-lookup"><span data-stu-id="cc899-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="cc899-110">Berikut adalah beberapa prosedur GAL dan OAB yang paling banyak digunakan:</span><span class="sxs-lookup"><span data-stu-id="cc899-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="cc899-111">Karena berbagai alasan, Anda mungkin ingin agar beberapa objek disembunyikan dari GAL.</span><span class="sxs-lookup"><span data-stu-id="cc899-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="cc899-112">Silakan lihat [Menyembunyikan penerima dari daftar alamat](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="cc899-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="cc899-113">Jika Anda perlu memberikan tampilan terkustomisasi GAL organisasi kepada grup pengguna tertentu, lihat [Kebijakan buku alamat di Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="cc899-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="cc899-114">[Membuat daftar alamat global di Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) dan untuk mempelajari cara bekerja dengan izin GAL, lihat [Daftar alamat di Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="cc899-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="cc899-115">Perhatikan bahwa jika Anda membuat GAL baru, Anda mungkin juga ingin membuat OAB baru.</span><span class="sxs-lookup"><span data-stu-id="cc899-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="cc899-116">Lihat [Prosedur buku alamat offline](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="cc899-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
