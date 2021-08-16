---
title: Esportare i risultati di eDiscovery/Ricerca contenuto
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7221"
ms.openlocfilehash: de5d6f2bbf32ca1b7a0bbb9dd416fb19186d2e72ad57fbf25d9b55bd733fdc21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988110"
---
# <a name="export-ediscoverycontent-search-results"></a>Esportare i risultati di eDiscovery/Ricerca contenuto

Potrebbe essere necessario esportare i risultati della ricerca in un file PST (dalla posta elettronica) o in documenti Office nativi (da SharePoint e OneDrive for Business siti). Se sì, procedere come segue:

- Assicurati che all'account siano assegnate le autorizzazioni appropriate per l'esportazione. Per altre info, vedi [Assegnare l'autorizzazione di eDiscovery.](https://go.microsoft.com/fwlink/?linkid=2102406)
- Verificare che il computer abbia soddisfatto tutti [i prerequisiti](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin). Non tutti i browser sono supportati, ad esempio Chrome.
- Per esportare da una ricerca contenuto: a. Passare al [Centro sicurezza & conformità](https://protection.office.com/contentsearch) e fare clic su **Ricerca** e quindi selezionare Ricerca **contenuto**. Nella pagina **Ricerca contenuto** selezionare una ricerca salvata.
    b. Nel riquadro Dettagli, in **Esporta risultati in un computer,** selezionare Avvia **esportazione.** Se si esportano più di 100.000 cassette postali, sarà necessario utilizzare PowerShell per scaricare i risultati dell'esportazione. Per altre info, vedi [Esportazione di risultati da più di 100.000 cassette postali.](https://go.microsoft.com/fwlink/?linkid=2143861)

Per ulteriori informazioni, vedere [Export Content Search Results.](https://go.microsoft.com/fwlink/?linkid=2102118)