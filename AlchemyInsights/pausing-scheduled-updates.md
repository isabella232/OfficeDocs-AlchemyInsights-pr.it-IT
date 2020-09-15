---
title: Sospensione degli aggiornamenti programmati
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 13abc7c9201b1897a9c766add4d105ef12f0d66f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721559"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="88f51-102">Sospensione degli aggiornamenti programmati</span><span class="sxs-lookup"><span data-stu-id="88f51-102">Pausing scheduled updates</span></span>

<span data-ttu-id="88f51-103">Quando viene emesso un comando di pausa, i dispositivi non elaborano il comando fino al successivo accesso in Intune.</span><span class="sxs-lookup"><span data-stu-id="88f51-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="88f51-104">Per questo motivo, i dispositivi potrebbero:</span><span class="sxs-lookup"><span data-stu-id="88f51-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="88f51-105">Aver installato gli aggiornamenti programmati prima dell'accesso.</span><span class="sxs-lookup"><span data-stu-id="88f51-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="88f51-106">Essere stati spenti quando è stato emesso il comando di pausa.</span><span class="sxs-lookup"><span data-stu-id="88f51-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="88f51-107">In questo caso, quando i dispositivi sono stati accesi, potrebbero aver scaricato e installato gli aggiornamenti programmati prima dell'accesso.</span><span class="sxs-lookup"><span data-stu-id="88f51-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>