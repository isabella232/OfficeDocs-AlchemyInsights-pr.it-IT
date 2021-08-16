---
title: Regole per la riduzione della superficie di attacco
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 0f2e3d2d2cfa205f95a5d5dc84f7293fbee165a2976248de75a96379becd6925
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072200"
---
# <a name="attack-surface-reduction-rules"></a>Regole per la riduzione della superficie di attacco

L'esclusione di file o cartelle può ridurre in modo grave la protezione fornita dalle regole di riduzione delle superficie di attacco. È consentita l'esecuzione dei file che sarebbero stati bloccati da una regola e non vengono registrati report o eventi. Un'esclusione si applica a tutte le regole che consentono le esclusioni.

Le esclusioni di riduzione della superficie di attacco usano la stessa sintassi delle esclusioni di Antivirus Microsoft Defender. Per informazioni dettagliate, vedere [Configurare e convalidare le esclusioni per le analisi di Antivirus Microsoft Defender](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus). Per evitare problemi, esaminare [Errori comuni da evitare quando si definiscono le esclusioni](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).

Non tutte le regole di riduzione della superficie di attacco supportano le esclusioni. Per verificare se la regola supporta le esclusioni, vedere la tabella [Regole per la riduzione della superficie di attacco](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

## <a name="attack-surface-reduction-rules"></a>Regole per la riduzione della superficie di attacco

La superficie di attacco dell'organizzazione include tutte le aree in cui un utente malintenzionato potrebbe compromettere dispositivi o reti aziendali. Ridurre la superficie di attacco significa proteggere i dispositivi e la rete dell'organizzazione, lasciando agli utenti malintenzionati meno modi per eseguire gli attacchi. Può essere utile configurare regole di riduzione della superficie di attacco in Microsoft Defender per endpoint.

Per altre informazioni, vedere:

- [Eseguire il mapping del GUID della regola ASR al nome](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- Requisiti delle regole ASR:
    - [Windows 10 Pro, versione 1709 o successiva](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise, versione 1709 o successiva](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server, versione 1803 (Canale semestrale) o successiva](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Identificare l'esclusione corretta da applicare

1. Cercare eventID 1121 o 1122 nel log Microsoft-Windows-Windows Defender/Operational.

1. Valutare lo scenario e il contesto dei blocchi e verificare che lo scenario deve essere sbloccato.

1. Leggere il valore Path nei dettagli dell'evento, ovvero il valore che definisce l'esclusione.
    - Rendere l'esclusione il più restrittiva possibile.
    - Applicare un carattere jolly quando necessario, ad esempio sostituire la variabile User.

1. Applicare l'esclusione in base alle esigenze di distribuzione. Per informazioni dettagliate, vedere [Personalizzare regole per la riduzione della superficie di attacco](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).

## <a name="exclusion-is-not-honored"></a>L'esclusione non viene rispettata

1. Determinare se la regola supporta le esclusioni. Per informazioni dettagliate, vedere [Regole per la riduzione della superficie di attacco](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

1. Esaminare le esclusioni applicate e verificare se i dati dell'evento sono relativi a errori di digitazione o a caratteri jolly non interpretati correttamente. Per altre informazioni, vedere i [Tipi di esclusione supportati](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. Se l'impatto della regola è troppo elevato, è consigliabile riportare la regola in modalità di controllo per eseguire ulteriori convalide. Per informazioni dettagliate, vedere [Verificare il funzionamento delle funzionalità di Microsoft Defender per endpoint in modalità di controllo](/microsoft-365/security/defender-endpoint/audit-windows-defender).

1. Raccogliere dati di supporto per aprire un caso di supporto usando questo comando:
    
   ** MDEClientAnalyzer.cmd -v**

    Per altre informazioni, vedere [Problemi con l’onboarding delle macchine a Microsoft Defender per endpoint](issues-with-onboarding-machines.md).
