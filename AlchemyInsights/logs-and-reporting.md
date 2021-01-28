---
title: Logfiler og rapportering
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035861"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="08a9f-102">Logfiler og rapportering</span><span class="sxs-lookup"><span data-stu-id="08a9f-102">Logs and Reporting</span></span>

<span data-ttu-id="08a9f-103">[Ofte stillede spørgsmål om Azure Active Directory-rapportering](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) besvarer ofte stillede spørgsmål om Azure Active Directory-rapportering (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="08a9f-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="08a9f-104">Du kan finde flere oplysninger i [Azure Active Directory-rapportering.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)</span><span class="sxs-lookup"><span data-stu-id="08a9f-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="08a9f-105">**Fejlfinding af problemer med Overvågning**</span><span class="sxs-lookup"><span data-stu-id="08a9f-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="08a9f-106">Hvis du har problemer med at se nogle overvågningsaktiviteter, og den manglende aktivitet er på [denne liste,](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)skal du indsende en supportanmodning.</span><span class="sxs-lookup"><span data-stu-id="08a9f-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="08a9f-107">Hvis du har problemer med at se overvågningslogfiler i din lejer, skal du indsende en supportanmodning.</span><span class="sxs-lookup"><span data-stu-id="08a9f-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="08a9f-108">Hvis dine overvågningsaktiviteter ikke vises med det samme [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) i Azure-portalen, kan du se vores oplysninger om ventetid og arkivere en supportanmodning, hvis forsinkelsen overstiger den dokumenterede ventetid.</span><span class="sxs-lookup"><span data-stu-id="08a9f-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="08a9f-109">Opbevaring af Azure AD-aktivitetslogfiler</span><span class="sxs-lookup"><span data-stu-id="08a9f-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="08a9f-110">Hvis du ikke kan se hele overvågning for det datointerval, du har valgt, kan du hente op til 250.000 rækker (sorteret efter nyeste) af logons fra Azure-portalen.</span><span class="sxs-lookup"><span data-stu-id="08a9f-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="08a9f-111">Du kan finde flere oplysninger under [Overførsel af overvågningsaktiviteter.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)</span><span class="sxs-lookup"><span data-stu-id="08a9f-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="08a9f-112">**Fejlfinding af problemer med logon**</span><span class="sxs-lookup"><span data-stu-id="08a9f-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="08a9f-113">Du kan kun se de seneste 30 dages data, hvis du har en Azure AD Premium-licens (P1 eller P2) til din lejer.</span><span class="sxs-lookup"><span data-stu-id="08a9f-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="08a9f-114">Logon er kun tilgængelige for Azure AD Premium-lejere.</span><span class="sxs-lookup"><span data-stu-id="08a9f-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="08a9f-115">Den er ikke tilgængelig for gratis lejere eller basislicenserede lejere.</span><span class="sxs-lookup"><span data-stu-id="08a9f-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="08a9f-116">Hvis din lejer har en Premium P1-licens, og du ikke [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) kan se logons, kan du se vores oplysninger om ventetid og arkivere en supportbillet, hvis forsinkelsen overstiger den dokumenterede ventetid.</span><span class="sxs-lookup"><span data-stu-id="08a9f-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="08a9f-117">Hvis du ikke kan se alle logons for det datointerval, du har valgt, skal du bemærke, at du kan hente op til 250.000 rækker (sorteret efter nyeste) af logons fra Azure-portalen.</span><span class="sxs-lookup"><span data-stu-id="08a9f-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="08a9f-118">Du kan finde flere oplysninger [under download af logonaktiviteter.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)</span><span class="sxs-lookup"><span data-stu-id="08a9f-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="08a9f-119">**Fejlfinding af sikkerhedsrapporter (brugere, der er markeret med risiko, risikabelt logon)**</span><span class="sxs-lookup"><span data-stu-id="08a9f-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="08a9f-120">Brugere, der er markeret med flag til rapport om risikosikkerhed</span><span class="sxs-lookup"><span data-stu-id="08a9f-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="08a9f-121">Risikabel logonrapport i Azure Active Directory-portalen</span><span class="sxs-lookup"><span data-stu-id="08a9f-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="08a9f-122">Azure Active Directory-risikohændelser</span><span class="sxs-lookup"><span data-stu-id="08a9f-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
