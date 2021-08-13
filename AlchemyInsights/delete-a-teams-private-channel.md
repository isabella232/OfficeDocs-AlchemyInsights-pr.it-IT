---
title: Eliminare un canale privato di Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 33bf8a5cdc3a8e8da78c9d02e11387a778a7acce483e4485f595d9e05b344433
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948275"
---
# <a name="delete-a-teams-private-channel"></a>Eliminare un canale privato di Teams

Microsoft è consapevole di un problema che si verifica durante l'eliminazione di un canale privato di Teams se per il sito di SharePoint sottostante sono abilitati i criteri di conservazione di SharePoint. Microsoft sta lavorando alla risoluzione del problema. Nel frattempo, è possibile provare le soluzioni alternative seguenti per eliminare il canale privato.

**Escludere il Team o la raccolta siti dai criteri di conservazione di SharePoint.**

1. Passare al portale di amministrazione di Office 365 e selezionare **Mostra tutto** nel riquadro di spostamento sinistro.
2. In **Interfacce di amministrazione**, selezionare **Sicurezza e conformità** > **Prevenzione della perdita dei dati** > **Criteri**.
3. Identificare i criteri applicabili ai siti di SharePoint e modificarli in modo che il sito di SharePoint per il Team contenente il canale privato NON sia incluso nei criteri di conservazione.
4. Salvare il criterio.
    Possono essere necessarie fino a 24 ore prima che le impostazioni dei criteri diventino effettive.
    Una volta escluso il sito, è possibile eliminare il canale privato.  
    
È ***possibile*** eliminare il canale privato usando Microsoft Teams sul dispositivo Android. 

Per informazioni collegate a SharePoint, si veda [Non è possibile eliminare elementi in SharePoint Online o OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).