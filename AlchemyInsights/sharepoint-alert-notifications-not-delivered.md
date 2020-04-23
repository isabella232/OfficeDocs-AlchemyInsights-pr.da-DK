---
title: Meddelelser om SharePoint-beskeder er ikke leveret
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: a422805d11a128909e1be7bf5d08b24efc132e23
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742041"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="00896-102">Meddelelser om SharePoint-beskeder er ikke leveret</span><span class="sxs-lookup"><span data-stu-id="00896-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="00896-103">Kontroller mappen UØNSKET mail i din mail, da der nogle gange kan gå advarsler derhen.</span><span class="sxs-lookup"><span data-stu-id="00896-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="00896-104">Find ud af, om **alle beskeder ikke leveres,** eller om **en individuel besked** fra en bestemt fil eller et bestemt bibliotek ikke leveres.</span><span class="sxs-lookup"><span data-stu-id="00896-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="00896-105">**Individuelle beskeder leveres ikke**: Hvis en individuel besked fra en bestemt fil eller et bestemt bibliotek ikke leveres, kan du forsøge at slette og genoprette den.</span><span class="sxs-lookup"><span data-stu-id="00896-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="00896-106">Se [Administrere, få vist eller slette SharePoint-beskeder](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) for at genoprette beskeden.</span><span class="sxs-lookup"><span data-stu-id="00896-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="00896-107">**Alle beskeder leveres ikke:** Hvis alle beskeder fra flere filer eller biblioteker ikke leveres, skal du gå til [dashboardet Tjenestetilstand](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) for at søge efter eventuelle meddelelser/hændelser, der kan forekomme med SharePoint eller Exchange.</span><span class="sxs-lookup"><span data-stu-id="00896-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="00896-108">Problemet kan være med SharePoint-beskedfunktionen eller forsinkelser i e-mails via Exchange.</span><span class="sxs-lookup"><span data-stu-id="00896-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="00896-109">Det vil også være vigtigt at bemærke, om andre e-mails bliver leveret, og hvis ikke, er problemet sandsynligvis med Forsinkelser i Exchange.</span><span class="sxs-lookup"><span data-stu-id="00896-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="00896-110">Ofte stillede spørgsmål om advarsler:</span><span class="sxs-lookup"><span data-stu-id="00896-110">FAQ on alerts:</span></span>

- <span data-ttu-id="00896-111">Det er ikke muligt at sende beskeder til distributionsgruppen, kun sikkerheds- og O365-grupper understøttes.</span><span class="sxs-lookup"><span data-stu-id="00896-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="00896-112">Du kan ikke tilpasse mailskabeloner til påmindelser. Du skal bruge Microsoft FLOW eller SharePoint Designer Workflow for at opnå disse.</span><span class="sxs-lookup"><span data-stu-id="00896-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

<span data-ttu-id="00896-113">Flere oplysninger:</span><span class="sxs-lookup"><span data-stu-id="00896-113">More Information:</span></span>

- <span data-ttu-id="00896-114">**Konfiguration af beskeder**: Du kan finde flere oplysninger om konfiguration af beskeder under [Oprette en besked for at få besked, når en fil eller mappe ændres i SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span><span class="sxs-lookup"><span data-stu-id="00896-114">**Alert setup**: For more information about setting up alerts, see [Create an alert to get notified when a file or folder changes in SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span></span>
- <span data-ttu-id="00896-115">**Fejlfinding af beskeder**: Du kan finde flere oplysninger om fejlfinding af advarsler under [Brugere modtager ikke Meddelelser om Beskeder om SharePoint Online](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span><span class="sxs-lookup"><span data-stu-id="00896-115">**Troubleshoot alerts**: For more information about troubleshooting alerts, see [Users don't receive SharePoint Online alert notifications](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span></span>
- <span data-ttu-id="00896-116">**Avancerede O365-politikker for overholdelse af regler og standarder**: Du kan finde flere oplysninger om konfiguration af disse påmindelser under Politikker for overholdelse af regler for overholdelse af regler for [overholdelse](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span><span class="sxs-lookup"><span data-stu-id="00896-116">**Advanced O365 Compliance Alert Policies**: For more information about setting up these alerts, see [Compliance Alert Policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span></span>
- <span data-ttu-id="00896-117">**SharePoint- og OneDrive-overvågningslogfiler**: Du kan finde flere oplysninger om, hvordan du henter disse hændelser, [under Søge i overvågningsloggen](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="00896-117">**SharePoint and OneDrive Audit Logs**: For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
- <span data-ttu-id="00896-118">**Beskeder, der sendes af Avanceret trusselsbeskyttelse:** Se [ATP for SharePoint og OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="00896-118">**Alerts sent by Advanced Threat Protection**: See [ATP for SharePoint and OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
- <span data-ttu-id="00896-119">**Advarsler sendt af datatab forebyggelse politikker**: Se [E-mail-meddelelser for DLP politikker](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="00896-119">**Alerts sent by Data Loss Prevention polices**: See [Email notifications for DLP policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

## <a name="related-topics"></a><span data-ttu-id="00896-120">Relaterede emner</span><span class="sxs-lookup"><span data-stu-id="00896-120">Related Topics</span></span>

<span data-ttu-id="00896-121">Vil du prøve Microsoft Flow i SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="00896-121">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="00896-122">Opret flow</span><span class="sxs-lookup"><span data-stu-id="00896-122">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="00896-123">SharePoint og Flow</span><span class="sxs-lookup"><span data-stu-id="00896-123">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
