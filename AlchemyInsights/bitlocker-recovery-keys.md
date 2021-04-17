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
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820290"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="0889f-102">Accesso alle chiavi di ripristino di Bitlocker</span><span class="sxs-lookup"><span data-stu-id="0889f-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="0889f-103">Quando si configurano le impostazioni di Bitlocker Intune Endpoint Protection Policy, è possibile definire se le informazioni di ripristino di Bitlocker devono essere archiviate in Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0889f-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="0889f-104">Se questa impostazione è configurata, i dati di ripristino archiviati devono essere visibili a un amministratore di Intune come parte dei dati del record del dispositivo nel pannello Dispositivi intune in due modi:</span><span class="sxs-lookup"><span data-stu-id="0889f-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="0889f-105">Dispositivi - Dispositivi Azure AD -> "Dispositivo" O Dispositivi -> Tutti i dispositivi -> "Dispositivo" -> chiavi di ripristino</span><span class="sxs-lookup"><span data-stu-id="0889f-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="0889f-106">In alternativa, se è disponibile l'accesso amministrativo al dispositivo stesso, è possibile visualizzare la chiave di ripristino (Password) eseguendo il comando seguente da un prompt dei comandi con privilegi elevati:</span><span class="sxs-lookup"><span data-stu-id="0889f-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="0889f-107">Se il dispositivo è stato crittografato prima della registrazione in Intune, la chiave di ripristino potrebbe essere stata associata all'"account Microsoft" (MSA) usato per accedere al dispositivo durante il processo di configurazione guidata.</span><span class="sxs-lookup"><span data-stu-id="0889f-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="0889f-108">In tal caso, l'accesso e l'accesso con tale servizio dovrebbero mostrare i dispositivi per i quali sono state archiviate  https://onedrive.live.com/recoverykey le chiavi di ripristino.</span><span class="sxs-lookup"><span data-stu-id="0889f-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="0889f-109">Se il dispositivo è stato crittografato a seguito della configurazione tramite criteri di gruppo basati su dominio, le informazioni di ripristino possono essere archiviate in Active Directory locale.</span><span class="sxs-lookup"><span data-stu-id="0889f-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="0889f-110">Se sono stati configurati criteri di Endpoint protection per archiviare la chiave di ripristino in Azure Active Directory ma la chiave per un dispositivo specifico non è stata caricata, è possibile attivare il caricamento ruotando la chiave di ripristino per tale dispositivo dalla console MEM.</span><span class="sxs-lookup"><span data-stu-id="0889f-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="0889f-111">Per informazioni dettagliate, vedere [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span><span class="sxs-lookup"><span data-stu-id="0889f-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

