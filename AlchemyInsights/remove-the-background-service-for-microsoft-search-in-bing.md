---
title: Rimuovere il servizio in background per Microsoft Search in Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/12/2021
ms.locfileid: "50753416"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Rimuovere il servizio in background per Microsoft Search in Bing

Per rimuovere il servizio in background per Microsoft Search in Bing, è possibile provare i rimedi seguenti:

1. Per ripristinare le impostazioni originali del motore di ricerca, eseguire queste operazioni:

    a. Disattivare l'opzione **Usa Bing come motore di ricerca predefinito[](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) impostando l’interruttore su Disattivato**.

    b. [Accedere all'interfaccia di amministrazione di Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) e deselezionare l'impostazione che riguarda tutti gli utenti dell'organizzazione.

2. Per rimuovere il servizio in background da un singolo dispositivo, eseguire queste attività:

    a. Scegliere **Pannello di controllo > Programmi > Programmi e funzionalità**.

    b. Fare clic con il pulsante destro del mouse su **Microsoft Search in Bing** nell'elenco dei programmi installati e quindi scegliere **Disinstalla**.

3. Per rimuovere il servizio in background da più dispositivi dell'organizzazione, accedere come amministratore ed eseguire il comando seguente in uno script: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
