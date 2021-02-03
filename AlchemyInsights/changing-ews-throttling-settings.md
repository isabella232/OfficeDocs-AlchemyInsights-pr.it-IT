---
title: Modificare le impostazioni della limitazione EWS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075901"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="6d326-102">Modificare le impostazioni della limitazione EWS</span><span class="sxs-lookup"><span data-stu-id="6d326-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="6d326-103">Eseguire il test automatico che consente di modificare i criteri di limitazione EWS per la durata della migrazione.</span><span class="sxs-lookup"><span data-stu-id="6d326-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="6d326-104">Tenere presente che, anche dopo l'esecuzione, le importazioni di EWS saranno comunque limitate a 150 MB ogni 5 minuti per cassetta postale. Per ottenere velocità di migrazione più elevate, eseguire simultaneamente la migrazione di più utenti.</span><span class="sxs-lookup"><span data-stu-id="6d326-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="6d326-105">Si prega di notare che le modifiche apportate ai criteri di limitazione EWS non hanno alcun effetto sui seguenti tipi di trasferimenti (in caso di utilizzo di strumenti Microsoft): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Cartelle Pubbliche o il Servizio d’importazione PST.</span><span class="sxs-lookup"><span data-stu-id="6d326-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>