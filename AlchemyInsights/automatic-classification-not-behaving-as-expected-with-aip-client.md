---
title: La classificazione automatica non funziona come previsto con il client di AIP
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
- "4373"
ms.openlocfilehash: d7a2246d78cbd6c4ab40c2a4e5a21807933b619a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715205"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>La classificazione automatica non funziona come previsto con il client di AIP

La classificazione automatica non funziona come previsto; usare le linee guida consigliate seguenti:

1. Se si verificano problemi con l'etichettatura automatica, vedere [Come configurare le condizioni per la classificazione automatica e consigliata per Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) e [Cosa individuano le tipologie di informazioni sensibili](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Verificare se sono utilizzati criteri con ambito non configurati correttamente: [Come configurare i criteri di Azure Information Protection per utenti specifici tramite criteri con ambito](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Se l'etichettatura automatica non funziona per Outlook quando si allega un documento con etichetta, verificare che `DRMEncryptProperty` non sia definito come descritto qui: [Impostazioni IRM del Registro di sistema per la sicurezza](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Se sono stati utilizzati i [tipi di informazioni integrati](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) per i criteri di Azure Information Protection, verificare che il contenuto corrisponda al formato previsto.
5. Verificare che l'etichetta sia configurata in modo appropriato per l'opzione **automatica** o **consigliata**. L'etichettatura **automatica** è disponibile per tutte le app di Microsoft 365, mentre quella **consigliata** è disponibile per tutte le app di Microsoft 365 ad eccezione di Outlook.
6. Non è possibile usare la classificazione automatica per i documenti e i messaggi di posta elettronica in precedenza etichettati manualmente o associati automaticamente a una classificazione superiore.  Per ulteriori informazioni, vedere: [Come vengono applicate le etichette automatiche o consigliate](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Se i problemi persistono, è possibile raccogliere i log del client di Azure Information Protection e allegare i log esportati al ticket di supporto. Per esportare i log di Azure Information Protection:
    - Aprire un documento di Office o creare un nuovo messaggio di posta elettronica in Outlook.
    - Fare clic su **Protezione/Riservatezza** > **Guida e feedback**.
    - Fare clic su **Esporta log**.
    - Salvare i log nella posizione desiderata e allegarli alla richiesta di servizio.

Per ulteriori informazioni, vedere:

- [Come configurare le condizioni per la classificazione automatica e consigliata di Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Guide sulle procedure per scenari comuni che usano Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Consultare la documentazione di Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Controllare le funzionalità e gli abbonamenti di Azure Information Protection](https://azure.microsoft.com/pricing/details/information-protection)
- [Requisiti di Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Guida introduttiva per Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Scaricare il client di Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
