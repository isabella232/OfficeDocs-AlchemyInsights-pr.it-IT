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
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529274"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="d1104-102">Risoluzione dei problemi relativi al certificato di firma SAML</span><span class="sxs-lookup"><span data-stu-id="d1104-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="d1104-103">Per risolvere i problemi con il certificato di firma SAML, è consigliabile eseguire i passaggi seguenti:</span><span class="sxs-lookup"><span data-stu-id="d1104-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="d1104-104">Quando si aggiunge un'applicazione aziendale che supporta Single Sign-On, Azure genera un certificato denominato [Certificato di firma SAML ](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span><span class="sxs-lookup"><span data-stu-id="d1104-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="d1104-105">La data di scadenza del certificato è di 3 anni.</span><span class="sxs-lookup"><span data-stu-id="d1104-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="d1104-106">Per modificare la data di scadenza del certificato, vedere [Personalizzare la data di scadenza per il certificato della federazione e implementarla nel nuovo certificato](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span><span class="sxs-lookup"><span data-stu-id="d1104-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="d1104-107">Azure userà questo certificato per firmare i token SAML richiesti dall'applicazione e per inviarli all'applicazione per ottenere un Single Sign-On corretto.</span><span class="sxs-lookup"><span data-stu-id="d1104-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="d1104-108">Per completare il processo, scaricare il certificato dal portale di Azure e inviarlo al fornitore dell'applicazione per completare il processo SSO.</span><span class="sxs-lookup"><span data-stu-id="d1104-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="d1104-109">Al termine, l'applicazione considererà attendibile questo certificato e accetterà tutti i token SAML firmati dal certificato.</span><span class="sxs-lookup"><span data-stu-id="d1104-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="d1104-110">Alla scadenza del certificato, creare un nuovo certificato, aggiornarlo tramite il fornitore dell'applicazione e quindi renderlo attivo sul lato Azure.</span><span class="sxs-lookup"><span data-stu-id="d1104-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="d1104-111">Per altre informazioni, vedere [Rinnovare un certificato con scadenza imminente](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span><span class="sxs-lookup"><span data-stu-id="d1104-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="d1104-112">In caso di scadenza del certificato, l'utente non verrà bloccato.</span><span class="sxs-lookup"><span data-stu-id="d1104-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="d1104-113">[Aggiungere un indirizzo di posta elettronica per le notifiche](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) da ricevere prima della scadenza del certificato corrente.</span><span class="sxs-lookup"><span data-stu-id="d1104-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="d1104-114">Il passaggio 4 è facoltativo.</span><span class="sxs-lookup"><span data-stu-id="d1104-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="d1104-115">Modificare le opzioni di firma del certificato SAML di un'applicazione e l'algoritmo di firma del certificato.</span><span class="sxs-lookup"><span data-stu-id="d1104-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="d1104-116">Per altre informazioni, vedere [Modificare le opzioni di firma del certificato e l'algoritmo di firma](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="d1104-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

