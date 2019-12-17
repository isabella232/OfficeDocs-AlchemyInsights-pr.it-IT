---
title: S/MIME in Outlook sul Web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 33e94eac6a2982b8036e13d17bf60015f244f2cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053229"
---
# <a name="encrypt-email-messages-in-outlook"></a>Crittografare i messaggi di posta elettronica in Outlook

La crittografia dei messaggi di Office 365 è basata su Microsoft Azure Rights Management (Azure RMS), che fa parte di Azure Information Protection. Se l'abbonamento include Azure Rights Management o Azure Information Protection, **non è necessario eseguire alcuna azione per attivare o disattivare manualmente** il servizio Rights Management.

In base al feedback dei clienti, non è più possibile abilitare le regole del flusso di posta di Exchange per crittografare automaticamente la posta elettronica in uscita contenente alcuni tipi di informazioni riservate nel tenant per impostazione predefinita. Al contrario, vengono fornite istruzioni dettagliate su come è possibile farlo da soli. Per ulteriori informazioni su come creare una regola di trasporto per crittografare le informazioni riservate, vedere [questo articolo](https://aka.ms/OmeEtr).

- Se si utilizza Outlook sul Web (in precedenza **OWA**): quando si compone un messaggio di posta elettronica, è sufficiente fare clic su **Proteggi** in OWA. Verrà applicata l'autorizzazione "non inoltrare". Fare clic su **Cambia autorizzazione** e scegliere **Crittografa** solo per crittografare il messaggio.

- Se si utilizza il **client di Outlook**: per inviare un messaggio crittografato da Outlook 2013 o 2016 o Outlook 2016 per Mac, selezionare **Opzioni** > **autorizzazioni**, quindi selezionare l'opzione di protezione necessaria.

- Per **crittografare automaticamente tutti i messaggi di posta elettronica** inviati a determinati destinatari o organizzazioni partner esterne, è necessario creare una regola di trasporto del flusso di posta nell'interfaccia di amministrazione di Exchange. Istruzioni dettagliate sono disponibili in [questo articolo del supporto tecnico](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

