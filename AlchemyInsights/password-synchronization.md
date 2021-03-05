---
title: Synkronisering af adgangskoder
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481444"
---
# <a name="password-synchronization"></a><span data-ttu-id="88d0f-102">Synkronisering af adgangskoder</span><span class="sxs-lookup"><span data-stu-id="88d0f-102">Password synchronization</span></span>

<span data-ttu-id="88d0f-103">**Synkronisering af adgangskodehash virker slet ikke**</span><span class="sxs-lookup"><span data-stu-id="88d0f-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="88d0f-104">Nogle almindelige problemer, som kunder støder på, når synkronisering af adgangskodehash ikke virker, er:</span><span class="sxs-lookup"><span data-stu-id="88d0f-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="88d0f-105">Active Directory-kontoen, der bruges af Azure AD Connect til at kommunikere med Active Directory i det lokale miljø, tildeles ikke **Repliker** mappeændringer og **Repliker** mappeændringer Alle tilladelser, som er nødvendige for synkronisering af adgangskoder – Du skal løse dette problem ved at give disse tilladelser til Active Directory-kontoen.</span><span class="sxs-lookup"><span data-stu-id="88d0f-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="88d0f-106">Synkronisering af adgangskodehash er deaktiveret, efter  at en administrator har ændret metoden Bruger Sign-In fra Synkronisering af adgangskode til en anden  indstilling, f.eks. Sammenslutning med **AD FS,** i Azure AD Connect-guiden . Du kan løse dette problem ved at genaktivere funktionen til synkronisering af adgangskodehash i azure AD Connect-guiden.</span><span class="sxs-lookup"><span data-stu-id="88d0f-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="88d0f-107">Forbindelsesproblem med Active Directory i det lokale miljø.</span><span class="sxs-lookup"><span data-stu-id="88d0f-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="88d0f-108">Nogle domænecontrollere er f.eks. ikke tilgængelige [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) for Azure AD Connect, eller de påkrævede porte er blokeret af Firewall – du skal løse dette problem ved at sikre, at forbindelsen mellem Azure AD Connect-serveren og den lokale Active Directory fungerer korrekt.</span><span class="sxs-lookup"><span data-stu-id="88d0f-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="88d0f-109">Azure AD Connect-serveren befinder sig i øjeblikket i midlertidig tilstand, hvilket medfører, at serveren ikke kan bruge adgangskodehashes – Hvis du vil foretage fejlfinding af problemet, skal du følge de trin, der er beskrevet i afsnittet Fejlfinding i forbindelse med synkronisering af adgangskoder med [Azure AD Connect-synkronisering –](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)Der synkroniseres ingen adgangskoder.</span><span class="sxs-lookup"><span data-stu-id="88d0f-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="88d0f-110">**Synkronisering af adgangskodehash fungerer ikke for nogle af mine brugere**</span><span class="sxs-lookup"><span data-stu-id="88d0f-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="88d0f-111">Hvis du har bemærket, at adgangskodehash ikke  synkroniseres for en bruger, kan du bruge fejlfindingsopgaven i Azure AD Connect til at undersøge og løse problemet.</span><span class="sxs-lookup"><span data-stu-id="88d0f-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="88d0f-112">Udfør følgende opgaver:</span><span class="sxs-lookup"><span data-stu-id="88d0f-112">Perform the following tasks:</span></span>

    <span data-ttu-id="88d0f-113">a.</span><span class="sxs-lookup"><span data-stu-id="88d0f-113">a.</span></span> [<span data-ttu-id="88d0f-114">Kør fejlfindingsopgaven i guiden</span><span class="sxs-lookup"><span data-stu-id="88d0f-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="88d0f-115">b.</span><span class="sxs-lookup"><span data-stu-id="88d0f-115">b.</span></span> [<span data-ttu-id="88d0f-116">Brug fejlfindings-cmdlet'en til at undersøge synkroniseringsproblemet med adgangskodehash til en bestemt brug</span><span class="sxs-lookup"><span data-stu-id="88d0f-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="88d0f-117">Det lokale Active Directory-brugerobjekt er aktiveret for **brugeren, og adgangskoden skal ændres ved næste logonindstilling.**</span><span class="sxs-lookup"><span data-stu-id="88d0f-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="88d0f-118">Når denne indstilling er aktiveret, får brugeren tildelt en midlertidig adgangskode og bliver bedt om at ændre adgangskoden ved næste logon.</span><span class="sxs-lookup"><span data-stu-id="88d0f-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="88d0f-119">Azure AD Connect synkroniserer ikke midlertidige adgangskoder til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="88d0f-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="88d0f-120">Du kan løse problemet herover ved at udføre en af følgende opgaver:</span><span class="sxs-lookup"><span data-stu-id="88d0f-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="88d0f-121">Bed brugeren om at logge på det lokale program (f.eks. Skrivebordsversionen af Windows) og ændre adgangskoden.</span><span class="sxs-lookup"><span data-stu-id="88d0f-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="88d0f-122">Den nye adgangskode synkroniseres med Azure AD.</span><span class="sxs-lookup"><span data-stu-id="88d0f-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="88d0f-123">Få en administrator til at opdatere brugerens adgangskode uden at aktivere indstillingen Brugeren skal ændre adgangskoden ved næste **logon** og dele den nye adgangskode med brugeren.</span><span class="sxs-lookup"><span data-stu-id="88d0f-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="88d0f-124">Det lokale Active Directory User-objekt er ikke konfigureret **korrekt** til objektsynkronisering eller synkronisering af adgangskoder.</span><span class="sxs-lookup"><span data-stu-id="88d0f-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="88d0f-125">Hvis du vil foretage fejlfinding af dette problem, skal du følge de trin, der er beskrevet i [Fejlfinding af synkronisering af adgangskodehash med Azure AD Connect-synkronisering.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="88d0f-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







