---
title: Pensionamento dei servizi di accesso
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36747788"
---
# <a name="access-services-retirement"></a>Pensionamento dei servizi di accesso

Come annunciato originariamente in MC97576, nel marzo 2017, e ha continuato a comunicare negli ultimi anni, i servizi di accesso vengono ritirati da Office 365. La fase successiva di questo processo sarà la rimozione dei database di Access Web che utilizzano gli elenchi di SharePoint come archivio dati sottostante.

**In che modo questo ha effetto su di me?**

A partire da giugno 2019, si smetterà di creare nuovi database di Access in SharePoint Online e arrestare il servizio e le eventuali app restanti entro il 2020 aprile.

**Che cosa è necessario fare per prepararsi a questa modifica?**

Si consiglia di creare un piano di transizione per i database Web di Access dell'organizzazione. Gli amministratori possono utilizzare lo [scanner app di SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) per ottenere un inventario delle app di Access utilizzate dai siti.

Esistono diversi modi per eseguire la migrazione dei dati di Access Web database:

- Importazione in un database di Access locale (. ACCDB) o in un file di Excel.
- È inoltre consigliabile esplorare Microsoft PowerApps come piattaforma alternativa per creare soluzioni aziendali senza codice per dispositivi mobili e Web.