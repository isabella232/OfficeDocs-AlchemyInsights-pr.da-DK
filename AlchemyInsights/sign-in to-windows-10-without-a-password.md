---
title: Log på Windows 10 uden at bruge en adgangskode
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830540"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="97261-102">Log på Windows 10 uden at bruge en adgangskode</span><span class="sxs-lookup"><span data-stu-id="97261-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="97261-103">For at undgå at skulle skrive en adgangskode ved start af Windows anbefaler vi, at du bruger en af Windows Hello-indstillingerne til sikker logon, f.eks. en pinkode, ansigtsgenkendelse eller fingeraftryk, hvis den er tilgængelig.</span><span class="sxs-lookup"><span data-stu-id="97261-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="97261-104">Hvis du er sikker på, at du vil deaktivere sikker logon, skal du se vejledningen "Log automatisk på Windows 10" nedenfor.</span><span class="sxs-lookup"><span data-stu-id="97261-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="97261-105">**Gør Windows Hello-alternativer sikre til adgangskoden til kontoen**</span><span class="sxs-lookup"><span data-stu-id="97261-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="97261-106">Gå til **Indstillinger > konti > Logonindstillinger** (eller klik [her).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="97261-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="97261-107">De tilgængelige indstillinger for logon vises.</span><span class="sxs-lookup"><span data-stu-id="97261-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="97261-108">Eksempel:</span><span class="sxs-lookup"><span data-stu-id="97261-108">For example:</span></span>

![Logonindstillinger.](media/sign-in-options.png)

<span data-ttu-id="97261-110">Klik eller tryk på en af indstillingerne for at konfigurere den.</span><span class="sxs-lookup"><span data-stu-id="97261-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="97261-111">Næste gang du starter eller låser Windows op, vil du kunne bruge den nye indstilling i stedet for en adgangskode.</span><span class="sxs-lookup"><span data-stu-id="97261-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="97261-112">**Log automatisk på Windows 10**</span><span class="sxs-lookup"><span data-stu-id="97261-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="97261-113">**Bemærk!** Automatisk logon er praktisk, men introducerer en sikkerhedsrisiko, især hvis din pc er tilgængelig for flere personer.</span><span class="sxs-lookup"><span data-stu-id="97261-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="97261-114">Klik eller tryk på **knappen Start** på proceslinjen.</span><span class="sxs-lookup"><span data-stu-id="97261-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="97261-115">Skriv **netplwiz,** og tryk på Enter for at åbne vinduet Brugerkonti.</span><span class="sxs-lookup"><span data-stu-id="97261-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="97261-116">Under **Brugerkonti skal** du klikke på den konto, du automatisk vil logge på, når Windows starter.</span><span class="sxs-lookup"><span data-stu-id="97261-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="97261-117">Fjern markeringen i afkrydsningsfeltet "Brugere skal angive et brugernavn og en adgangskode for at bruge denne computer".</span><span class="sxs-lookup"><span data-stu-id="97261-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Brugere skal angive et brugernavn og en adgangskode.](media/users-must-enter-username.png)

5. <span data-ttu-id="97261-119">Klik på **OK**.</span><span class="sxs-lookup"><span data-stu-id="97261-119">Click **OK**.</span></span> <span data-ttu-id="97261-120">Du bliver bedt om at angive og bekræfte adgangskoden for den konto, du har valgt.</span><span class="sxs-lookup"><span data-stu-id="97261-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="97261-121">Klik **på OK** for at afslutte.</span><span class="sxs-lookup"><span data-stu-id="97261-121">Click **OK** to finish.</span></span> <span data-ttu-id="97261-122">Næste gang Windows 10 starter, logges der automatisk på den konto, du har valgt.</span><span class="sxs-lookup"><span data-stu-id="97261-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
