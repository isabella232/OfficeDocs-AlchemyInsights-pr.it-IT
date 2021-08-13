---
title: Utilizzo di un sito Web di Wix con domini acquistati o gestiti da Office 365
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
- "9001516"
- "3582"
ms.openlocfilehash: d7df06d768eabb44bcaee4a7450d16ecdb3395da4cee4810503d3dae358736ab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53980181"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Utilizzo di un sito Web di Wix con domini acquistati o gestiti da Office 365

- [Aggiornare i record DNS per mantenere il proprio sito Web con l'attuale provider di hosting](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- L'articolo di Wix "Connessione di un dominio a Wix usando il metodo di puntamento" consiglia di usare il puntamento (aggiungere i record DNS, come descritto nel collegamento sopra), anziché cambiare i server dei nomi quando si usa Office 365.
- Se si sceglie di modificare i server dei nomi in Wix, è necessario creare [record DNS in Wix per Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide).
- Se il dominio è stato acquistato da Microsoft, non è possibile modificare i server dei nomi. Se è necessario modificare i server dei nomi, il dominio acquistato Microsoft deve essere [trasferito in un altro provider di hosting dopo 60 giorni](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)