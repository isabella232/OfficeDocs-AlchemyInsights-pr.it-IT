---
title: Supporto di Microsoft Edge per la protezione delle applicazioni Microsoft Defender
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576548"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Supporto di Microsoft Edge per la protezione delle applicazioni Microsoft Defender

Progettata per Windows 10 e Microsoft Edge, Application Guard utilizza un approccio di isolamento hardware che consente a un utente di accedere a un sito non attendibile dall'interno di un contenitore isolato, Hyper-V abilitato, separato dal sistema operativo host.

Un amministratore dell'organizzazione definisce un elenco di siti attendibili, risorse cloud e reti interne. Quando un utente visita un sito non presente nell'elenco, Microsoft Edge aprirà il sito nel contenitore. Ciò significa che se il sito risulta essere dannoso, il PC host rimarrà protetto e l'utente malintenzionato non otterrà i dati dell'organizzazione.

L'installazione delle estensioni nel contenitore è supportata da Microsoft Edge versione 81 e può essere controllata tramite un criterio. L'indirizzo updateURL utilizzato nei criteri di ExtensionInstallForcelist deve essere aggiunto come risorsa neutra nei criteri di isolamento della rete utilizzati dalla protezione dell'applicazione.

Per altre informazioni, vedere [supporto Microsoft Edge per Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).
