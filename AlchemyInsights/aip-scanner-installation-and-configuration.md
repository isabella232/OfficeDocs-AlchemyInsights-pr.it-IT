---
title: 'Scanner AIP: Installazione e configurazione'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: be5b63ffccd5bbd83e7802e4ef5aa657ed921ae6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686646"
---
# <a name="aip-scanner-installation-and-configuration"></a>Scanner AIP: Installazione e configurazione

**Per installare lo scanner AIP, seguire le linee guida consigliate**:

1. Se si sta eseguendo l'aggiornamento e non viene eseguita un'installazione pulita, accertarsi di aver seguito le linee guida per [aggiornare lo scanner di Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) e per i client di etichetta unificata, vedere [Aggiornamento scanner Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Verificare che l'utente sia conforme con tutti i [Requisiti per i firewall e le impostazioni dell'infrastruttura di rete](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Verificare che i [criteri siano impostati](https://docs.microsoft.com/azure/information-protection/configure-policy) sull'etichettatura automatica o che nel criterio sia presente un'etichetta predefinita.
4. Assicurarsi che il tipo di file pertinente sia configurato per l'etichetta/protezione come descritto in [Tipi di file supportati dal client di Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Inoltre, se si vuole modificare il comportamento predefinito, seguire queste linee guida: [Cambiare il livello di protezione predefinito dei file](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Verificare che l'account utente configurato per l'esecuzione del servizio scanner disponga delle autorizzazioni necessarie per accedere a tutti i repository configurati.
6. Se si verificano ancora problemi, esportare i log di scanner e aggiungerli al ticket di supporto.

**Esportare i log dello scanner di Azure Information Protection**

1. Passare a%localappdata%\Microsoft\MSIP nel contesto utente che sta eseguendo il servizio scanner.
2. Comprimere tutto il contenuto in un file zip nella cartella MSIP.
3. Salvare i log nella posizione desiderata e allegarli alla richiesta di servizio.
4. È anche possibile usare [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Per altre informazioni, vedere**:
- [Distribuzione dello strumento di analisi Azure Information Protection per classificare e proteggere automaticamente i file](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Specificare e usare il parametro token per Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Eseguire un ciclo di individuazione e visualizzare i report per lo scanner](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Consultare la documentazione di Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Requisiti di Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Scaricare il client di Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
