---
title: Problemi correlati alla VPN
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
- "1545"
- "9000076"
ms.openlocfilehash: 3c031725c92f5d7af7c0dd0c37ea34fecf4792c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726095"
---
# <a name="vpn-related-issues"></a>Problemi correlati alla VPN

L'implementazione efficace della connettività VPN per i client MDM dipende da un profilo distribuito che riflette correttamente i requisiti dell'infrastruttura VPN. Per le impostazioni appropriate per le piattaforme client su cui si sta lavorando, vedere: 

[Impostazioni del dispositivo Windows 10 e Windows Holographic per aggiungere connessioni VPN usando Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Aggiungere impostazioni VPN sui dispositivi iOS e iPadOS in Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Impostazioni di dispositivi Android per configurare la VPN in Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Aggiungere impostazioni VPN sui dispositivi macOS in Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Se il profilo VPN usa l'autenticazione basata su certificato, assicurarsi che il certificato radice e i profili dei certificati di autenticazione client collegati al profilo VPN vengano distribuiti correttamente.

**Problemi comuni**

**Ho distribuito un profilo VPN in un dispositivo. Intune indica che l'operazione è riuscita, ma il dispositivo non è connesso alla rete VPN.**

Lo stato corretto indica che Intune ha distribuito correttamente il profilo come configurato. Tuttavia, queste configurazioni potrebbero non corrispondere ai requisiti di rete e/o di autenticazione. Rivedere i registri nel servizio di infrastruttura e autenticazione (sul server VPN e sul server NPS/RADIUS) per ulteriori dettagli sul tentativo di connessione. Potrebbe essere necessario usare il team dell'infrastruttura di rete o il fornitore di terze parti per raccogliere e rivedere i registri.

**Quando configuro una VPN personalizzata per iOS, la funzionalità VPN per app non è disponibile.**

I dispositivi VPN per le app per dispositivi iOS di Intune sono attualmente disponibili per un elenco di provider e partner specifico, che deve inoltre soddisfare i prerequisiti dei certificati prima di poter configurare una VPN per app. Per altre informazioni, vedere [Configurare una rete privata virtuale (VPN) per app per dispositivi iOS/iPadOS in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Per altre informazioni su tutti i tipi di connessione VPN in Intune, vedere [Creare profili VPN per connettersi ai server VPN di Intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**La rete VPN iOS su richiesta non viene attivata quando si accede a un dominio configurato**

Per testare le impostazioni di VPN automatiche, impostare i seguenti valori:

Voglio eseguire queste operazioni: **Valutare ogni tentativo di connessione** 

Scegli se eseguire la connessione: **Eseguire la connessione se necessario**

Quando gli utenti accedono a questi domini: **nome dominio** *di destinazione*

Se la configurazione non riesce, aggiungere l'elemento seguente:

Quando l'URL non è raggiungibile, forzare la connessione VPN: **BADURL**