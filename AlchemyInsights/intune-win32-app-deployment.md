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
ms.openlocfilehash: d169dc0dd4e3cd9d94681d7db16ce3051677b708df02d3c9bd461855daabb295
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925889"
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