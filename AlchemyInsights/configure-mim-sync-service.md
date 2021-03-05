---
title: Mengonfigurasi Layanan Sinkronisasi MIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: id-ID
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481872"
---
# <a name="configure-mim-sync-service"></a><span data-ttu-id="956c2-102">Mengonfigurasi Layanan Sinkronisasi MIM</span><span class="sxs-lookup"><span data-stu-id="956c2-102">Configure MIM Sync service</span></span>

<span data-ttu-id="956c2-103">Layanan Sinkronisasi Microsoft Identity Manager (MIM) adalah komponen MIM.</span><span class="sxs-lookup"><span data-stu-id="956c2-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="956c2-104">Ini adalah layanan terpusat di tempat yang menyimpan dan mengintegrasikan informasi untuk organisasi yang memiliki beberapa direktori dan database di tempat.</span><span class="sxs-lookup"><span data-stu-id="956c2-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="956c2-105">Anda mungkin dapat mengatasi masalah dengan sinkronisasi MIM jika masalah telah diatasi dalam pembaruan terbaru untuk MIM atau merupakan salah satu masalah lain yang disebutkan di bawah ini.</span><span class="sxs-lookup"><span data-stu-id="956c2-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="956c2-106">**Langkah yang direkomendasikan**</span><span class="sxs-lookup"><span data-stu-id="956c2-106">**Recommended steps**</span></span>

1. <span data-ttu-id="956c2-107">Pastikan bahwa Anda menggunakan pembaruan terbaru MIM Sync dan periksa [catatan rilis MIM Sync](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) untuk menentukan apakah masalah telah diatasi dalam pembaruan.</span><span class="sxs-lookup"><span data-stu-id="956c2-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="956c2-108">Jika masalahnya dengan generik LDAP, Generic SQL, Lotus Domino atau Web Services Connector, pastikan bahwa Anda menggunakan pembaruan terbaru dari [konektor generik](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span><span class="sxs-lookup"><span data-stu-id="956c2-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="956c2-109">Jika MIM Sync-Run berhenti dengan kesalahan, lihat tabel [kode kesalahan Jalankan](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) untuk menentukan penyebab potensial.</span><span class="sxs-lookup"><span data-stu-id="956c2-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="956c2-110">Jika Jalankan perhentian dengan **ekstensi-dll-pengecualian**, lalu klik kata tersebut untuk membuka jendela **properti objek Ruang konektor** , dan klik pada **pelacakan stack...** untuk melihat informasi selengkapnya tentang penyebab utama, seperti yang diuraikan dalam [ekstensi-dll-pengecualian](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span><span class="sxs-lookup"><span data-stu-id="956c2-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="956c2-111">Jika komponen Layanan pemberitahuan Ubah kata sandi (PCNS) melaporkan **kesalahan 6025** dalam log kejadian selama sinkronisasi kata sandi, lihat panduan pemecahan masalah [pelaporan pcns kesalahan 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span><span class="sxs-lookup"><span data-stu-id="956c2-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="956c2-112">Jika sinkronisasi penuh dengan agen manajemen layanan FIM lambat, periksa pengaturan **otomatis tumbuh** untuk Code, seperti yang diuraikan dalam [pemecahan masalah sinkronisasi penuh Slow atau Hanging](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span><span class="sxs-lookup"><span data-stu-id="956c2-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="956c2-113">Jika Anda mengalami kesalahan server berhenti-dengan pembuatan yang gagal-melalui-Web-Services menggunakan agen manajemen layanan FIM, lihat [dukungan-Info: pembuatan gagal-melalui-web-layanan](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) untuk gambaran umum penyebab.</span><span class="sxs-lookup"><span data-stu-id="956c2-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

