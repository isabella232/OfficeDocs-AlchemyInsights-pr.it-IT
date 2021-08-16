---
title: Configurazione virtuale con Azure Active Directory Domain Services
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 03a6ec63ba8e2779b0fe3f0381606af2c0748f8b848baaa7cd88b61317bd7a5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072848"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Configurazione virtuale con Azure Active Directory Domain Services

La configurazione virtuale con Azure Active Directory Domain Services comporta i seguenti passaggi: 

1. Controllo dell'integrità del dominio sul portale di Azure https://aka.ms/aadds-health
2. Controllo del gruppo di sicurezza di rete per rilevare la presenza di eventuali regole che bloccano le porte necessarie per la sincronizzazione in Azure Active Directory Domain Services sul portale https://aka.ms/aadds-networking
3. Verifica che la rete virtuale sia stata distribuita nella stessa area di Azure come dominio gestito da Azure Active Directory Domain Services.
4. Verifica che non siano presenti domini disponibili nella rete con lo stesso nome dominio.

Per ulteriori considerazioni sulla progettazione sulla rete virtuale di Azure a supporto di Azure Active Directory Domain Services, vedere [Considerazioni sulla rete virtuale](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

