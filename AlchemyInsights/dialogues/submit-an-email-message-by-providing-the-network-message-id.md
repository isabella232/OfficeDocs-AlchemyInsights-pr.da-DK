---
title: Sende en mail ved at angive netværksmeddelelses-id'et
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693163"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="bcc29-102">Sende en mail ved at angive netværksmeddelelses-id'et</span><span class="sxs-lookup"><span data-stu-id="bcc29-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="bcc29-103">Vælg **Mail- og** netværksmeddelelses-id  i pop **op-dialogboksen Ny indsendelse.**</span><span class="sxs-lookup"><span data-stu-id="bcc29-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="bcc29-104">Følg disse trin for at finde meddelelses-id'et for en mail i Outlook:</span><span class="sxs-lookup"><span data-stu-id="bcc29-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="bcc29-105">Dobbeltklik på mailen for at åbne den.</span><span class="sxs-lookup"><span data-stu-id="bcc29-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="bcc29-106">Vælg   >  **Filegenskaber.**</span><span class="sxs-lookup"><span data-stu-id="bcc29-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="bcc29-107">Åbn Notesblok eller et tomt Word-dokument, og kopiér og indsæt derefter det indhold, der findes i feltet Internetoverskrifter, i det åbne dokument for at gøre det mere synligt. </span><span class="sxs-lookup"><span data-stu-id="bcc29-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="bcc29-108">Find **feltet X-MS-Exchange-Organization-Network-Message-Id.**</span><span class="sxs-lookup"><span data-stu-id="bcc29-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="bcc29-109">Værdien efter: er **det** id, du skal bruge til indsendelsen.</span><span class="sxs-lookup"><span data-stu-id="bcc29-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="bcc29-110">Under **Modtagere skal** du vælge Markér alt, hvis mailen er landet i mappen med uønsket mail for alle modtagere af denne **mail.**</span><span class="sxs-lookup"><span data-stu-id="bcc29-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="bcc29-111">Hvis ikke, skal du kun vælge den bruger, der har rapporteret problemet.</span><span class="sxs-lookup"><span data-stu-id="bcc29-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="bcc29-112">Hvis **du vælger** Bør have været blokeret, skal du angive, om meddelelsen skal **være** blokeret som **spam,** **phishing** eller **malware,** og derefter vælge **Send.**</span><span class="sxs-lookup"><span data-stu-id="bcc29-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="bcc29-113">Du kan få mere at vide ved at se, hvordan du [sender mistænkeligt spam, phish, URL-adresser og filer til Microsoft til scanning.](https://go.microsoft.com/fwlink/?linkid=2101479)</span><span class="sxs-lookup"><span data-stu-id="bcc29-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
