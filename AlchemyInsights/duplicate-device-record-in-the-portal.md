---
title: Dupliker enhedspost i-portalen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789683"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="cac42-102">Dupliker enhedspost i-portalen</span><span class="sxs-lookup"><span data-stu-id="cac42-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="cac42-103">Du kan få vist 2 poster for en enhed i-portalen, hvis enheden ikke korrekt rapporterer status for fælles administration på Konfigurationsstyringswebstedet.</span><span class="sxs-lookup"><span data-stu-id="cac42-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="cac42-104">Hvis du vil kontrollere en enheds administrationsstatus, skal du gennemse kolonnen **Fælles administreret** for enheden i Konfigurationsstyringskonsollen.</span><span class="sxs-lookup"><span data-stu-id="cac42-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="cac42-105">Hvis kolonnen ikke er synlig, kan du tilføje den ved at højreklikke på en af kolonneoverskrifterne og markere den på listen.</span><span class="sxs-lookup"><span data-stu-id="cac42-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="cac42-106">Den fællesadministrerede værdi skal være **Ja**..</span><span class="sxs-lookup"><span data-stu-id="cac42-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="cac42-107">Hvis værdien er **Nej**, skal du åbne Konfigurationsstyring-klient-applet på klientenheden og markere egenskaben **Fælles administration** på Generel-fanen.</span><span class="sxs-lookup"><span data-stu-id="cac42-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="cac42-108">Hvis værdien er **Aktiveret**, indikerer dette, at der er problemer med klientkommunikationen med Administrationspunktet.</span><span class="sxs-lookup"><span data-stu-id="cac42-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="cac42-109">Gennemse **CcmMessaging.log** på enheden for at undersøge potentielle forbindelsesproblemer.</span><span class="sxs-lookup"><span data-stu-id="cac42-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="cac42-110">Hvis værdien er Deaktiveret og enheden er tilmeldt i Intune, skal du sørge for, at enheden har modtaget politikken for fælles administration, ved at gennemgå **CoManagementHandler.log** på enheden.</span><span class="sxs-lookup"><span data-stu-id="cac42-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
