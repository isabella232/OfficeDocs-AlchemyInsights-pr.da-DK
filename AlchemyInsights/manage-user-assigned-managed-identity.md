---
title: Administrere en bruger tildelt administreret identitet
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8211"
- "9003230"
ms.openlocfilehash: a44cb484b6d89e6d5f67b2900c38dde3610b0e23
ms.sourcegitcommit: 23e778f7414e5f1a98cc786146fe76d622b458bc
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177461"
---
# <a name="manage-a-user-assigned-managed-identity"></a><span data-ttu-id="a4a80-102">Administrere en bruger tildelt administreret identitet</span><span class="sxs-lookup"><span data-stu-id="a4a80-102">Manage a user-assigned managed identity</span></span>

<span data-ttu-id="a4a80-103">Administrationen af en bruger tildelt administreret identitet indebærer:</span><span class="sxs-lookup"><span data-stu-id="a4a80-103">The management of a user-assigned managed identity involves:</span></span>

- <span data-ttu-id="a4a80-104">Tildele roller til en bruger-tildelt administreret identitet</span><span class="sxs-lookup"><span data-stu-id="a4a80-104">Assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="a4a80-105">Sletning af en bruger tildelt administreret identitet</span><span class="sxs-lookup"><span data-stu-id="a4a80-105">Deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="a4a80-106">Liste over en bruger tildelt administreret identitet</span><span class="sxs-lookup"><span data-stu-id="a4a80-106">Listing a user-assigned managed identity</span></span>

<span data-ttu-id="a4a80-107">Du kan finde flere oplysninger om de opgaver, der er nævnt ovenfor, i følgende artikler:</span><span class="sxs-lookup"><span data-stu-id="a4a80-107">For more information on the tasks mentioned above, see the following articles:</span></span>

- <span data-ttu-id="a4a80-108">[Sådan oprettes en brugerbaseret administreret](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) identitet – til at tildele roller til en brugerbaseret administreret identitet</span><span class="sxs-lookup"><span data-stu-id="a4a80-108">[How to create a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="a4a80-109">[Sådan sletter du en bruger tildelt administreret](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) identitet – for at slette en bruger tildelt administreret identitet</span><span class="sxs-lookup"><span data-stu-id="a4a80-109">[How to delete a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="a4a80-110">[Sådan får du vist en bruger tildelt administreret identitet](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) – til angivelse af en bruger tildelt administreret identitet</span><span class="sxs-lookup"><span data-stu-id="a4a80-110">[How to list a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for listing a user-assigned managed identity</span></span>

> [!NOTE]
> <span data-ttu-id="a4a80-111">Kontrollér, om du har **rolletildelingen Administreret identitetsbidrager.**</span><span class="sxs-lookup"><span data-stu-id="a4a80-111">Verify whether you have the **Managed Identity Contributor** role assignment.</span></span> <span data-ttu-id="a4a80-112">Denne rolletildeling er påkrævet for at oprette/slette bruger tildelte administrerede identiteter.</span><span class="sxs-lookup"><span data-stu-id="a4a80-112">That role assignment is required for creating/deleting user-assigned managed identities.</span></span>
