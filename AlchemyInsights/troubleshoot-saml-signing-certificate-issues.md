---
title: Risoluzione dei problemi relativi al certificato di firma SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: fb043122edf5f99325f0403810eb0dc119d254e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314424"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Risoluzione dei problemi relativi al certificato di firma SAML

Per risolvere i problemi con il certificato di firma SAML, è consigliabile eseguire i passaggi seguenti:

1. Quando si aggiunge un'applicazione aziendale che supporta Single Sign-On, Azure genera un certificato denominato [Certificato di firma SAML ](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications). La data di scadenza del certificato è di 3 anni. Per modificare la data di scadenza del certificato, vedere [Personalizzare la data di scadenza per il certificato della federazione e implementarla nel nuovo certificato](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).
2. Azure userà questo certificato per firmare i token SAML richiesti dall'applicazione e per inviarli all'applicazione per ottenere un Single Sign-On corretto. Per completare il processo, scaricare il certificato dal portale di Azure e inviarlo al fornitore dell'applicazione per completare il processo SSO.

Al termine, l'applicazione considererà attendibile questo certificato e accetterà tutti i token SAML firmati dal certificato.

3. Alla scadenza del certificato, creare un nuovo certificato, aggiornarlo tramite il fornitore dell'applicazione e quindi renderlo attivo sul lato Azure. Per altre informazioni, vedere [Rinnovare un certificato con scadenza imminente](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).

**Nota**: in caso di scadenza del certificato, l'utente non verrà bloccato.

4. [Aggiungere un indirizzo di posta elettronica per le notifiche](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) da ricevere prima della scadenza del certificato corrente.

**Nota**: Il passaggio 4 è facoltativo.

5. Modificare le opzioni di firma del certificato SAML di un'applicazione e l'algoritmo di firma del certificato. Per altre informazioni, vedere [Modificare le opzioni di firma del certificato e l'algoritmo di firma](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).

