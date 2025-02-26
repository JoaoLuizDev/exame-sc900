## Descreva os conceitos de segurança, conformidade e identidade (10–15%)
### Descreva os conceitos de segurança e conformidade
• Descreva o modelo de responsabilidade compartilhada
![Modelo de responsabilidade compartilhada](https://learn.microsoft.com/en-us/training/wwl-sci/describe-security-concepts-methodologies/media/3-shared-responsibility-model.png)

• Defina a defesa em profundidade
```
A ideia de camadas de segurança, não apenas proteger o perímetro.
```
• Descreva o modelo Zero-Trust
```
assuma comprometimento, verifique explicitamente, privilégio mínimo para executar uma ação.
```
• Descreva a criptografia e o hash
```
criptografia = função bidirecional usada para embaralhar dados para serem remontados por uma parte confiável.
Hashing = função unidirecional para padronizar dados em um único formato.
```

• Descreva os conceitos de conformidade
```
Residência de dados = onde os dados podem ser armazenados.
Soberania de dados = dados pessoais sujeitos a leis.
Privacidade de dados = como os dados são usados/coletados.
```
### Defina os conceitos de identidade
• Defina a identidade como o perímetro de segurança primário
```
a identidade une todos os pontos e o acesso.
```
• Defina a autenticação
```
verificando se o usuário é quem ele diz ser. Isso normalmente é para dar acesso aos recursos, no entanto, isso é autorização.
```
• Defina a autorização
```
Permissão para executar uma ação em um recurso.
```
• Descreva os provedores de identidade
```
Cria, mantém e gerencia informações de identidade ao oferecer.
```
serviços de autenticação, autorização e auditoria.
```
SSO/Provedores que permitem que você use a mesma credencial em aplicativos/organizações.
```
• Descreva o Active Directory
```
Rede de domínio baseada no local. É muito diferente do Azure AD.
```
• Descreva o conceito de Federação
```
Estabelecendo uma relação de confiança. Confia e estabelecendo confianças de IdP entre organizações/limites de domínio.
```
## Descreva os recursos das Soluções de Gerenciamento de Identidade e Acesso da Microsoft (25–30%)

### Descreva os serviços básicos de identidade e os tipos de identidade do Azure AD
• Descreva o Azure Active Directory
```
Serviço de gerenciamento de identidade e acesso baseado em nuvem da Microsoft.
```
• Descreva as identidades do Azure AD
```
Usuário = Representação de um usuário.
Principal de serviço = identidade para um aplicativo. Deve ser registrado no AZ AD para habilitar a integração.
Identidade gerenciada = Tipo de SP que gerencia automaticamente no AZ AD. Não há necessidade de desenvolvedores gerenciarem credenciais.
```
• Descreva a identidade híbrida
```
2 tipos de identidade gerenciada:
- Atribuída pelo sistema – identidade criada no Azure AD vinculada ao ciclo de vida da instância de serviço, quando excluída, o Azure exclui automaticamente a identidade.
- Atribuída pelo usuário – a identidade é gerenciada separadamente do serviço ao qual é atribuída.
```
• Descreva os diferentes tipos de identidade externa
```
- B2B
- B2C
```
### Descreva os recursos de autenticação do Azure AD
• Descreva os métodos de autenticação disponíveis no Azure AD
```
- Baseado em senha
- Sem senha - Chave FIDO2 sec ou Windows Hello. Hello for Business substitui por 2fa.
```
• Descreva a autenticação multifator
```
Provando que você é quem diz ser com 2 artefatos conhecidos para o sistema no qual está se autenticando.
```
• Descreva a redefinição de senha de autoatendimento
```
- Alteração de senha – o usuário sabe a senha, mas quer alterá-la.
- Redefinição de senha – não sabe a senha.
- Desbloqueio de conta – o usuário não consegue entrar porque está bloqueado.
```
• Descreva os recursos de proteção e gerenciamento de senha disponíveis no Azure AD
```
Lista global de senhas proibidas de senhas conhecidas.
Listas personalizadas de senhas proibidas – pode criar suas próprias listas de senhas proibidas
Proteja contra pulverização de senhas e força bruta.
Segurança híbrida – no local recebe a lista global de proibição e as políticas personalizadas de proteção de senha do Azure AD.
```
### Descreva os recursos de gerenciamento de acesso do Azure AD
• Descreva o acesso condicional
```
Segurança antes de permitir que usuários autenticados acessem dados ou outros ativos.
```
• Descreva os benefícios das funções do Azure AD
```
As funções do Azure AD ajudam a segmentar as permissões de usuário das organizações, assim como VNets e NSGs ajudam a segmentar o acesso à rede das organizações.
```
• Descreva os benefícios do controle de acesso baseado em função do Azure AD
```
Ele permite que os usuários tenham conjuntos de permissões elevados quando necessário e acordado de forma explicitamente permitida e controlada.
```
### Descreva os recursos de proteção e governança de identidade do Azure AD
• Descreva a governança de identidade no Azure AD:
```
- Governe o ciclo de vida da identidade.
- Governe o ciclo de vida do acesso.
- Proteja o acesso privilegiado para administração.
```

• Descreva o gerenciamento de direitos e as revisões de acesso
```
O gerenciamento de direitos é um recurso de governança de identidade que permite que as organizações gerenciem o ciclo de vida da identidade e do acesso em escala.
```
• Descreva os recursos do Azure AD Privileged Identity Management (PIM)
```
O PIM permite que os usuários elevem seus privilégios por um tempo alocado para executar ações que seu usuário padrão normalmente não teria permissão para fazer. Ele ajuda a manter as organizações seguras enquanto permite que os fluxos de trabalho evoluam.
```
• Descreva a proteção de identidade do Azure AD
```
A proteção de identidade é uma ferramenta que permite que as organizações realizem três tarefas principais:
- Automatizar a detecção e a correção de riscos baseados em identidade.

- Investigar riscos usando dados no portal.

- Exportar dados de detecção de risco para utilitários de terceiros para análise posterior.
```

## Descreva os recursos das soluções de segurança da Microsoft (25–30%)

### Descreva os recursos básicos de segurança no Azure
• Descreva a proteção contra DDoS do Azure

```
2 tipos, avançado permite ajuste automático, padrão fornece todo o resto.
```
• Descreva o Firewall do Azure
```
Serviço de segurança de firewall de rede nativo da nuvem e totalmente com estado. Ele fornece proteção contra ameaças para cargas de trabalho na nuvem em execução no Azure.
```
• Descreva o Web Application Firewall
```
Proteção centralizada para aplicativos da Web. O WAF no Azure Application Gateway fornece proteção contra explorações e vulnerabilidades comuns.

```
• Descreva a segmentação de rede com VNet
```
A segmentação é usada para minimizar a pegada de rede, garantindo restrições à rede da organização mais ampla, impedindo o acesso a itens fora da rede virtual sem permissão explícita para isso.
```
• Descreva os grupos de segurança de rede do Azure
```
Filtre o tráfego de rede entre os recursos do Azure em uma rede virtual do Azure. Um NSG contém regras de segurança que permitem ou negam o tráfego de rede de entrada ou o tráfego de rede de saída de vários tipos de recursos do Azure. Para cada regra, você pode especificar a origem e o destino, a porta e o protocolo.
```

• Descreva o Azure Bastion e o acesso JIT
```
O Azure Bastion é um serviço que você implanta e permite que você se conecte a uma máquina virtual usando seu navegador e o portal do Azure ou por meio do cliente SSH ou RDP nativo já instalado em seu computador local.
O JIT ou Just in Time gerencia o acesso para garantir que usuários com credenciais corretas sejam autorizados a acessar os recursos com base em condições especificadas.
```

• Descreva as maneiras como o Azure criptografa dados
```
- Criptografia de serviço de armazenamento - dados em repouso criptografados automaticamente.
- Criptografia de disco do Azure - criptografa discos de VM do Windows e Linux.
- Criptografia de dados transparente - protege bancos de dados SQL e o Azure Data Warehouse contra atividades maliciosas.
- Azure KeyVault - usado para armazenar segredos, chaves e certificados com segurança.
```

## Descreva os recursos de gerenciamento de segurança do Azure
• Descreva o gerenciamento de postura de segurança em nuvem (CSPM)
```
Melhora as funções de segurança de nuvem de nível superior e as relações de objetos de nuvem.
```

• Descreva o Microsoft Defender para Nuvem
• Descreva os recursos de segurança aprimorados do Microsoft Defender para Nuvem
```
Habilita os recursos do modo livre para cargas de trabalho em execução no Azure, híbridas e outras plataformas de nuvem. Planos integrados do Microsoft Defender, específicos para os tipos de recursos em suas assinaturas e fornecem recursos de segurança aprimorados para suas cargas de trabalho.
```

• Descreva as linhas de base de segurança para o Azure
```
O Benchmark fornece práticas recomendadas e recomendações prescritivas para ajudar a melhorar a segurança de cargas de trabalho, dados e serviços no Azure
As linhas de base aplicam a orientação do Azure Security Benchmark ao serviço específico para o qual são definidas.

```

### Descreva os recursos de segurança do Microsoft Sentinel
• Defina os conceitos de SIEM e SOAR
```
SIEM - Usado para ingerir dados de várias fontes diferentes e correlacioná-los em um ponto centralizado.
SOAR - respondendo a incidentes automaticamente.
```

• Descreva como o Microsoft Sentinel fornece gerenciamento integrado de ameaças
```
coleta dados, detecta, investiga e responde a ameaças.
```

### Descreva a proteção contra ameaças com o Microsoft 365 Defender
• Descreva os serviços do Microsoft 365 Defender
```
Defender para 365, nuvem, endpoint, aplicativos em nuvem.
```
• Descreva o Microsoft Defender for Identity (antigo Azure ATP)
```
solução de segurança baseada em nuvem que identifica, detecta e ajuda a investigar ameaças avançadas, identidades comprometidas e ações maliciosas de pessoas internas.
```

• Descreva o Microsoft Defender para Office 365 (antigo Office 365 ATP)
```
Proteja-se contra ameaças maliciosas representadas por mensagens de e-mail, links (URLs) e ferramentas de colaboração.
```
• Descreva o Microsoft Defender para Endpoint (antigo Microsoft Defender ATP)
```
Solução de endpoint para defender.
```
• Descreva o Microsoft Defender para aplicativos em nuvem
```
Solução de segurança de aplicativo em nuvem.
```
• Descreva o portal do Microsoft 365 Defender
```
Combina proteção, detecção, investigação e resposta ao seguinte:
- E-mail
- Colaboração (B2B, B2C)
- Identidade
- Dispositivos
- Ameaças de aplicativos em nuvem

```
## Descreva os recursos das soluções de conformidade da Microsoft (25–30%)
### Descreva o Portal de Confiança de Serviço da Microsoft e os princípios de privacidade
• Descreva as ofertas do portal de Confiança de Serviço
```
- Certificações, regulamentos e padrões
- Relatórios, whitepapers e artefatos
- Recursos regionais e do setor
- Recursos para sua organização
```
• Descreva os princípios de privacidade da Microsoft
```
- controle
- transparência
- segurança
- proteções legais fortes
```

#### Descreva os recursos de gerenciamento de conformidade do Microsoft Purview
• Descreva o portal de conformidade do Microsoft Purview
```
reúne todos os ferramentas e dados que são necessários para ajudar a entender e gerenciar as necessidades de conformidade de uma organização.
fornece avaliação pré-construída, recursos de fluxo de trabalho, melhoria passo a passo e pontuação.
```
• Descreva o gerenciador de conformidade
```
Recurso que ajuda os administradores a gerenciar os requisitos de conformidade.
```

• Descreva o uso e os benefícios da pontuação de conformidade
```
calculada usando pontuações atribuídas a ações
2 tipos de ação:
- Suas ações aprimoradas: ações que a organização deve gerenciar.
- Ações da Microsoft: ações que a Microsoft gerencia para a organização.
```

### Descreva os recursos de proteção de informações e gerenciamento do ciclo de vida de dados do Purview
#### Microsoft Purview
• Descreva os recursos de classificação de dados
```
Identificação e classificação de itens confidenciais dentro da organização de 3 maneiras:
- Manual por usuários
- Reconhecimento automatizado baseado em padrões, mais ou menos como os tipos de informações confidenciais funcionam
- Aprendizado de máquina
```

• Descreva os benefícios do explorador de conteúdo e atividade
```
O explorador de conteúdo usa o painel de classificação de dados para obter visibilidade do conteúdo no painel de visão geral.
O explorador de atividade mostra qual conteúdo foi descoberto e rotulado.
```

• Descreva os rótulos de sensibilidade
```
Habilite a proteção do conteúdo sem afetar a produtividade e a colaboração.
```

• Descreva a Prevenção contra Perda de Dados (DLP)
```
Uma maneira de proteger informações confidenciais e evitar sua divulgação inadvertida.
```

• Descreva o Gerenciamento de Registros
```
Conteúdo de liberação, política de retenção aplicada, retenção baseada em eventos, revisão e validação, prova de exclusão, informações de exportação sobre itens descartados.
```

• Descreva as Políticas de Retenção e os Rótulos de Retenção
```
O conteúdo é mantido apenas pelo tempo necessário e, em seguida, excluído permanentemente.
```

### Descreva os recursos de risco interno no Microsoft Purview
• Descreva o Gerenciamento de Risco Interno
```
Há uma ampla gama de riscos internos. O gerenciamento de riscos é centrado em transparência, fluxos de trabalho de integração, ações e configurações relacionadas a riscos internos.
```

• Descreva a conformidade da comunicação
```
Solução de risco interno que ajuda a minimizar os riscos de comunicação detectando, capturando e agindo em mensagens não compatíveis.
```

• Descreva as barreiras de informação
```
As políticas de barreira de informação determinam e previnem comunicações não autorizadas.
```

## Descreva os recursos de governança de recursos no Azure
• Descreva a Política do Azure
```
Projetado para ajudar a impor padrões e avaliar a conformidade em uma organização.
```

• Descreva os Blueprints do Azure
```
Maneira declarativa de orquestrar a implantação de vários modelos de recursos e outros artefatos.
```

• Descreva os recursos no portal de governança do Microsoft Purview
```
Crie mapas holísticos do cenário de dados com funções automatizadas, permita que os curadores de dados gerenciem e protejam o patrimônio, torne a pesquisa de dados mais valiosa e integral.
```