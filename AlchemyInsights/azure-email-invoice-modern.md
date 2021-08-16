---
title: Fatturazione moderna di Azure tramite posta elettronica
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: caf300873c3a9a97502819c7938ecc86491795d2fc7b6f022ead5d38ca965b8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082838"
---
# <a name="email-invoicing-in-azure"></a>Fatturazione di Azure tramite posta elettronica

Per aggiornare le preferenze per la fatturazione tramite posta elettronica, è necessario disporre del ruolo di proprietario o collaboratore nel profilo o nell'account di fatturazione. Dopo aver accettato esplicitamente, tutti gli utenti con il ruolo di proprietario, collaboratore, lettore e responsabile della fatturazione nel profilo di fatturazione riceveranno la fattura tramite posta elettronica.

1. Accedere al [portale di Azure](https://portal.azure.com/).
2. Cercare **Gestione costi e fatturazione**.
3. Selezionare **Fatture** nel lato sinistro e quindi selezionare **Fattura per posta elettronica** nella parte superiore della pagina.
4. Se si hanno più profili di fatturazione, selezionare un profilo e quindi selezionare **Acconsento esplicitamente**.

5. Selezionare **Aggiorna**.
6. Se si hanno più profili di fatturazione, selezionare un profilo e quindi selezionare **Acconsento esplicitamente**.

È possibile concedere ad altri utenti l'accesso alla visualizzazione, al download e al pagamento delle fatture assegnando loro il ruolo di responsabile per un profilo di fatturazione MCA o MPA. Se si è scelto di ricevere le fatture tramite posta elettronica, anche gli utenti riceveranno le fatture tramite posta elettronica.

1. Accedere al [portale di Azure](https://portal.azure.com/).
2. Cercare **Gestione costi e fatturazione**.
3. Selezionare **Profili di fatturazione** nel lato sinistro. Nell'elenco dei profili fatturazione, selezionare un profilo per il quale si vuole assegnare un ruolo di responsabile della fatturazione.
4. Selezionare **Controllo di accesso (IAM)** nel lato sinistro e quindi selezionare **Aggiungi** nella parte superiore della pagina.

Nell'elenco a discesa Ruolo, selezionare **Responsabile per la fatturazione**. Immettere l'indirizzo di posta elettronica dell'utente a cui si vuole concedere l'accesso. Selezionare **Salva** per assegnare il ruolo.
