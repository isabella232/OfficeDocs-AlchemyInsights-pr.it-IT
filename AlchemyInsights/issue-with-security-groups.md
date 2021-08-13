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
ms.openlocfilehash: d8a3c011a3a7cba6c0b1cd00ac0eb587b75bbb5b06d96ef9fd75313734e74fd0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925745"
---
# <a name="issue-with-security-groups"></a>Problemi con i gruppi di sicurezza

**Se si riceve un errore di rete AADDS104**

Le regole non valide dei gruppi di sicurezza di rete sono la causa più comune degli errori di rete per Servizi di dominio Azure Active Directory (AD DS). Il gruppo di sicurezza di rete per la rete virtuale deve consentire l'accesso a porte e protocolli specifici. Se queste porte sono bloccate, la piattaforma Azure non può monitorare o aggiornare il dominio gestito. Ha anche effetto sulla sincronizzazione tra Azure AD e Azure AD DS. Assicurarsi di tenere aperte le porte predefinite per evitare interruzioni del servizio.

Per comprendere e risolvere gli avvisi comuni per i problemi di configurazione dei gruppi di sicurezza di rete, vedere [Aggiungere e verificare i gruppi di sicurezza](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).
