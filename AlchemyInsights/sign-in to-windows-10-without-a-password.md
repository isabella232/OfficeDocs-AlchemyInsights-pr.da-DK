---
title: Logge på Windows 10 uden at bruge en adgangskode
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719947"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="02431-102">Logge på Windows 10 uden at bruge en adgangskode</span><span class="sxs-lookup"><span data-stu-id="02431-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="02431-103">Hvis du vil undgå at skulle skrive en adgangskode ved start af Windows, anbefaler vi, at du bruger en af de Secure-logonindstillinger til Windows Hello, som en pinkode, ansigtsgenkendelse eller fingeraftryk, hvis det er muligt.</span><span class="sxs-lookup"><span data-stu-id="02431-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="02431-104">Hvis du er sikker på, at du vil deaktivere Secure logon, skal du se instruktionerne "Log automatisk på Windows 10" nedenfor.</span><span class="sxs-lookup"><span data-stu-id="02431-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="02431-105">**Sikre Windows Hello-alternativer til kontoens adgangskode**</span><span class="sxs-lookup"><span data-stu-id="02431-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="02431-106">Gå til **indstillinger > konti > indstillinger for logon** (eller klik [her](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="02431-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="02431-107">Tilgængelige logonindstillinger vises.</span><span class="sxs-lookup"><span data-stu-id="02431-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="02431-108">Det kan f.eks. være:</span><span class="sxs-lookup"><span data-stu-id="02431-108">For example:</span></span>

![Logonindstillinger.](media/sign-in-options.png)

<span data-ttu-id="02431-110">Klik eller tryk på en af indstillingerne for at konfigurere den.</span><span class="sxs-lookup"><span data-stu-id="02431-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="02431-111">Næste gang du starter eller låser Windows op, kan du bruge den nye indstilling i stedet for en adgangskode.</span><span class="sxs-lookup"><span data-stu-id="02431-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="02431-112">**Logge på Windows 10 automatisk**</span><span class="sxs-lookup"><span data-stu-id="02431-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="02431-113">**Bemærk**! det er praktisk at logge på automatisk logon, men det introducerer en sikkerhedsrisiko, især hvis din pc er tilgængelig for flere personer.</span><span class="sxs-lookup"><span data-stu-id="02431-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="02431-114">Klik eller tryk på knappen **Start** på proceslinjen.</span><span class="sxs-lookup"><span data-stu-id="02431-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="02431-115">Skriv **netplwiz** , og tryk på ENTER for at åbne vinduet brugerkonti.</span><span class="sxs-lookup"><span data-stu-id="02431-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="02431-116">I **brugerkonti**skal du klikke på den konto, du automatisk vil logge på, når Windows starter.</span><span class="sxs-lookup"><span data-stu-id="02431-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="02431-117">Fjern markeringen i afkrydsningsfeltet "brugerne skal angive et Brugernavn og en adgangskode for at bruge denne computer".</span><span class="sxs-lookup"><span data-stu-id="02431-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Brugerne skal angive et Brugernavn og en adgangskode indstilling.](media/users-must-enter-username.png)

5. <span data-ttu-id="02431-119">Klik på **OK**.</span><span class="sxs-lookup"><span data-stu-id="02431-119">Click **OK**.</span></span> <span data-ttu-id="02431-120">Du bliver bedt om at angive og bekræfte adgangskoden for den konto, du har valgt.</span><span class="sxs-lookup"><span data-stu-id="02431-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="02431-121">Klik på **OK** for at afslutte.</span><span class="sxs-lookup"><span data-stu-id="02431-121">Click **OK** to finish.</span></span> <span data-ttu-id="02431-122">Næste gang Windows 10 starter, bliver den automatisk logget på den konto, du har valgt.</span><span class="sxs-lookup"><span data-stu-id="02431-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
