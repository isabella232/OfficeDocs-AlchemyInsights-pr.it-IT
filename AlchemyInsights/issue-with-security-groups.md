---
title: Problemi con i gruppi di sicurezza
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162944"
---
# <a name="issue-with-security-groups"></a>Problemi con i gruppi di sicurezza

**Se si riceve un errore di rete AADDS104**

Le regole non valide dei gruppi di sicurezza di rete sono la causa più comune degli errori di rete per Servizi di dominio Azure Active Directory (AD DS). Il gruppo di sicurezza di rete per la rete virtuale deve consentire l'accesso a porte e protocolli specifici. Se queste porte sono bloccate, la piattaforma Azure non può monitorare o aggiornare il dominio gestito. Ha anche effetto sulla sincronizzazione tra Azure AD e Azure AD DS. Assicurarsi di tenere aperte le porte predefinite per evitare interruzioni del servizio.

Per comprendere e risolvere gli avvisi comuni per i problemi di configurazione dei gruppi di sicurezza di rete, vedere [Aggiungere e verificare i gruppi di sicurezza](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).
