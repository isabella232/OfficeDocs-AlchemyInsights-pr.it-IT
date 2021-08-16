---
title: S/MIME in Outlook sul Web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010728"
---
# <a name="encrypt-email-messages-in-outlook"></a>Crittografare i messaggi di posta elettronica Outlook

Microsoft 365 La crittografia dei messaggi è Microsoft Azure Rights Management (Azure RMS), che fa parte di Azure Information Protection. Se la sottoscrizione include Azure Rights Management o Azure Information **Protection,** non è necessario eseguire alcuna azione per abilitare o attivare manualmente Rights Management Service.

In base al feedback dei clienti, non abilitazione delle regole del flusso di posta Exchange crittografare automaticamente la posta elettronica in uscita contenente determinati tipi di informazioni riservate nel tenant per impostazione predefinita. Vengono invece fornite istruzioni dettagliate su come eseguire questa operazione. Per ulteriori informazioni su come creare una regola di trasporto per crittografare le informazioni riservate, vedere [questo articolo](https://aka.ms/OmeEtr).

- Se si utilizza Outlook sul Web (in precedenza **OWA**): Quando si compone un messaggio di posta elettronica, è sufficiente fare clic **su** Proteggi in OWA. Verrà applicata l'autorizzazione "Non inoltrare". Fare **clic su Modifica** autorizzazione e scegliere **Crittografa** per crittografare solo il messaggio.

- Se si utilizza **Outlook client:** per inviare un messaggio crittografato da Outlook 2013 o 2016 o Outlook 2016 per Mac, selezionare Opzioni   >  **Autorizzazioni,** quindi selezionare l'opzione di protezione necessaria.

- Per **crittografare** automaticamente tutti i messaggi di posta elettronica inviati a determinati destinatari o organizzazioni partner esterne, è necessario creare una regola di trasporto del flusso di posta nell'Exchange admin center. In questo articolo di supporto vengono fornite [istruzioni dettagliate.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

