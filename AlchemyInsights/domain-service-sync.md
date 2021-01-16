---
title: Sincronizzazione dei servizi di dominio
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876517"
---
# <a name="domain-service-synchronization"></a>Sincronizzazione dei servizi di dominio

Gli oggetti e le credenziali di un dominio gestito di Azure Active Directory (Azure AD DS) possono essere creati localmente all'interno del dominio oppure sincronizzati da un tenant di Azure Active Directory (Azure AD). Quando si distribuisce Azure AD DS per la prima volta, viene configurata e avviata una sincronizzazione automatica unidirezionale per replicare gli oggetti da Azure AD. Questa sincronizzazione unidirezionale continua a essere eseguita in background per mantenere il dominio gestito di Azure AD DS aggiornato con le modifiche apportate da Azure AD. Nessuna sincronizzazione si verifica da Azure AD DS di nuovo ad Azure AD.

Per ulteriori informazioni sulla sincronizzazione dei servizi di dominio di Azure Active Directory, vedere [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization). 
