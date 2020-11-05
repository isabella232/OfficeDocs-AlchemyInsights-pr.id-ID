---
title: Faktur email Azure modern
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922064"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="3daa1-102">Faktur email di Azure</span><span class="sxs-lookup"><span data-stu-id="3daa1-102">Email invoicing in Azure</span></span>

<span data-ttu-id="3daa1-103">Anda harus memiliki pemilik atau peran kontributor pada profil tagihan atau akun tagihan untuk memperbarui preferensi faktur email.</span><span class="sxs-lookup"><span data-stu-id="3daa1-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="3daa1-104">Setelah Anda memilih ikut, semua pengguna dengan pemilik, kontributor, pembaca, dan peran Manajer faktur pada profil tagihan akan menerima faktur di email.</span><span class="sxs-lookup"><span data-stu-id="3daa1-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="3daa1-105">Masuk ke [Azure portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="3daa1-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="3daa1-106">Cari **biaya manajemen + tagihan**.</span><span class="sxs-lookup"><span data-stu-id="3daa1-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="3daa1-107">Pilih **faktur** dari sisi kiri, lalu pilih **faktur email** dari bagian atas halaman.</span><span class="sxs-lookup"><span data-stu-id="3daa1-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="3daa1-108">Jika Anda memiliki beberapa profil tagihan, pilih profil tagihan lalu pilih pilih **masuk**.</span><span class="sxs-lookup"><span data-stu-id="3daa1-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="3daa1-109">Pilih **Perbarui**.</span><span class="sxs-lookup"><span data-stu-id="3daa1-109">Select **Update**.</span></span>
6. <span data-ttu-id="3daa1-110">Jika Anda memiliki beberapa profil tagihan, pilih profil tagihan lalu pilih pilih **masuk**.</span><span class="sxs-lookup"><span data-stu-id="3daa1-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="3daa1-111">Anda memberikan akses kepada orang lain untuk menampilkan, mengunduh, dan membayar faktur dengan menetapkan peran Manajer faktur untuk profil tagihan MCA atau MPA.</span><span class="sxs-lookup"><span data-stu-id="3daa1-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="3daa1-112">Jika Anda memilih untuk mendapatkan faktur Anda dalam email, pengguna juga mendapatkan faktur dalam email.</span><span class="sxs-lookup"><span data-stu-id="3daa1-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="3daa1-113">Masuk ke [Azure portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="3daa1-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="3daa1-114">Cari **biaya manajemen + tagihan**.</span><span class="sxs-lookup"><span data-stu-id="3daa1-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="3daa1-115">Pilih **profil tagihan** dari sisi kiri.</span><span class="sxs-lookup"><span data-stu-id="3daa1-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="3daa1-116">Dari daftar profil tagihan, pilih sebuah profil tagihan yang ingin Anda tetapkan peran Manajer faktur.</span><span class="sxs-lookup"><span data-stu-id="3daa1-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="3daa1-117">Pilih **kontrol akses (iam)** dari sisi kiri, lalu pilih **Tambahkan** dari bagian atas halaman.</span><span class="sxs-lookup"><span data-stu-id="3daa1-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="3daa1-118">Dalam daftar turun bawah peran, pilih **manajer faktur**.</span><span class="sxs-lookup"><span data-stu-id="3daa1-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="3daa1-119">Masukkan alamat email pengguna untuk memberi akses.</span><span class="sxs-lookup"><span data-stu-id="3daa1-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="3daa1-120">Pilih **Simpan** untuk menetapkan peran.</span><span class="sxs-lookup"><span data-stu-id="3daa1-120">Select **Save** to assign the role.</span></span>
