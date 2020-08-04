---
title: Masalah menggunakan konsol admin Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555384"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="b37d3-102">Masalah menggunakan konsol admin Intune</span><span class="sxs-lookup"><span data-stu-id="b37d3-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="b37d3-103">**"Akses ditolak" saat menavigasi portal admin Intune.**</span><span class="sxs-lookup"><span data-stu-id="b37d3-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="b37d3-104">Jika Anda adalah anggota dari peran kustom Intune, pastikan bahwa Intune atau Enterprise Mobility Suite (EMS) lisensi ditetapkan ke akun Anda.</span><span class="sxs-lookup"><span data-stu-id="b37d3-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="b37d3-105">Jika Anda menggunakan Manajer konfigurasi untuk mengelola perangkat, verifikasi Anda bukan bagian dari koleksi pengguna Intune untuk manajer konfigurasi MDM.</span><span class="sxs-lookup"><span data-stu-id="b37d3-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="b37d3-106">Verifikasi bahwa Anda telah ditetapkan sesuai peran berbasis administrasi kontrol (RBAC) izin dalam bilah peran Intune.</span><span class="sxs-lookup"><span data-stu-id="b37d3-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="b37d3-107">Verifikasi grup yang digunakan bukanlah daftar distribusi.</span><span class="sxs-lookup"><span data-stu-id="b37d3-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="b37d3-108">Intune di portal Azure hanya mendukung akun pengguna yang menjadi bagian dari grup keamanan Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b37d3-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="b37d3-109">Tinjau grup Anda di Azure portal > **Intune**  >  **grup**, atau Azure portal > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="b37d3-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="b37d3-110">**Pengguna memiliki terlalu banyak izin untuk ditetapkan Intune peran**</span><span class="sxs-lookup"><span data-stu-id="b37d3-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="b37d3-111">Menyarankan pengguna untuk pergi ke **Intune**  >  **Intune peran**  >  **izin saya**  >  **ekspor** untuk meninjau diberikan izin.</span><span class="sxs-lookup"><span data-stu-id="b37d3-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="b37d3-112">**Saya menambahkan grup lingkup ke peran, namun pengguna dalam peran tersebut masih melihat pengguna atau perangkat lain.**</span><span class="sxs-lookup"><span data-stu-id="b37d3-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="b37d3-113">Grup lingkup tidak menyaring pengguna atau perangkat.</span><span class="sxs-lookup"><span data-stu-id="b37d3-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="b37d3-114">Kelompok lingkup:</span><span class="sxs-lookup"><span data-stu-id="b37d3-114">Scope groups:</span></span>

- <span data-ttu-id="b37d3-115">Batasi pengguna yang dapat menetapkan kebijakan atau aplikasi.</span><span class="sxs-lookup"><span data-stu-id="b37d3-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="b37d3-116">Izinkan hanya pengguna tertentu untuk menjalankan tugas jarak jauh di perangkat.</span><span class="sxs-lookup"><span data-stu-id="b37d3-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="b37d3-117">Untuk informasi selengkapnya tentang grup lingkup, lihat [kontrol akses berbasis peran (RBAC) dengan Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="b37d3-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="b37d3-118">**Saya menambahkan pengguna ke peran Intune tetapi mereka masih memiliki akses penuh ke konsol admin Intune.**</span><span class="sxs-lookup"><span data-stu-id="b37d3-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="b37d3-119">Arahkan ke Intune > **pengguna** di Azure portal dan verifikasi bahwa pengguna tidak ditetapkan ke salah satu peran berikut ini di Azure Portal:</span><span class="sxs-lookup"><span data-stu-id="b37d3-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="b37d3-120">Administrator global</span><span class="sxs-lookup"><span data-stu-id="b37d3-120">Global administrator</span></span>
- <span data-ttu-id="b37d3-121">Intune Layanan administrator</span><span class="sxs-lookup"><span data-stu-id="b37d3-121">Intune service administrator</span></span>
- <span data-ttu-id="b37d3-122">Administrator SharePoint</span><span class="sxs-lookup"><span data-stu-id="b37d3-122">SharePoint administrator</span></span>

<span data-ttu-id="b37d3-123">Untuk informasi lebih lanjut, lihat [kontrol akses berbasis peran (RBAC) dengan Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="b37d3-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="b37d3-124">**Masalah akses**</span><span class="sxs-lookup"><span data-stu-id="b37d3-124">**Access Issues**</span></span>

<span data-ttu-id="b37d3-125">Untuk informasi lebih lanjut, lihat [Anda tidak dapat masuk ke Office 365, Azure, atau Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="b37d3-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>