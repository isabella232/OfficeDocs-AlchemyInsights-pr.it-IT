---
title: Sincronizzazione del servizio di dominio
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
ms.openlocfilehash: 95b5c3b768caf4b5d80a088a17a33facb39805fc766e4888586ae052d91681e3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057862"
---
# <a name="domain-service-synchronization"></a>Sincronizzazione del servizio di dominio

Gli oggetti e le credenziali in un dominio gestito di Servizi di dominio Azure Active Directory (Azure AD DS) possono essere creati localmente nel dominio o sincronizzati da un tenant di Azure Active Directory (Azure AD). Quando si distribuisce per la prima volta Azure AD DS, viene configurata e avviata una sincronizzazione unidirezionale automatica per replicare gli oggetti da Azure AD. Questa sincronizzazione unidirezionale continua a essere eseguita in background per mantenere aggiornato il dominio gestito di Azure AD DS con eventuali modifiche da Azure AD. Non viene eseguita alcuna sincronizzazione da Azure AD DS ad Azure AD.

Per ulteriori dettagli sulla sincronizzazione Azure Active Directory del servizio di dominio, vedere [Domain Service Synchronization.](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization) 
