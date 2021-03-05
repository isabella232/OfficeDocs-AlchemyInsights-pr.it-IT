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
ms.openlocfilehash: b93377a33eebc7899041b684449e46caedb04415
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50465010"
---
# <a name="export-ediscoverycontent-search-results"></a>Esportare i risultati di eDiscovery/Ricerca contenuto

Potrebbe essere necessario esportare i risultati della ricerca in un file PST (da posta elettronica) o in documenti di Office nativi (dai siti di SharePoint e OneDrive for Business). Se sì, procedere come segue:

- Assicurati che all'account siano assegnate le autorizzazioni appropriate per l'esportazione. Per altre informazioni, vedere [Assegnare l'autorizzazione di eDiscovery.](https://go.microsoft.com/fwlink/?linkid=2102406)
- Verificare che il computer abbia soddisfatto [tutti i prerequisiti.](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin) Non tutti i browser sono supportati, ad esempio Chrome.
- Per eseguire l'esportazione da una ricerca di contenuto: a. Accedere al [Centro sicurezza & conformità](https://protection.office.com/contentsearch) e fare clic su **Ricerca** e quindi selezionare **Ricerca contenuto.** Nella pagina **Ricerca contenuto** selezionare una ricerca salvata.
    b. Nel riquadro Dei dettagli, in **Esporta risultati in un computer,** selezionare Avvia **esportazione.** Se si esportano più di 100.000 cassette postali, è necessario utilizzare PowerShell per scaricare i risultati dell'esportazione. Per ulteriori informazioni, vedere [Esportazione dei risultati da più di 100.000 cassette postali.](https://go.microsoft.com/fwlink/?linkid=2143861)

Per ulteriori informazioni, vedere [Export Content Search Results.](https://go.microsoft.com/fwlink/?linkid=2102118)