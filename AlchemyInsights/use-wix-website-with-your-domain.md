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
ms.openlocfilehash: ef2e7278b1a70aedca1b2ad9c13c249bf8b09c00
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825951"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Utilizzo di un sito Web di Wix con domini acquistati o gestiti da Office 365

- [Aggiornare i record DNS per mantenere il proprio sito Web con l'attuale provider di hosting](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- L'articolo di Wix "Connessione di un dominio a Wix usando il metodo di puntamento" consiglia di usare il puntamento (aggiungere i record DNS, come descritto nel collegamento sopra), anziché cambiare i server dei nomi quando si usa Office 365.
- Se si sceglie di modificare i server dei nomi in Wix, è necessario creare [record DNS in Wix per Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide).
- Se il dominio è stato acquistato da Microsoft, non è possibile modificare i server dei nomi. Se è necessario modificare i server dei nomi, il dominio acquistato Microsoft deve essere [trasferito in un altro provider di hosting dopo 60 giorni](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)