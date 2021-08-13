---
title: Configurare il punto di connessione del servizio (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 5ccb55996ccef4b55c8d80de6e35f4ba27e3dfa18dfcaeaf6f6ad1c54b6bb376
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53965969"
---
# <a name="configure-service-connection-point-scp"></a>Configurare il punto di connessione del servizio (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Motivo**: non è possibile leggere l'oggetto SCP e ottenere le informazioni sul tenant di Azure AD
- **Risoluzione**: vedere la sezione [Configurare un punto di connessione del servizio](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Piano di azione**

- Verificare se il dispositivo ha ricevuto l'oggetto Criteri di gruppo per la convalida controllata.
- Verificare che l'oggetto Criteri di gruppo abbia creato le chiavi del Registro di sistema.
- Assicurarsi di aver creato 2 chiavi con l'ID directory e il dominio onmicrosoft.

**Configurare l'impostazione del Registro di sistema sul lato client per SCP**

Usare l'esempio seguente per creare un oggetto Criteri di gruppo per distribuire un'impostazione del Registro di sistema che configura una voce SCP nel Registro di sistema dei dispositivi.

1. Aprire una console Gestione Criteri di gruppo e creare un nuovo oggetto Criteri di gruppo nel dominio.
     - Specificare un nome per l'oggetto Criteri di gruppo appena creato, ad esempio ClientSideSCP

2. Modificare l'oggetto Criteri di gruppo e individuare il percorso seguente: **Configurazione computer > Preferenze > Impostazioni di Windows > Registro di sistema**.

3. Fare clic con il pulsante destro del mouse su **Registro di sistema** e selezionare **Nuovo > Elemento Registro di sistema**.

4. Nella scheda **Generale** configurare gli elementi seguenti:
  
- **Azione**: Aggiorna
    
- **Hive**: HKEY_LOCAL_MACHINE
    
- **Percorso chiave**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Nome valore**: TenantId
    
- **Tipo di valore**: REG_SZ
    
- **Dati valore**: GUID o ID directory dell'istanza di Azure AD. Questo valore si trova nel **portale di Azure > Azure Active Directory > Proprietà > ID directory**
 
- Fare clic su **OK**.
 
5. Fare clic con il pulsante destro del mouse su **Registro di sistema** e selezionare **Nuovo > Elemento Registro di sistema**.

6. Nella scheda **Generale** configurare gli elementi seguenti:
  
- **Azione**: Aggiorna
    
- **Hive**: HKEY_LOCAL_MACHINE
    
- **Percorso chiave**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Nome valore**: TenantName
    
- **Tipo di valore**: REG_SZ
    
- **Dati valore**: nome di dominio verificato se si usa un ambiente federato, ad esempio AD FS. Nome di dominio verificato o nome di dominio onmicrosoft.com, ad esempio contoso.onmicrosoft.com, se si usa un ambiente gestito

- Fare clic su **OK**.

7. Chiudere l'editor per l'oggetto Criteri di gruppo appena creato.

8. Collegare l'oggetto Criteri di gruppo appena creato all'unità organizzativa desiderata contenente i computer aggiunti a un dominio che appartengono alla popolazione di implementazione controllata.

Per altre informazioni, vedere [Convalida controllata di Aggiunta ad Azure AD ibrido - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) e [Risoluzione dei problemi dei dispositivi ibridi aggiunti ad Azure Active Directory | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









