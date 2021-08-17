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
ms.openlocfilehash: 2d5f0486ed8d4cbd95603f223bc0e48c4dcf38abb001d1616ca968b1d6bba7de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044236"
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