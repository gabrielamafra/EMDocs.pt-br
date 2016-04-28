---
# required metadata

title: Experiência do usuário final para acesso condicional em dispositivos Windows Phone
description:
keywords:
author: craigcaseyMSFT
manager: swadhwa
ms.date: 04/28/2016
ms.topic: article
ms.prod:
ms.service:
ms.technology:
ms.assetid: 3e186dd2-e17c-40d8-b160-48038b2c6593

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
ms.reviewer: 
ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom:

---

# Windows Phone

O processo de registro e as telas que o usuário vê serão um pouco diferentes dependendo da versão do sistema operacional em execução no dispositivo do usuário final.  Este tópico descreve a experiência do usuário final para dispositivos Windows Phone.

## Registro

1.  Se um usuário já estiver registrado no Intune e for compatível, ele não verá nenhuma diferença em dispositivos do Windows: o acesso aos emails continuará normalmente. Os usuários ainda não registrados no Intune receberão um email de quarentena semelhante a este exemplo:

    ![](./media/ProtectEmail/EUX-Windows-quarantineEmail.png)

    A usuário clica em **Comece agora mesmo** para começar a registrar seus dispositivos.

2.  Na tela de Configuração de Acesso da Empresa, o usuário clica em **Iniciar** para começar a configurar seu dispositivo e verificar se ele é compatível.

    ![](./media/ProtectEmail/EUX-Windows1-company-Access-Setup.png)

3.  Na tela Registre Seu Dispositivo, o usuário clica em **Confirmar Registro** para registrar seu dispositivo.

    ![](./media/ProtectEmail/EUX-Windows3-enroll-Device.png)

    Durante o registro, o perfil de Gerenciamento de Dispositivo Móvel é instalado para permitir que você, o administrador de TI, gerencie remotamente o dispositivo. O usuário pode ser solicitado a aceitar um certificado de autorização de Ingresso do Local de Trabalho.

    ![](./media/ProtectEmail/EUX-Windows4-workplaceJoin1.png)

4.  O usuário faz logon usando seu endereço de email usado com o Office. Depois de conectados, talvez seja necessário clicar em **Confirmar Registro** mais uma vez para continuar a registrar seu dispositivo.

    ![](./media/ProtectEmail/EUX-Windows5-workplaceJoin2.png)

    O dispositivo é verificado para ver se ele está registrado.

    ![](./media/ProtectEmail/EUX-Windows6-checking-Enrollment.png)

5.  O usuário conclui então o processo de registro selecionando seu dispositivo e clicando em **Selecionar**. Se seu dispositivo não for exibido, é possível selecionar **Meu dispositivo não está listado** para tentar novamente.

    ![](./media/ProtectEmail/EUX-Windows7-confirm-Device.png)

    O dispositivo é verificado para confirmar se ele é compatível com as políticas da empresa.

    ![](./media/ProtectEmail/EUX-Windows9-checking-Compliance.png)

6.  Se houver um problema de conformidade, será solicitado que o usuário resolva o problema (como criar uma senha válida) e, em seguida, clique em **Verificar Conformidade** para continuar.

    ![](./media/ProtectEmail/EUX-Windows13-resolve-Compliance.png)

    Depois que a conformidade for verificada, o usuário verá que o registro está sendo ativado.

    ![](./media/ProtectEmail/EUX-Windows10-activating-Enrollment.png)

7.  O registro é ativado e o usuário clica em **Continuar** para concluir o processo. O usuário clica em **Concluído** para sair da configuração.

    ![](./media/ProtectEmail/EUX-Windows11-COMPLETE.png)

    Depois que o usuário estiver registrado e a conformidade for verificada, o acesso ao email deverá ficar disponível dentro de alguns minutos.

Se o usuário seguir essas etapas para registrar e ficar compatível e ainda não puder acessar seus emails no dispositivo móvel, ele poderá seguir estas etapas adicionais para tentar corrigir o problema:

-   Primeiro, verifique se seu dispositivo está registrado. Caso contrário, o usuário deve seguir as etapas acima.

-   Verifique se o dispositivo é compatível clicando em **Verificar conformidade**. Se um erro de conformidade for identificado, o usuário poderá seguir as instruções específicas para seu dispositivo móvel sobre como resolvê-la, tal como redefinir sua senha.

-   Ligue para o suporte técnico.

## Problemas e soluções
Por padrão, a cada 8 horas os dispositivos são verificados para verificar se eles ainda são compatíveis. Se um dispositivo que era anteriormente compatível for considerado incompatível (por exemplo, devido a uma política de conformidade ter sido adicionada ou alterada), o usuário pode seguir estas etapas para restaurar a conformidade do dispositivo:

1.  O usuário recebe a notificação por email ou em seu dispositivo que este é incompatível. Neste momento, o dispositivo está em quarentena no Exchange.

2.  Se o usuário tentar acessar o email, ele será redirecionado para a tela de Configuração de Acesso da Empresa do Portal da Empresa do Intune em que se é mostrado se eles estão fora de conformidade.

    ![](./media/ProtectEmail/EUX-Windows14-OutOfCompliance.png)

3.  A usuário clica em **Continuar** e o problema de conformidade que está impedindo que ele acesse o email é mostrado.

4.  Depois que o problema foi corrigido, eles devem clicar em **Verificar Conformidade** para verificar se o problema foi resolvido.

5.  Se o problema estiver corrigido, o usuário clica em **Continuar** para concluir o processo. O acesso ao email deverá ficar disponível novamente dentro de alguns minutos.

### Onde ir daqui
A experiência do usuário final é um pouco diferente em outros dispositivos móveis. Saiba mais sobre a experiência do usuário final para [Android](../Solutions/end-user-experience-conditional-access-android.md) e
[iOS](../Solutions/end-user-experience-conditional-access-ios.md).


<!--HONumber=Apr16_HO2-->

