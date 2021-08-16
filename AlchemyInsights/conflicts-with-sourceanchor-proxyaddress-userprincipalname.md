---
title: Conflitti con SourceAnchor, ProxyAddress, UserPrincipalName
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 2d58078fcabb416c418b67a2f2ce2eba679a18c6ecf3846c534bde74188d7827
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033066"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a>Conflitti con SourceAnchor, ProxyAddress, UserPrincipalName

Se durante una sincronizzazione si ricevono errori simili a "Nella directory esiste già un oggetto sincronizzato con lo stesso valore di ProxyAddress o UserPrincipalName", vedere [Diagnosticare e risolvere gli errori di sincronizzazione degli attributi duplicati](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).

Inoltre, è consigliabile abilitare la resilienza degli attributi duplicati. Per altre informazioni, vedere [Sincronizzazione delle identità e resilienza degli attributi duplicati](https://aka.ms/duplicateattributeresiliency).