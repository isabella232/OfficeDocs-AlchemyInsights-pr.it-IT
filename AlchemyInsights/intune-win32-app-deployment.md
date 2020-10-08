---
title: Distribuzione delle app Win32 con Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366526"
---
# <a name="intune-win32-app-deployment"></a>Distribuzione delle app Win32 con Intune

Microsoft Intune consente di distribuire le applicazioni Win32, inclusi MSI e i file .EXE, sui dispositivi Windows 10. Il meccanismo di distribuzione usato richiede che l’estensione Intune Management Extension (IME) sia installata sul dispositivo di destinazione. L’estensione IME è installata automaticamente dopo che lo script di PowerShell o la distribuzione dell’applicazione Win32 sono associati a un utente/dispositivo.

La distribuzione delle app Win32 prevede anche una serie di prerequisiti da soddisfare, tra cui:

- Piattaforme supportate: Windows 10 versione 1607 o successiva (versioni Enterprise, Pro ed Education)
- Architettura supportata: x86 e x64.
- Gestione dispositivi: AAD connesso e registrato automaticamente (inclusi i domini ibridi aggiunti e i criteri di gruppo registrati automaticamente).
- Formato pacchetto dell’applicazione: file .**intunewin** preparato dallo strumento [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).
- Limitazioni:
    - Dimensione massima: 8 GB.
    - Architettura supportata: ARM.

Consultare il documento "[Aggiungere, assegnare e monitorare app Win32 in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" per le informazioni su questi passaggi.

I dettagli per risoluzione dei problemi di distribuzione su Windows, incluse le app Win32, sono disponibili nei seguenti documenti

- [Risoluzione dei problemi di installazione delle app](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Risoluzione dei problemi delle app Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)