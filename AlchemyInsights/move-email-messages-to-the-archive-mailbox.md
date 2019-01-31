---
title: Flytte e-mails til postkassen arkiv
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 2147c70f64087bf95fc4e39c193caeac3b2c5361
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 01/30/2019
ms.locfileid: "29660371"
---
<span data-ttu-id="b9adf-p101">Problemer med arkivering af elementer til arkiv-postkasse. Kontroller, at du har udført følgende trin:</span><span class="sxs-lookup"><span data-stu-id="b9adf-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="b9adf-p102">Bekræft, at en **arkivere postkasse** er aktiveret. Hvis ikke, skal du bruge trinnene i [denne artikel](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) til at aktivere postkassen arkiv.</span><span class="sxs-lookup"><span data-stu-id="b9adf-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="b9adf-106">Vælg **Tilbageholdelse mærker** under **Administration af overholdelse**i administrationssiden Exchange, oprette en **tilbageholdelse mærke** med handlingen **flytter til arkiv** , der indeholder den ønskede **Tilbageholdelse alder**.</span><span class="sxs-lookup"><span data-stu-id="b9adf-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="b9adf-107">Vælg **Opbevaringspolitikker**i Exchange Admin Center, Opret en **Opbevaringspolitik** , og Tilføj **flytter til arkiv** tilbageholdelse af mærket til denne politik.</span><span class="sxs-lookup"><span data-stu-id="b9adf-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="b9adf-p103">[Tildele opbevaringspolitikken](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til brugerens postkasse. Denne politik anvendes til både den **primære** og **arkiv** -postkasse.</span><span class="sxs-lookup"><span data-stu-id="b9adf-p103">[Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="b9adf-p104">Brugerens postkasse skulle nu være en arkiveringspolitik til at flytte varer til arkiv-postkasse. Det kan være nødvendigt at tvinge den administrerede mappe assistenten (MFA) til at køre og anvende de nye indstillinger i brugerens postkasse. Kør følgende kommando under [tilsluttet EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) til at starte en administreret Mappeassistent for en bestemt postkasse:</span><span class="sxs-lookup"><span data-stu-id="b9adf-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="b9adf-113">Vil have yderligere oplysninger om opsætning af en arkiveringspolitik, finder du i [oprette et arkiv og sletning af en politik for postkasser](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="b9adf-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

