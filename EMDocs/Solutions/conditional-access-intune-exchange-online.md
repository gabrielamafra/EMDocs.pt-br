---
# required metadata

title: Usar acesso condicional com o Microsoft Intune e o Exchange Online
description:
keywords:
author: craigcaseyMSFT
manager: swadhwa
ms.date: 04/28/2016
ms.topic: article
ms.prod:
ms.service:
ms.technology:
ms.assetid: 8cfe421b-52c9-4d44-8df1-15c82375c335

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
ms.reviewer: 
ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom:

---

# Implantar o Exchange Online com o Intune

Agora que leu as [diretrizes de arquitetura para proteger emails e documentos da empresa](../Solutions/architecture-guidance-for-protecting-company-email-and-documents.md), você está pronto para prosseguir com a implantação de uma solução.

Para o Intune gerenciar dispositivos móveis diretamente, os usuários precisam registrar os dispositivos no Intune.

## Etapas de Implantação
Siga estas etapas para implantar a solução Exchange Online com Intune:

### Etapa 1: criar políticas de conformidade e implantá-las para os usuários.
As políticas de conformidade definem regras e configurações com que um dispositivo deve manter a conformidade para ser considerado compatível pelas políticas de acesso condicional. Siga as etapas em [Criar uma política de conformidade no Microsoft Intune](https://stage.docs.microsoft.com/en-us/intune/deployuse/create-a-device-compliance-policy-in-microsoft-intune) para criar e implantar políticas de conformidade.

Se você desejar poder remover todos os email corporativo de um dispositivo iOS depois que ele não fizer mais parte da sua empresa, será necessário criar e implantar um perfil de email e, em seguida, definir a política de conformidade que especifica que perfis de email são gerenciados pelo Intune. Você deve implantar o perfil de email para o mesmo conjunto de usuários-alvos desta política de conformidade.

![Captura de tela que mostra a página "Regras" do Assistente para Criar Política de Conformidade, onde é possível especificar que um perfil de email deve ser gerenciado pelo Intune.](./media/ProtectEmail/Hybrid-Onprem-ExchSrvr-Wizard6.PNG)

Se você especificar esta política de conformidade, um usuário que já tenha configurado a conta de email, deverá removê-la manualmente e, em seguida, o Intune a adicionará novamente por meio do processo de registro descrito em [Experiência de usuário final do acesso condicional](../Solutions/end-user-experience-conditional-access.md).

> [!IMPORTANT]
> Se você habilitar a política de acesso condicional do Exchange sem ter antes implantado uma política de conformidade, todos os dispositivos de destino terão o acesso permitido.

### Etapa 2: Avaliar o efeito da política de acesso condicional.
Se tiver configurado uma conexão entre o Intune e o Exchange usando o [Service to Service Connector do Microsoft Intune](https://stage.docs.microsoft.com/en-us/intune/deployuse/intune-service-to-service-exchange-connector), você poderá usar os **Relatórios de Inventário de Dispositivo Móvel** para identificar os clientes de email EAS que serão impedidos de acessar o Exchange depois que você configurar a política de acesso condicional.

Siga as instruções em [Avaliar o efeito da política de acesso condicional](https://stage.docs.microsoft.com/en-us/intune/deployuse/restrict-access-to-exchange-online-with-microsoft-intune#configure-conditional-access) para identificar os usuários que serão afetados pela política de acesso condicional.

### Etapa 3: Configurar grupos de usuários para a política de acesso condicional
Você direciona políticas de acesso condicional a diferentes grupos de usuários de acordo com os tipos de política. Esses grupos contêm os usuários que serão afetados ou que ficarão isentos da política. Quando um usuário é afetado por uma política, cada dispositivo que ele usa deve ser compatível para que possa acessar o email.

Para saber mais, confira [Configurar grupos de usuários para a política de acesso condicional](https://stage.docs.microsoft.com/en-us/intune/deployuse/restrict-access-to-exchange-online-with-microsoft-intune#configure-conditional-access).

### Etapa 4: Configurar a política de acesso condicional.
As políticas de acesso condicional usam o seguinte fluxo para o Exchange Online para decidir se devem permitir ou bloquear os dispositivos.

![Fluxograma que mostra como as políticas de acesso condicional do Exchange Online avaliam se permitem ou bloqueiam dispositivos.](./media/ProtectEmail/conditional-access-8-1.png)

Siga as informações fornecidas em [Configurar a política de acesso condicional](https://stage.docs.microsoft.com/en-us/intune/deployuse/restrict-access-to-exchange-online-with-microsoft-intune#configure-conditional-access) para definir a política de acesso condicional.



## Relatórios

### Monitorar a conformidade e políticas de acesso condicional
Para exibir dispositivos que foram bloqueados no Exchange:

No painel do Intune, clique no bloco **Dispositivos Bloqueados no Exchange** para mostrar o número de dispositivos bloqueados e links para mais informações.
![Captura de tela que mostra o bloco "Dispositivos Bloqueados no Exchange" no painel do Intune.](./media/ProtectEmail/intune-sa-6blocked-devices.PNG)



## Onde ir daqui
Depois que tiver implantado uma solução para proteger emails corporativos e dados de emails em dispositivos móveis, você poderá aprender mais sobre a [experiência de acesso condicional do usuário final](../Solutions/end-user-experience-conditional-access.md). Isso ajudará a preparar você para problemas que possam surgir quando os usuários finais registrarem seus dispositivos específicos.


<!--HONumber=Apr16_HO2-->

