---
title: Slet et websted permanent i SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955130"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>Slet et websted permanent i SharePoint

Hvis du vil genbruge en webadresse fra et slettet websted (for at genskabe et websted) eller permanent slette et websted, fordi det ikke længere er i brug,kan du bruge **Slet permanent** fra det nye SharePoint Administration. 

1. Gå til [siden Slettede websteder i det nye SharePoint Administration](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true), og log på med en konto, der har administratortilladelser for din organisation. 

2. Markér et websted i venstre kolonne. 

3. Klik på **Slet permanent**. 

**Bemærk**: Gruppe-forbundne websteder kan ikke slettes permanent fra det nye SharePoint Administration. Du skal bruge [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) i stedet.  

Hvis du vil have flere oplysninger, skal du se [Slet et websted permanent](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site). 
