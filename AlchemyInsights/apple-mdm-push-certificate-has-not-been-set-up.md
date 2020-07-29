---
title: Il certificato Apple MDM push non è stato configurato
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431649"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Il certificato Apple MDM push non è stato configurato

Per l'abbonamento non è stato configurato un certificato Apple MDM push, noto anche come certificato del servizio di notifica push Apple (APNS). Se non è configurato un certificato Apple MDM push, non è possibile registrare e gestire dispositivi iOS e MacOS. Dopo l'aggiunta del certificato in Intune, gli utenti potranno installare l'app Portale aziendale per registrare i propri dispositivi iOS.

1. Selezionare **"Accetto".** per assegnare a Microsoft l'autorizzazione a inviare dati a Apple.

2. Selezionare **Scaricare il CSR** la richiesta di firma del certificato Intune necessaria per creare un certificato Apple MDM push. Il file è utilizzato per richiedere un certificato di relazione di trust dal portale dei certificati push di Apple.

3. Selezionare **Creare il certificato MDM push** per andare sul portale dei certificati push di Apple. Accedere con l'ID Apple aziendale e selezionare **Creare un certificato**. Selezionare **Scegliere file**, cercare il file della richiesta di firma del certificato, quindi scegliere **Caricare**. Nella pagina di conferma scegliere **Download** per scaricare il file del certificato (con estensione PEM) e salvare il file in locale.
 
**Nota**: il certificato è associato all'ID Apple usato per crearlo. Come procedura consigliata, usare un ID Apple aziendale per le attività di gestione e verificare che la cassetta postale sia monitorata da più di una persona o usando una lista di distribuzione. Non usare mai un ID Apple personale. Usare lo stesso ID Apple per rinnovare il certificato push Apple ogni 12 mesi.
 
4. Inserire l'ID Apple usato per creare il certificato MDM push Apple. Registrare questo ID come promemoria per quando è necessario rinnovare il certificato.

5. Cercare il file del certificato (con estensione PEM), scegliere **Aprire**, quindi scegliere **Caricare**. Con il certificato push, Intune può registrare e gestire i dispositivi Apple.