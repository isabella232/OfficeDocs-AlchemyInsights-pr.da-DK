---
title: Installér Office og OneDrive på Windows Virtual Desktop
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
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: da-DK
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595509"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Installér Office og OneDrive på Windows Virtual Desktop

1. [Forbered og tilpas et master-VHD-billede.](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image) Opret en virtuel maskine (VM), hvis den ikke allerede er blevet oprettet.

1. [Installér Office i aktiveringstilstand for delt computer.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode) Aktivering af delt computer giver flere brugere adgang til Office.

1. [Installér OneDrive i tilstanden pr. computer.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode) Normalt installeres OneDrive pr. bruger, men her skal det installeres pr. computer.