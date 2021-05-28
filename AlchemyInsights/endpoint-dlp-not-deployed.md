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
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/27/2021
ms.locfileid: "52694807"
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

Per requisiti aggiuntivi sulla prevenzione della perdita dei dati degli endpoint, passare a [Introduzione alla prevenzione della perdita di dati degli endpoint](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).