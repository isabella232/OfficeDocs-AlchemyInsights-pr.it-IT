---
title: 'AIP: I criteri non funzionano come previsto'
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
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663193"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: I criteri non funzionano come previsto

Azure Information Protection: i criteri non funzionano come previsto; vedere le linee guida consigliate seguenti per vari problemi relativi ai criteri:

1. Se si verificano problemi con i contrassegni visivi, consultare l'articolo che descrive [quando vengono applicati i contrassegni visivi](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Se si verificano problemi con l'etichettatura automatica, consultare [Come configurare le condizioni per la classificazione automatica e consigliata per Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) e [Cosa individuano le tipologie di informazioni sensibili](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Se si verificano problemi con la protezione di file nativi/Pfile, consultare [Configurazione API file](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Verificare se sono utilizzati criteri con ambito non configurati correttamente: [Come configurare i criteri di Azure Information Protection per utenti specifici tramite criteri con ambito](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Se l'etichettatura automatica non funziona per Outlook quando si allega un documento con etichetta, verificare che DRMEncryptProperty non sia definito come descritto qui: [Impostazioni IRM del Registro di sistema per la sicurezza](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Se i problemi persistono, è possibile raccogliere i log del client di Azure Information Protection e allegare i log esportati al ticket.

1. Aprire un documento di Office o creare un nuovo messaggio di posta elettronica in Outlook.
2. Fare clic su **Protezione/Riservatezza** > **Guida e feedback**.
3. Fare clic su **Esporta log**.
4. Salvare i log nella posizione desiderata e allegarli alla richiesta di servizio.

Risorse aggiuntive:

- [Come configurare un'etichetta per contrassegni visivi di Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Consultare la documentazione di Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Usare le etichette di riservatezza nelle app di Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

