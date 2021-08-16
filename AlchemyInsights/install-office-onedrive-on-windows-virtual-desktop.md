---
title: Installere Office og OneDrive på Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 226bd24a955f6165969102c8cf00cf45da537ee05a5363c74f1dfd055d922e1d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: da-DK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028610"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Installere Office og OneDrive på Windows Virtual Desktop

1. [Forbered og tilpas et VHD-masterbillede](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image). Opret en virtuel maskine (VM), hvis den ikke allerede er blevet oprettet.

1. [Installer Office aktiveringstilstand for en delt computer.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode) Aktivering af delte computere giver flere brugere adgang til Office.

1. [Installér OneDrive i tilstanden pr. computer.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode) Normalt er OneDrive installeret pr. bruger, men her skal den installeres pr. computer.