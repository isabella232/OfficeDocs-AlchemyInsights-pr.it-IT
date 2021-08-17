---
title: Chiavi di ripristino bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: f71fae0aabda3fc48f20d5ea1e6909475f0c17ff5cdf98b58b1403bd2e291c19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060068"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Accesso alle chiavi di ripristino di Bitlocker

Quando si configurano le impostazioni di Bitlocker Intune Endpoint Protection Criteri, è possibile definire se le informazioni di ripristino di Bitlocker devono essere archiviate in Azure Active Directory.

Se questa impostazione è configurata, i dati di ripristino archiviati devono essere visibili a un amministratore di Intune come parte dei dati del record del dispositivo nel pannello Dispositivi intune in due modi:

Dispositivi - Dispositivi Azure AD -> "Dispositivo" O Dispositivi -> Tutti i dispositivi -> "Dispositivo" -> chiavi di ripristino

In alternativa, se è disponibile l'accesso amministrativo al dispositivo stesso, è possibile visualizzare la chiave di ripristino (Password) eseguendo il comando seguente da un prompt dei comandi con privilegi elevati:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Se il dispositivo è stato crittografato prima della registrazione in Intune, la chiave di ripristino potrebbe essere stata associata all'"account Microsoft" (MSA) usato per accedere al dispositivo durante il processo di configurazione guidata. In tal caso, l'accesso e l'accesso con tale servizio dovrebbero mostrare i dispositivi per i quali sono state archiviate  https://onedrive.live.com/recoverykey le chiavi di ripristino.
 
Se il dispositivo è stato crittografato a seguito della configurazione tramite criteri di gruppo basati su dominio, le informazioni di ripristino possono essere archiviate in Active Directory locale.

Se hai configurato i criteri di Endpoint protection per archiviare la chiave di ripristino in Azure Active Directory ma la chiave per un dispositivo specifico non è stata caricata, puoi attivare il caricamento ruotando la chiave di ripristino per tale dispositivo dalla console MEM. Per informazioni dettagliate, vedere [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).

