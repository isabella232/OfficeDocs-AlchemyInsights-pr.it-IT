---
title: Distribuzione degli oggetti Criteri di gruppo
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067844"
---
# <a name="gpo-deployment"></a>Distribuzione degli oggetti Criteri di gruppo

Le impostazioni per gli oggetti utente e computer in Azure Active Directory Domain Services (Azure AD DS) sono spesso gestite con oggetti Criteri di gruppo. Azure AD DS include oggetti Criteri di gruppo predefiniti per i contenitori Utenti AAD DC e Computer AAD DC. È possibile personalizzare questi oggetti Criteri di gruppo predefiniti per configurare criteri di gruppo in base alle esigenze dell'ambiente in uso. I membri del gruppo di amministratori di Azure AD DC hanno privilegi di amministrazione dei criteri di gruppo nel dominio Azure AD DS e possono anche creare unità organizzative e oggetti Criteri di gruppo personalizzati. Per ulteriori informazioni sul funzionamento e sul funzionamento di Criteri di gruppo, vedere [Group Policy Overview.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

In un ambiente ibrido i criteri di gruppo configurati in un ambiente AD DS locale non vengono sincronizzati con Azure AD DS. Per definire le impostazioni di configurazione per utenti o computer in Azure AD DS, modificare uno degli oggetti Criteri di gruppo predefiniti oppure creare un oggetto Criteri di gruppo personalizzato.

L'articolo sulla [gestione di Criteri di gruppo](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) illustra come installare gli strumenti Gestione Criteri di gruppo, come modificare gli oggetti Criteri di gruppo predefiniti e come creare oggetti Criteri di gruppo personalizzati.
