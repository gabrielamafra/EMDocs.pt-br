---
# required metadata

title: Requisitos de gerenciamento
description:
keywords:
author: YuriDio
manager: swadhwa
ms.date: 04/28/2016
ms.topic: article
ms.prod:
ms.service:
ms.technology:
ms.assetid: c576a1be-c706-4a12-a2e2-b3d85e632afa

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
ms.reviewer: 
ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom:

---

# Requisitos de gerenciamento

Gerenciamento de dispositivos é um dos fundamentos de qualquer estratégia centrada em pessoas e deve ser avaliada em relação aos requisitos da empresa. Dependendo do nível de maturidade da empresa, um sistema de gerenciamento pode estar estabelecido, precisando ser expandida para cobrir os cenários BYOD que a empresa está adotando. A Figura 4 mostra interações de gerenciamento ao gerenciar usuários, dispositivos e dados. Considerações devem ser feitas para cada componente do subdomínio de gerenciamento.

![Requisitos de gerenciamento](./media/BYOD_Figure4.png)

Ao considerar os requisitos de capacidade de gerenciamento, você deve começar fazendo as perguntas listadas na próxima seção.

## Perguntas a fazer

As perguntas sobre requisitos de gerenciamento são categorizadas em sete áreas:

- Monitoramento
- Relatórios
- Configuração
- Computar
- Armazenamento
- Automação
- Implantação e provisionamento


### Monitoramento

- Sua empresa precisa monitorar as configurações de conformidade, como senha, câmera e criptografia, em dispositivos dos usuários?
- Sua empresa deseja diferenciar propriedade de dispositivo (dispositivos de propriedade da empresa versus dispositivos de propriedade do usuário)?
- Sua empresa deseja permitir que os usuários redefinam suas senhas em seus próprios dispositivos?
- Sua empresa precisa ter o recurso de log integrado ao sistema de gerenciamento?
- Sua empresa precisa de recursos de auditoria integrados ao sistema de gerenciamento?
- Sua empresa agrega esse tipo de log em um único repositório?

### Relatórios

- Sua empresa precisa de recursos de relatório para seu modelo BYOD?
    - Nesse caso, que tipos de relatórios (como atualizações de software instalados e inventário) serão necessários?
- O sistema de gerenciamento em vigor tem esses requisitos de relatórios?
    - Nesse caso, é possível personalizá-los?
- Há alguma diferenciação nos requisitos de emissão de relatórios para dispositivos ingressados de domínio e ingressados não de domínio?
    - Nesse caso, quais são os requisitos para cada cenário?

### Configuração

- Sua empresa precisa de um sistema de gerenciamento que exija que os dispositivos dos usuários sejam ingressados no domínio para serem gerenciado?
- Sua empresa precisa de um sistema de gerenciamento que se integre ao diretório atual?
- Sua empresa precisa um sistema de gerenciamento que gerencie apenas aplicativos ou ele também deve gerenciar o sistema operacional em execução em dispositivos dos usuários?
- Sua empresa precisa de um sistema de gerenciamento que possa impor políticas aos dispositivos dos usuários?
- Sua empresa precisa de um sistema de gerenciamento possa ser integrado a serviços de nuvem?
- A sua empresa planeja executar limpeza seletiva no caso de um usuário não precisar mais de acesso a aplicativos que foram instalados?
    - Nesse caso, o sistema de gerenciamento em vigor oferece suporte a recurso de limpeza seletiva?

### Computar

- Quais são os recursos de computação necessários para executar o sistema de gerenciamento em servidores de back-end?
- Quais são os recursos de computação necessários para executar o sistema de gerenciamento em dispositivos dos usuários?
- O sistema de gerenciamento dá suporte a aproveitar a capacidade de nuvem para expandir os recursos de computação local?

### Armazenamento

- Quais são os requisitos de armazenamento para executar o sistema de gerenciamento em servidores de back-end?
- Quais são os requisitos de armazenamento para executar o sistema de gerenciamento em dispositivos dos usuários?
- O sistema de gerenciamento dá suporte a aproveitar recursos de nuvem para expandir os recursos de armazenamento local?
- A empresa precisa gerenciar as unidades de armazenamento externo que devem ser adicionadas a dispositivos dos usuários?
- A empresa precisa de um sistema de gerenciamento que também seja capaz de integrar-se ao armazenamento em nuvem?

### Automação

- Que operações sua empresa planeja automatizar para cenários BYOD?
- Quais são os requisitos de automação para o sistema de gerenciamento que sua empresa planeja adotar?
- O sistema de gerenciamento atual dá suporte a automação de linha de comando ou script integrada?
- A sua empresa tem um sistema de gerenciamento que integra serviços de nuvem e fornece recursos de automação?

### Implantação e provisionamento

- Quais são os requisitos para implantação de agentes de gerenciamento para o sistema de gerenciamento atual?
- Será oferecido algum serviço aos usuários remotos que possa ser provisionado instantaneamente por meio de um portal?
- Os dispositivos pessoais são registrados com a empresa pela TI ou são registrados pessoalmente?
- Haverá um plano em vigor para permitir que os usuários provisionem serviços usando seus próprios dispositivos?
    - Nesse caso, o sistema de gerenciamento nativamente permite aos usuários executar esta operação em seus dispositivos?



<!--HONumber=Apr16_HO2-->

