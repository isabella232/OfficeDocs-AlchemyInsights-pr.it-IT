---
title: Chiavi di ripristino di BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685890"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Accesso alle chiavi di ripristino di BitLocker

Quando si configurano i criteri di protezione dell'endpoint di configurazione di BitLocker, è possibile definire se le informazioni di ripristino di BitLocker devono essere archiviate in Azure Active Directory.

Se tale impostazione è configurata, i dati di ripristino archiviati devono essere visibili a un amministratore di Intune come parte dei dati del record del dispositivo nel Blade dei dispositivi Intune in due modi:

Devices-Azure AD Devices-> "dispositivo" o dispositivi-> tutti i dispositivi-> "dispositivo"-tasti di ripristino >

In alternativa, se è presente un accesso amministrativo al dispositivo stesso, il tasto di ripristino (password) può essere visualizzato eseguendo il comando seguente da un prompt dei comandi con privilegi elevati:

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
Se il dispositivo è stato crittografato prima dell'iscrizione in Intune, è possibile che la chiave di ripristino sia stata associata all'account Microsoft (MSA) utilizzato per accedere al dispositivo durante il processo di configurazione. In tal caso, l'accesso e la  https://onedrive.live.com/recoverykey firma di MSA devono mostrare i dispositivi per i quali sono state archiviate le chiavi di ripristino.
 
Se il dispositivo è stato crittografato in seguito alla configurazione tramite criteri di gruppo basati sul dominio, è possibile che le informazioni di ripristino vengano archiviate in Active Directory locale.
 

