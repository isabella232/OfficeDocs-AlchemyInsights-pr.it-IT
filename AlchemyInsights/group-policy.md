---
title: Criteri di gruppo
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 02/15/2021
ms.locfileid: "50243918"
---
# <a name="group-policy"></a>Criteri di gruppo

Le impostazioni per gli oggetti utente e computer in Azure Active Directory Domain Services (Azure AD DS) sono spesso gestite con oggetti Criteri di gruppo. Azure AD DS include oggetti Criteri di gruppo predefiniti per i contenitori Utenti AAD DC e Computer AAD DC. È possibile personalizzare questi oggetti Criteri di gruppo predefiniti per configurare criteri di gruppo in base alle esigenze dell'ambiente in uso. I membri del gruppo di amministratori di Azure AD DC hanno privilegi di amministrazione dei criteri di gruppo nel dominio Azure AD DS e possono anche creare unità organizzative e oggetti Criteri di gruppo personalizzati. Per altre informazioni sui criteri di gruppo e sul relativo funzionamento, vedere la [panoramica di Criteri di gruppo](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

In un ambiente ibrido i criteri di gruppo configurati in un ambiente AD DS locale non vengono sincronizzati con Azure AD DS. Per definire le impostazioni di configurazione per utenti o computer in Azure AD DS, modificare uno degli oggetti Criteri di gruppo predefiniti oppure creare un oggetto Criteri di gruppo personalizzato.

L'articolo sulla [gestione di Criteri di gruppo](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) illustra come installare gli strumenti Gestione Criteri di gruppo, come modificare gli oggetti Criteri di gruppo predefiniti e come creare oggetti Criteri di gruppo personalizzati.



