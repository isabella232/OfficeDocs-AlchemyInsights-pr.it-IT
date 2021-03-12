---
title: Set di repliche
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50716272"
---
# <a name="replica-set"></a>Set di repliche

AADDS viene chiamato anche come dominio gestito. Si tratta in realtà di due controller di dominio eseguiti e gestiti dal back-end. I due controller di dominio includono un controller di dominio principale e un controller di dominio di replica. I backup in AADDS (dominio gestito) sono processi automatizzati gestiti dalla piattaforma Azure. In caso di un problema con il dominio gestito, il supporto di Azure può essere di aiuto nel ripristino dal backup.

Ogni set di repliche viene creato in una rete virtuale. Ogni rete virtuale deve essere peered a ogni altra rete virtuale che ospita il set di repliche di un dominio gestito. Questa configurazione crea una topologia di rete mesh che supporta la replica della directory. Una rete virtuale può supportare più set di repliche, purché ogni set di repliche si trova in una subnet virtuale diversa.

Per ulteriori informazioni sul set di repliche, vedere [Concepts Replica sets.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
