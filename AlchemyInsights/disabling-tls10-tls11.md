---
title: Disabilitazione di TLS1.0 e TLS 1.1 per l'invio del client SMTP AUTH
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13649"
- "9005383"
ms.openlocfilehash: 6751f4e8a177958fdec674899606252a4ae40a72
ms.sourcegitcommit: d9e6f700cd73a61c109e2a99bc71e559dba34722
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/18/2021
ms.locfileid: "58380673"
---
# <a name="disabling-tls10-and-tls-11-for-smtp-auth-client-submission"></a>Disabilitazione di TLS1.0 e TLS 1.1 per l'invio del client SMTP AUTH

Recentemente abbiamo iniziato a disabilitare TLS1.0 e TLS 1.1 per l'invio del client SMTP AUTH. 

Se è stato configurato un dispositivo, un'applicazione o un server che invia posta elettronica a Microsoft 365 usando il metodo di invio del client SMTP AUTH, verificare che il dispositivo, l'applicazione o il server supporti TLS 1.2 per SMTP. 