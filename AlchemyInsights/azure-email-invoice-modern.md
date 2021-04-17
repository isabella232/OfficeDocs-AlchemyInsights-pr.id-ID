---
title: Faktur email Azure modern
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
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: id-ID
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820829"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="ebcfd-102">Faktur email di Azure</span><span class="sxs-lookup"><span data-stu-id="ebcfd-102">Email invoicing in Azure</span></span>

<span data-ttu-id="ebcfd-103">Anda harus memiliki peran pemilik atau kontributor di profil tagihan atau akun tagihannya untuk memperbarui preferensi faktur email.</span><span class="sxs-lookup"><span data-stu-id="ebcfd-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="ebcfd-104">Setelah memilih ikut, semua pengguna dengan peran pemilik, kontributor, pembaca, dan manajer faktur di profil tagihan akan mendapatkan faktur dalam email.</span><span class="sxs-lookup"><span data-stu-id="ebcfd-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="ebcfd-105">Masuk ke [portal Microsoft Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="ebcfd-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="ebcfd-106">Cari **Manajemen Biaya + Tagihan**.</span><span class="sxs-lookup"><span data-stu-id="ebcfd-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="ebcfd-107">Pilih **Faktur** dari sisi kiri, lalu pilih **Faktur Email** dari bagian atas halaman.</span><span class="sxs-lookup"><span data-stu-id="ebcfd-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="ebcfd-108">Jika memiliki beberapa profil tagihan, pilih sebuah profil tagihan, lalu pilih **Ikut**.</span><span class="sxs-lookup"><span data-stu-id="ebcfd-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="ebcfd-109">Pilih **Perbarui**.</span><span class="sxs-lookup"><span data-stu-id="ebcfd-109">Select **Update**.</span></span>
6. <span data-ttu-id="ebcfd-110">Jika memiliki beberapa profil tagihan, pilih sebuah profil tagihan, lalu pilih **Ikut**.</span><span class="sxs-lookup"><span data-stu-id="ebcfd-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="ebcfd-111">Anda memberi orang lain akses untuk melihat, mengunduh, dan membayar faktur dengan menetapkan peran manajer faktur kepada mereka untuk profil tagihan MCA atau MPA.</span><span class="sxs-lookup"><span data-stu-id="ebcfd-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="ebcfd-112">Jika Anda memilih mendapatkan faktur dalam email, pengguna juga akan mendapatkan faktur dalam email.</span><span class="sxs-lookup"><span data-stu-id="ebcfd-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="ebcfd-113">Masuk ke [portal Microsoft Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="ebcfd-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="ebcfd-114">Cari **Manajemen Biaya + Tagihan**.</span><span class="sxs-lookup"><span data-stu-id="ebcfd-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="ebcfd-115">Pilih **Profil tagihan** dari sisi kiri.</span><span class="sxs-lookup"><span data-stu-id="ebcfd-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="ebcfd-116">Dari daftar profil tagihan, pilih profil tagihan yang ingin ditetapkan peran manajer faktur.</span><span class="sxs-lookup"><span data-stu-id="ebcfd-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="ebcfd-117">Pilih **Kontrol Akses (IAM)** dari sisi kiri, lalu pilih **Tambahkan** dari bagian atas halaman.</span><span class="sxs-lookup"><span data-stu-id="ebcfd-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="ebcfd-118">Di daftar menurun Peran, pilih **Manajer Faktur**.</span><span class="sxs-lookup"><span data-stu-id="ebcfd-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="ebcfd-119">Masukkan alamat email pengguna untuk memberikan akses.</span><span class="sxs-lookup"><span data-stu-id="ebcfd-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="ebcfd-120">Pilih **Simpan** untuk menetapkan peran.</span><span class="sxs-lookup"><span data-stu-id="ebcfd-120">Select **Save** to assign the role.</span></span>
