---
title: Begræns SharePoint online til klassisk tilstand
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 6315a83ac825f96ceea60798d441de8e8e53336fe29eda4d0491dd8a6a43b352
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958795"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Begræns SharePoint online til klassisk tilstand

Nogle organisationer kræver stadig oplevelsen klassisk tilstand. Der er ingen planer om at fjerne klassisk tilstand på et detaljeret niveau, men det er ikke længere muligt at begrænse en hel organisation (lejer) til klassisk tilstand for lister og biblioteker.

Administratoren har følgende muligheder for at administrere individuelle lister og biblioteker i klassisk tilstand ved hjælp af granular opt-out-parametre, som vi leverer på følgende niveauer:

- gruppe af websteder
- websted
- liste
- bibliotek

Lister, der anvender visse funktioner og tilpasninger, som ikke understøttes af moderne, vil stadig automatisk blive ændret til tilstanden Klassisk.

Fra og med d. 1. april 2019 vil processen med at deaktivere lejerniveau fravælge moderne lister og biblioteker begynde og fortsætte til den 31. maj 2019.  De lister og biblioteker, der er i den klassiske tilstand som et resultat af lejertilvalget, ændres automatisk til moderne.

Hvis du har brug for [](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) klassisk tilstand, kan [](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) du se flere oplysninger her og PnP Powershell-vejledningen her, der beskriver de indstillinger og værktøjer, du kan bruge i dag for at bruge den klassiske tilstand.
