---
title: Prevenzione della perdita dei dati degli endpoint non distribuita sul dispositivo dell’utente
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 56783b007b5eebc7ca671247f24f5b513b9d8f5c321f59a63170425c2d376a94
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57900252"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>Prevenzione della perdita dei dati degli endpoint non distribuita sul dispositivo dell’utente

Se l’impostazione della prevenzione della perdita di dati degli endpoint non è stata applicata sul dispositivo dell’utente, confermare che si soddisfano questi requisiti:

- Windows 10 x64 build 1809 o installata successivamente sul dispositivo.
- Client antimalware versione 4.18.2009.7 o installata successivamente.
- Il dispositivo è **uno** dei seguenti:
    
    - Aggiunto ad Azure Active Directory (Azure AD)
    - Aggiunto ad Azure AD ibrido
    - Registrato ad Azure AD

- Per applicare azioni dei criteri, assicurarsi che il browser Microsoft Edge Chromium sia installato sul dispositivo endpoint.

Per requisiti aggiuntivi sulla prevenzione della perdita dei dati degli endpoint, passare a [Introduzione alla prevenzione della perdita di dati degli endpoint](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).