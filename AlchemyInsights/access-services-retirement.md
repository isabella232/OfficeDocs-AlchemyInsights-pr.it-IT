---
title: Pensionamento dei servizi di accesso
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973928"
---
# <a name="access-services-retirement"></a>Pensionamento dei servizi di accesso

Come annunciato originariamente in MC97576, nel marzo 2017, e ha continuato a comunicare negli ultimi anni, i servizi di accesso vengono ritirati da Office 365. La fase successiva di questo processo sarà la rimozione dei database di Access Web che utilizzano gli elenchi di SharePoint come archivio dati sottostante.

## <a name="how-does-this-affect-me"></a>In che modo questo ha effetto su di me?

A partire da giugno 2019, si smetterà di creare nuovi database di Access in SharePoint Online e arrestare il servizio e le eventuali app restanti entro il 2020 aprile.

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a>Che cosa è necessario fare per prepararsi a questa modifica?

Si consiglia di creare un piano di transizione per i database Web di Access dell'organizzazione. Gli amministratori possono utilizzare lo [scanner app di SharePoint Access](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) per ottenere un inventario delle app di Access utilizzate dai siti. 

Esistono diversi modi per eseguire la migrazione dei dati di Access Web database:

- Importazione in un database di Access locale (. ACCDB) o in un file di Excel.
- È inoltre consigliabile esplorare Microsoft PowerApps come piattaforma alternativa per creare soluzioni aziendali senza codice per dispositivi mobili e Web.