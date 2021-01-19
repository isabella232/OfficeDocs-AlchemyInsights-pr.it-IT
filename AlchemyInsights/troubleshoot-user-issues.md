---
title: Risolvere i problemi relativi all'utente
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886854"
---
# <a name="announcements"></a>Annunci

Seguire le linee guida di Google sulla verifica della compatibilità per rilevare se le applicazioni sono interessate. Le linee guida di Google sono disponibili in https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support.

Verificare che si stia utilizzando la Webview di sistema o il browser di sistema durante l'accesso degli utenti con gli account utente Google. Per ulteriori informazioni, vedere [Problemi durante l'accesso alle applicazioni solo tramite il browser Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).


**Impossibile creare un nuovo utente nella directory Azure AD**

Per risolvere il problema relativo all'impossibilità di creare un nuovo utente in Azure AD, seguire questi passaggi:

1. Verificare che si disponga dell'autorizzazione per creare un nuovo utente standard. Solo chi dispone del ruolo di amministratore globale o amministratore utente in Azure Active Directory (AD) può creare un nuovo utente standard. Se non di dispone di uno dei ruoli di cui sopra, chiedere a un amministratore di essere aggiunto a uno di questi ruoli o di creare un nuovo account utente.
2. Verificare che il nome utente sia in un dominio verificato in Azure AD. Se non si dispone di un nome dominio verificato personalizzato in Azure AD, è possibile usare il dominio Azure AD iniziale, che termina con *.onmicrosoft.com.
3. Verificare che il nome utente sia in un dominio non federato ad Azure AD dall'istanza locale di AD. Gli utenti non possono essere aggiunti nel cloud con i nomi di dominio federati da istanze locali.
4. Verificare che nessun altro utente o contatto disponga già del nome utente che si desidera assegnare al nuovo utente. I nomi utente devono essere univoci in Azure AD.
5. Vedere [Ruoli e amministratori Azure AD](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) per la propria istanza di Azure AD.
6. Vedere i [nomi di dominio](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) per la propria istanza di Azure AD.
7. Rivedere [Log di audit](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) per ulteriori informazioni su un utente creato o eliminato di recente, come chi abbia eseguito un'azione e quando.
8. Per ulteriori informazioni sull'aggiunta di nuovi utenti, vedere [Usare il portale di Microsoft Azure per creare un nuovo utente nella propria istanza di Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) .
9. Per ulteriori informazioni sulle autorizzazioni del ruolo di amministratore in Azure AD, vedere [Ruoli di amministratore in Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).
10. Per informazioni sulla creazione di un utente tramite Azure AD Powershell, vedere [Azure AD PowerShell per creare un nuovo utente](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).

**Problema con la registrazione in modalità self-service**

Per risolvere i problemi relativi alla registrazione in modalità self-service, seguire questi passaggi:

1. Per usare la registrazione in modalità self-service alle applicazioni, abilitare per prima cosa la registrazione in modalità self-service per il tenant. 
2. Per fare in modo che un'applicazione supporti la registrazione in modalità self-service, aggiungerla al flusso utente. Alla visita successiva alla pagina di accesso verrà visualizzata un'opzione **_Nessun account? Creane uno!_* _. Questo messaggio avvia il processo di registrazione self-service.
3. Per informazioni su come inserire i dati di un'organizzazione tramite la registrazione in modalità self-service in Azure AD, vedere [Registrazione in modalità self-service per Azure AD](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).
4. Una volta associato il flusso utente a una o più applicazioni, gli utenti che visitano tale applicazione potranno registrarsi e ottenere un account guest usando le opzioni configurate nel flusso utente. Per ulteriori informazioni sulla registrazione e su come ottenere un account guest, consultare [Registrazione in modalità self-service per gli utenti guest](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).

_ *Problema nell'invitare un utente esterno**

Per risolvere i problemi relativi all'invito di un utente esterno, seguire questi passaggi:

Verificare di aver inviato un invito all'utente all'indirizzo di posta elettronica che corrisponde al nome con cui l'utente ha effettuato l'accesso. Se si invia l'invito all'indirizzo di posta elettronica proxy, l'utente non può riscattarlo. Per ulteriori informazioni, vedere [Documentazione B2B di Azure AD](https://docs.microsoft.com/azure/active-directory/external-identities/).

**Impossibile assegnare licenze a un utente**

Per risolvere i problemi relativi all'assegnazione delle licenze a un utente, seguire questi passaggi:

1. Per gestire le licenze utente, verificare di usare un account che disponga di uno dei ruoli di amministratore richiesti: amministratore globale, amministratore delle licenze o amministratore utente. È possibile verificare il ruolo utente nella scheda **Ruolo della directory** nel pannello utente.
2. Se si sta usando il portale di Microsoft Azure e l'assegnazione della licenza non è andata a buon fine, fare clic sulla notifica nell'angolo in alto a destra. Questa operazione apre un pannello con le informazioni sugli eventuali errori riscontrati. Nella maggior parte dei casi questo basta per comprendere e risolvere il problema.
3. Prima di poter assegnare una licenza a un utente, verificare che sia impostata la proprietà **Località di utilizzo** per l'utente. Verificare che sia stata impostata quella proprietà per l'utente visualizzando la scheda **Profilo** nel pannello utente.
4. Verificare che siano disponibili sufficienti licenze per il prodotto che si sta cercando di assegnare. È possibile visualizzare il numero di licenze disponibili nel portale di Azure, qui [Azure Active Directory -> Licenze -> Tutti i prodotti](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).
5. L'utente potrebbe disporre di un'altra licenza, i cui servizi sono in conflitto con quelli presenti nella nuova licenza che si sta cercando di assegnare. Ad esempio, se l'utente dispone del servizio Exchange Online (Piano 1) abilitato, non potrà assegnare una licenza con Exchange Online (Piano 2). Disabilitare uno dei servizi per consentire l'assegnazione della nuova licenza. Se si sta usando il portale di Azure o i cmdlet di PowerShell, la pagina **dettagli problema** elenca i servizi specifici che stanno causando il conflitto.
6. Se si sta cercando di rimuovere una licenza e questa operazione non è andata a buon fine, l'utente potrebbe disporre di altre licenze con servizi che dipendono dai servizi che si sta cercando di rimuovere. Se si sta usando il portale di Azure o i cmdlet di PowerShell, il messaggio di errore elencherà i servizi specifici che dispongono di dipendenze.
7. Se si desidera comprendere perché una licenza è stata aggiunta/rimossa da un utente (ad esempio, chi nell'organizzazione possa avere apportato modifiche), verificare i log di audit. Impostare il filtro su **Attività licenza** per mostrare tutte le modifiche, incluso l'"attore" che le ha eseguite.
8. Se si sta usando Exchange Online, alcuni utenti nel tenant potrebbero essere configurati in modo non corretto con lo stesso valore dell'indirizzo proxy. In questi casi, si potrebbero visualizzare messaggi di errore generici quando un'operazione relativa a una licenza non va a buon fine. [Questo articolo](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) contiene ulteriori informazioni su questo problema, incluse informazioni su [come connettersi a Exchange Online tramite una sessione remota di PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell). Per identificare quali utenti nel tenant, contenere lo stesso indirizzo proxy, eseguire questo cmdlet di Exchange Online:

Esegui

Get-Recipient | where {$_.EmailAddresses -match <user principal name>} | fL Name, RecipientType,emailaddresses





