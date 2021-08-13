---
title: Ritiro dei servizi di accesso
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938699"
---
# <a name="access-services-retirement"></a>Ritiro dei servizi di accesso

Come abbiamo annunciato in origine in MC97576, a marzo 2017, e abbiamo continuato a comunicare nell'ultimo anno Access Services sono stati ritirati. La fase successiva di questo processo sarà la rimozione dei database Web di Access che utilizzano SharePoint come archivio dati sottostante.

**In che modo ciò influisce su di me?**

A partire da giugno 2019, verrà interrotta la creazione di nuovi database di Access in SharePoint Online e il servizio e tutte le altre app verranno arrestate entro aprile 2020.

**Cosa è necessario fare per prepararsi a questa modifica?**

Si consiglia di creare un piano di transizione per i database Web di Access dell'organizzazione. Gli amministratori possono usare lo [scanner SharePoint App Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) per ottenere un inventario delle app access utilizzate nei siti.

Esistono diversi modi per eseguire la migrazione dei dati dei database Web di Access:

- Importazione in un database di Access locale (. ACCDB) o a un Excel file.
- È inoltre consigliabile esplorare Microsoft PowerApps come piattaforma alternativa per creare soluzioni aziendali senza codice per dispositivi mobili e Web.