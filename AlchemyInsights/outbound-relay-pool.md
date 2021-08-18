---
title: Pool di inoltro in uscita
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: 7e5bb1fda1dec0c0f72d1944d54b6f2747a6e909
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326081"
---
# <a name="outbound-relay-pool"></a>Pool di inoltro in uscita

Microsoft apporta alcune modifiche alla configurazione per l'inoltro o l'inoltro della posta elettronica tramite Microsoft 365. I messaggi in determinati scenari vengono inoltrati o inoltrati tramite Microsoft 365 utilizzando uno speciale pool di inoltro. I messaggi inviati utilizzando il pool di inoltro potrebbero finire nella cartella posta indesiderata del destinatario. Per ulteriori informazioni, vedere [Outbound delivery pools](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Per evitare uno scenario che utilizza il pool di inoltro, assicurarsi che i messaggi inoltrati/inoltrati soddisfino uno dei criteri seguenti:

- Il mittente in uscita è un dominio accettato del tenant.
- Sender Policy Framework (SPF) passa quando il messaggio Microsoft 365.
- DomainKeys Identified Mail (DKIM) nel dominio del mittente P2 passa quando il messaggio Microsoft 365.
 
I messaggi che soddisfano i criteri precedenti non vengono inoltrati tramite il pool di inoltro.

Se il record MX per il dominio fa riferimento a un server di terze parti o locale, utilizzare il filtro avanzato per verificare che la convalida SPF sia corretta per la posta elettronica in ingresso ed evitare di inviare posta elettronica tramite il pool di inoltro.

**Come è possibile determinare se il pool di inoltro è in grado di influire su di noi?**

Se i messaggi di posta elettronica inoltrati o inoltrati utilizzano uno dei criteri precedenti, i messaggi non verranno inoltrati tramite il pool di inoltro. Tuttavia, se un messaggio viene inviato tramite un pool di inoltro, l'IP del server in uscita si trova nell'intervallo 40.95.0.0/16 e il nome del server in uscita include **rly** nel nome.

