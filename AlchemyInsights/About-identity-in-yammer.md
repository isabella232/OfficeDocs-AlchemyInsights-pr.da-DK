---
title: Om identitet i Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664164"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="3dc86-102">Om identitet i Yammer</span><span class="sxs-lookup"><span data-stu-id="3dc86-102">About identity in Yammer</span></span>

<span data-ttu-id="3dc86-103">Det anbefales, at alle netværk udfører følgende trin for at undgå identitets relaterede problemer:</span><span class="sxs-lookup"><span data-stu-id="3dc86-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="3dc86-104">Gennemtving Office 365-identitet efter klargøring af Microsoft 365-konti til brugere i Azure AD for at sikre, at alle brugere logger på med deres primære Microsoft 365-konto.</span><span class="sxs-lookup"><span data-stu-id="3dc86-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="3dc86-105">Du kan finde flere oplysninger i [Gennemtving Office 365-identitet for Yammer-brugere](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="3dc86-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="3dc86-106">Konsolider flere Yammer-netværk.</span><span class="sxs-lookup"><span data-stu-id="3dc86-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="3dc86-107">Ældre Yammer-konfigurationer giver mulighed for at oprette forbindelse til én lejer med flere Yammer-netværk.</span><span class="sxs-lookup"><span data-stu-id="3dc86-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="3dc86-108">Hvis du vil have mere at vide, skal du se [Network migration-Konsolider flere Yammer-netværk](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="3dc86-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="3dc86-109">Du kan også gennemtvinge licensering til Yammer for at blokere brugere fra Yammer, hvis de ikke har en licens.</span><span class="sxs-lookup"><span data-stu-id="3dc86-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="3dc86-110">Du kan finde flere oplysninger i [administrere Yammer-brugerlicenser i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="3dc86-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="3dc86-111">Til sidst skal du overvåge bruger listen for ældre Yammer-netværk og suspendere ældre brugere.</span><span class="sxs-lookup"><span data-stu-id="3dc86-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="3dc86-112">Det anbefales, at du suspenderer (deaktiverer) brugere i stedet for at slette dem, da sletningen er uigenkaldelige.</span><span class="sxs-lookup"><span data-stu-id="3dc86-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="3dc86-113">Hvis du vil have mere at vide, skal du se [Overvåg Yammer-brugere i netværk, der er forbundet til Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) og [fjernbrugere](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="3dc86-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="3dc86-114">Hvis du konfigurerer Yammer ved hjælp af disse trin, er du også klar til at konfigurere dit Yammer-netværk til Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3dc86-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="3dc86-115">Hvis du vil have mere at vide, skal du se [konfigurere dit Yammer-netværk til oprindelig tilstand for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="3dc86-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>