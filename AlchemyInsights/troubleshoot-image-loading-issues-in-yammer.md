---
title: Risoluzione dei problemi di caricamento delle immagini in Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 11315fd84f92251e435320f4550286fb2db4b0128f7ac85c0f79972e3f7fd203
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939239"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a>Risoluzione dei problemi di caricamento delle immagini in Yammer

Se si verificano problemi con le anteprime di foto e file in Yammer, risolvere i problemi controllando se il problema avviene per tutti gli utenti, su dispositivi mobili e se è riproducibile durante il caricamento degli allegati.  

**Problemi con la foto profilo**  

Se gli utenti finali accedono a Yammer tramite Microsoft 365, devono cambiare il profilo, incluse le foto del profilo. Se gli utenti non dispongono delle autorizzazioni per aggiornare il profilo, un amministratore potrà eseguire l'aggiornamento per conto loro. Per ulteriori informazioni, vedere [Visualizzare e aggiornare il profilo in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).

Per informazioni sulla modifica del profilo, incluse le foto del profilo, vedere [Cambiare il profilo e le impostazioni di Yammer](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851). 

Le foto del profilo aggiornate vengono sincronizzate in modo diverso rispetto agli attributi del profilo. Gli utenti devono accedere per avviare una sincronizzazione della foto del profilo. Per informazioni, vedere [Le immagini del profilo vengono aggiornate da Office 365 a Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).

Per informazioni sul ciclo di vita degli utenti per Yammer, vedere [Gestire gli utenti di Yammer per l'intero ciclo di vita da Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).  

Per informazioni dettagliate su come funziona la sincronizzazione delle immagini del profilo in Microsoft 365, vedere [Informazioni sulla sincronizzazione delle immagini del profilo in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).  

**Problemi relativi alle anteprime di documenti e miniature di immagini**  

Quando file o immagini vengono pubblicati in Yammer, le anteprime potrebbero non essere visualizzate perché: 

- Il file è danneggiato e non può essere elaborato.
- Il file non è stato caricato di recente in SharePoint Online o Yammer ha metadati non validi per altri motivi.
- Gli URL necessari per caricare le immagini di anteprima sono bloccati.
- L'anteprima del file è stata rimossa dall'utente prima di pubblicarla.
- Un problema di servizio ha impedito la generazione di un'anteprima.

**Nota** Le anteprime per i collegamenti e i caricamenti di file potrebbero comportarsi in modo diverso. È possibile che i collegamenti a file su Internet o collegamenti che richiedono ulteriore autenticazioni non vengano visualizzati correttamente.

Per altre informazioni, vedere [Allegare un file o un'immagine a un messaggio di Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf). 