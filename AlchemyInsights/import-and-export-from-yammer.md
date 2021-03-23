---
title: Importér og eksportér fra Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035440"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="67a48-102">Importér og eksportér fra Yammer</span><span class="sxs-lookup"><span data-stu-id="67a48-102">Import and export from Yammer</span></span>

<span data-ttu-id="67a48-103">**Importér**</span><span class="sxs-lookup"><span data-stu-id="67a48-103">**Import**</span></span>

<span data-ttu-id="67a48-104">Indstillingerne for brugerimport varierer, afhængigt af Yammer dit netværk er i oprindelig [tilstand til Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)eller ej.</span><span class="sxs-lookup"><span data-stu-id="67a48-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="67a48-105">**Ikke-indbygget tilstand:** Brugere kan importeres til grupper ved hjælp af Tilføj fra adressekartotek [](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) [(grænse](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) til 100 brugere) i gruppeindstillinger eller til netværket ved hjælp af masseopdatering i netværksadministrator.</span><span class="sxs-lookup"><span data-stu-id="67a48-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="67a48-106">**Indbygget** tilstand: Gruppemedlemskab og netværksmedlemskabshandlinger skal udføres fra [Microsoft 365-administrationsportalen,](https://docs.microsoft.com/microsoft-365/admin/add-users) [Azure AD-portalen](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)eller ved hjælp af en anden Azure AD-indstilling.</span><span class="sxs-lookup"><span data-stu-id="67a48-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="67a48-107">Netværk i indbygget tilstand har ikke længere adgang til Masseopdatering og andre ældre funktioner.</span><span class="sxs-lookup"><span data-stu-id="67a48-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="67a48-108">Yammer aldrig har understøttet import af indhold fra netværksadministrator, selv når funktionen Dataeksport blev brugt i et andet netværk.</span><span class="sxs-lookup"><span data-stu-id="67a48-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="67a48-109">Indhold kan genopslås af partnerløsninger eller Yammer REST-API'er.</span><span class="sxs-lookup"><span data-stu-id="67a48-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="67a48-110">**Eksportér**</span><span class="sxs-lookup"><span data-stu-id="67a48-110">**Export**</span></span>

<span data-ttu-id="67a48-111">[Eksportér netværksdata i netværksadministrator](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) tillader eksport af indhold fra Yammer netværk, herunder meddelelser og filer.</span><span class="sxs-lookup"><span data-stu-id="67a48-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="67a48-112">Vedhæftede filer kan være meget store og medføre, at eksporter tager lang tid at gennemføre.</span><span class="sxs-lookup"><span data-stu-id="67a48-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="67a48-113">Vi anbefaler, at aktive netværk eksporteres ved hjælp af [dataeksport-API'en](https://developer.yammer.com/docs/data-export-api) i dele efter dag eller uge.</span><span class="sxs-lookup"><span data-stu-id="67a48-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="67a48-114">Microsoft Support leverer ikke brugerdefinerede scripts til dette formål.</span><span class="sxs-lookup"><span data-stu-id="67a48-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="67a48-115">Der findes [en separat GDPR-eksport](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) for at eksportere indhold til en enkelt bruger.</span><span class="sxs-lookup"><span data-stu-id="67a48-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>