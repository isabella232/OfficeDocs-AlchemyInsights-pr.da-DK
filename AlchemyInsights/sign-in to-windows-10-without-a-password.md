---
title: Log på Windows 10 uden at bruge en adgangskode
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588275"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="20e9e-102">Log på Windows 10 uden at bruge en adgangskode</span><span class="sxs-lookup"><span data-stu-id="20e9e-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="20e9e-103">Hvis du vil undgå at skulle skrive en adgangskode ved start af Windows, anbefaler vi, at du bruger en af de sikre logonindstillinger i Windows Hello, f.eks.</span><span class="sxs-lookup"><span data-stu-id="20e9e-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="20e9e-104">Hvis du virkelig vil deaktivere sikker logon, skal du se vejledningen "Log automatisk på Windows 10" nedenfor.</span><span class="sxs-lookup"><span data-stu-id="20e9e-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="20e9e-105">**Sikre Alternativer til Windows Hello til adgangskoden til kontoen**</span><span class="sxs-lookup"><span data-stu-id="20e9e-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="20e9e-106">Gå til **Indstillinger > konti > logonindstillinger** (eller klik [her](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="20e9e-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="20e9e-107">Tilgængelige logonindstillinger vises.</span><span class="sxs-lookup"><span data-stu-id="20e9e-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="20e9e-108">Det kan f.eks. være:</span><span class="sxs-lookup"><span data-stu-id="20e9e-108">For example:</span></span>

![Indstillinger for logon.](media/sign-in-options.png)

<span data-ttu-id="20e9e-110">Klik eller tryk på en af indstillingerne for at konfigurere den.</span><span class="sxs-lookup"><span data-stu-id="20e9e-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="20e9e-111">Næste gang du starter eller låser Windows op, kan du bruge den nye indstilling i stedet for en adgangskode.</span><span class="sxs-lookup"><span data-stu-id="20e9e-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="20e9e-112">**Log på Windows 10 automatisk**</span><span class="sxs-lookup"><span data-stu-id="20e9e-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="20e9e-113">**Bemærk:** Automatisk login er praktisk, men indfører en sikkerhedsrisiko, især hvis din pc er tilgængelig for flere personer.</span><span class="sxs-lookup"><span data-stu-id="20e9e-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="20e9e-114">Klik eller tryk på knappen **Start** på proceslinjen.</span><span class="sxs-lookup"><span data-stu-id="20e9e-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="20e9e-115">Skriv **netplwiz,** og tryk på enter for at åbne vinduet Brugerkonti.</span><span class="sxs-lookup"><span data-stu-id="20e9e-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="20e9e-116">Klik på den konto, du automatisk vil logge på, når Windows starter, i **Brugerkonti.**</span><span class="sxs-lookup"><span data-stu-id="20e9e-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="20e9e-117">Fjern markeringen i afkrydsningsfeltet "Brugere skal angive et brugernavn og en adgangskode for at bruge denne computer".</span><span class="sxs-lookup"><span data-stu-id="20e9e-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Brugerne skal angive en indstilling for brugernavn og adgangskode.](media/users-must-enter-username.png)

5. <span data-ttu-id="20e9e-119">Klik på **OK**.</span><span class="sxs-lookup"><span data-stu-id="20e9e-119">Click **OK**.</span></span> <span data-ttu-id="20e9e-120">Du bliver bedt om at indtaste og bekræfte adgangskoden til den konto, du har valgt.</span><span class="sxs-lookup"><span data-stu-id="20e9e-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="20e9e-121">Klik på **OK** for at afslutte.</span><span class="sxs-lookup"><span data-stu-id="20e9e-121">Click **OK** to finish.</span></span> <span data-ttu-id="20e9e-122">Næste gang Windows 10 starter, logges den automatisk på den konto, du har valgt.</span><span class="sxs-lookup"><span data-stu-id="20e9e-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
