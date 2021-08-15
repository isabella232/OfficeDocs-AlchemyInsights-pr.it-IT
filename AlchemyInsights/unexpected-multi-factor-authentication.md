---
title: Autenticazione a più fattori imprevista
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: d2b97175049bd9732b7444b029f7ea8610c3d5a2c02878ec5f20ded916baadd5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53991143"
---
# <a name="unexpected-multi-factor-authentication"></a>Autenticazione a più fattori imprevista

Se il tenant è stato creato dopo il 21 ottobre 2019 e si riceve una richiesta di conferma per l'autenticazione a più fattori, è probabile che siano state abilitate le [impostazioni predefinite per la sicurezza](https://aka.ms/securitydefaults) nel tenant. 

Per gestire le impostazioni predefinite per la sicurezza:

1. Accedere all'[interfaccia di amministrazione](https://go.microsoft.com/fwlink/p/?linkid=834822) con le credenziali di amministratore globale.

2. Passare alle [Proprietà di Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).

3. Nella parte inferiore della pagina fare clic su **Gestire le impostazioni predefinite per la sicurezza**.

4. Fare clic su **Sì** per abilitare le impostazioni predefinite di sicurezza e su **No** per disabilitare le impostazioni predefinite per la sicurezza.
