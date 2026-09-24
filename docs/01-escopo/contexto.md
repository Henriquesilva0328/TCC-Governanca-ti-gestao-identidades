# Contexto do Projeto

## 1. Contextualização institucional

A transformação digital das instituições de ensino superior ampliou a utilização de recursos tecnológicos nas atividades acadêmicas e administrativas, tornando a infraestrutura de Tecnologia da Informação (TI) um elemento fundamental para o funcionamento dessas organizações.

Nesse contexto, os laboratórios de informática representam ambientes de utilização compartilhada, nos quais diferentes usuários acessam equipamentos, sistemas, aplicações e recursos institucionais ao longo do período acadêmico. A administração desses ambientes exige não apenas a disponibilidade dos equipamentos, mas também a definição de mecanismos adequados de identificação, autenticação, autorização e rastreabilidade dos usuários.

A Governança de TI fornece uma estrutura para orientar a utilização dos recursos tecnológicos, estabelecer responsabilidades, gerenciar riscos e assegurar que os processos de TI estejam alinhados às necessidades institucionais.
Segundo a ISACA (2019), o COBIT 2019 estabelece um modelo de governança e gestão da informação e tecnologia, permitindo que as organizações relacionem seus objetivos institucionais aos processos, controles e responsabilidades associados à utilização dos recursos tecnológicos. Sob essa perspectiva, a gestão de identidades e acessos constitui um componente relevante da Governança de TI, pois estabelece mecanismos para administrar quem pode acessar determinados recursos, quais permissões são concedidas e como a utilização desses recursos pode ser associada aos usuários.

## 2. Caracterização do ambiente estudado

O presente projeto tem como objeto de estudo os laboratórios de informática da Faculdade de Tecnologia de Barueri (FATEC Barueri).

Conforme o levantamento preliminar apresentado no relatório inicial do Trabalho de Graduação, os computadores dos laboratórios utilizam os perfis denominados "suporte" e "aluno". O acesso dos estudantes é realizado por meio de uma credencial compartilhada, utilizada por diferentes usuários durante as atividades acadêmicas. Embora esse modelo permita a utilização dos equipamentos sem exigir uma autenticação individual no sistema operacional, a utilização de uma identidade compartilhada limita a possibilidade de associar uma sessão específica ao estudante que efetivamente utilizou determinado computador.

O ambiente também possui um mecanismo de restauração das estações, configurado para remover arquivos e alterações realizadas durante sua utilização após o desligamento dos equipamentos. Esse mecanismo contribui para a manutenção de um ambiente padronizado entre diferentes utilizações. Entretanto, a restauração das estações não substitui a identificação individual dos usuários, uma vez que a remoção de arquivos e alterações locais não estabelece, por si só, um vínculo entre a identidade de um estudante e a sessão realizada.

Além disso, será necessário verificar durante a coleta de dados quais registros são efetivamente produzidos, preservados ou eliminados pelo mecanismo de restauração, bem como identificar a existência de eventuais controles complementares de autenticação e rastreabilidade. Dessa forma, o cenário preliminar evidencia a necessidade de compreender não apenas o funcionamento técnico dos computadores, mas também os processos de administração das contas, as responsabilidades dos profissionais envolvidos e os controles institucionais associados à utilização dos laboratórios.

## 3. Gestão de identidades e controle de acesso

A Gestão de Identidades e Acessos, denominada Identity and Access Management (IAM), compreende processos e mecanismos utilizados para administrar identidades digitais e controlar o acesso de usuários aos recursos tecnológicos de uma organização.

Entre os aspectos relevantes para este projeto estão:

- identificação dos usuários;
- autenticação individual;
- definição e administração de permissões;
- gerenciamento do ciclo de vida das contas;
- controle das sessões de utilização;
- registro dos eventos de acesso;
- rastreabilidade das atividades;
- administração de contas privilegiadas.

As diretrizes de identidade digital do NIST SP 800-63-4 apresentam orientações relacionadas aos processos de comprovação de identidade, autenticação e federação de identidades, incluindo considerações de segurança, privacidade e experiência dos usuários (NIST, 2025).

No contexto dos laboratórios, a adoção de uma identificação individual poderá ser considerada como alternativa para estabelecer uma associação entre o estudante, a sessão de utilização e o equipamento acessado, entretanto, a utilização de contas individuais não representa, isoladamente, uma garantia de rastreabilidade completa. A efetividade desse mecanismo depende de fatores adicionais, como a administração das credenciais, a configuração das permissões, a disponibilidade dos registros, o gerenciamento das sessões e a existência de controles que reduzam a possibilidade de compartilhamento indevido de contas.

Por esse motivo, o projeto deverá analisar o modelo atual de acesso em conjunto com os mecanismos de controle já existentes, evitando considerar a simples substituição de uma credencial compartilhada como solução suficiente para todos os riscos identificados.

## 4. Governança de TI e gestão de riscos

A análise do ambiente será conduzida sob a perspectiva da Governança de TI, utilizando o COBIT 2019 como principal referencial para compreender a relação entre processos, responsabilidades, recursos tecnológicos e riscos institucionais. A gestão de riscos será utilizada para identificar situações que possam comprometer a identificação dos usuários, a rastreabilidade das atividades e o controle de utilização dos equipamentos. A ISO/IEC 27001:2022 fornece uma referência complementar para a gestão da segurança da informação, estabelecendo requisitos relacionados à estruturação e melhoria contínua de um Sistema de Gestão de Segurança da Informação (ISO/IEC, 2022).

Neste trabalho, seus conceitos serão utilizados como apoio à identificação dos riscos e à avaliação dos controles de segurança pertinentes ao ambiente estudado. A análise deverá considerar tanto os riscos associados ao modelo atual quanto as possíveis dificuldades introduzidas por alternativas de identificação individual. Entre os aspectos que deverão ser considerados estão a compatibilidade com os equipamentos existentes, a disponibilidade dos serviços de autenticação, a capacidade de suporte, o gerenciamento das contas e os impactos de uma eventual alteração no processo de acesso durante as atividades acadêmicas.

A pesquisa não pressupõe que a instituição apresente falhas de segurança além das limitações inicialmente identificadas. A existência de outros problemas, controles ou riscos deverá ser verificada durante a coleta de dados e fundamentada nas evidências obtidas.

## 5. Privacidade e proteção de dados pessoais

A identificação individual dos estudantes envolve a utilização de informações capazes de estabelecer uma relação entre uma pessoa e determinado acesso aos recursos tecnológicos. Nesse contexto, a avaliação das alternativas deverá considerar a Lei Geral de Proteção de Dados Pessoais (LGPD), Lei nº 13.709/2018, especialmente quanto aos princípios de finalidade, adequação, necessidade, segurança e prevenção (BRASIL, 2018).

Entre as possibilidades inicialmente consideradas para identificação dos estudantes estão a utilização do Registro Acadêmico (RA) e, quando aplicável, do Cadastro de Pessoas Físicas (CPF). A utilização desses identificadores deverá ser avaliada considerando sua necessidade, adequação à finalidade pretendida, disponibilidade institucional e possibilidade de integração com os sistemas existentes. A existência de um dado pessoal nos sistemas institucionais não significa que sua utilização seja automaticamente necessária ou adequada para autenticação nos laboratórios. Também deverá ser considerada a possibilidade de utilização de identificadores internos ou de mecanismos de autenticação institucional que reduzam a necessidade de coleta e exposição de informações pessoais adicionais.

A pesquisa deverá distinguir o identificador utilizado para reconhecer uma conta do mecanismo empregado para autenticar o usuário, considerando que o conhecimento de um número de identificação, isoladamente, não comprova necessariamente a identidade de quem realiza o acesso. A proteção dos dados deverá ser considerada desde o levantamento dos requisitos até a avaliação das alternativas, incluindo aspectos relacionados ao acesso às informações, armazenamento, retenção e utilização dos registros de autenticação.

## 6. Governança de Inteligência Artificial como camada complementar

A utilização de ferramentas baseadas em Inteligência Artificial (IA) em atividades de desenvolvimento, análise técnica e administração de sistemas introduz questões adicionais relacionadas à utilização de informações institucionais, à definição de responsabilidades e ao controle dos resultados produzidos por essas ferramentas. No contexto deste projeto, a Governança de IA será considerada como uma camada complementar e preventiva à Governança de TI e à segurança da informação. Sua inclusão não pressupõe que os laboratórios da FATEC Barueri utilizem atualmente mecanismos de inteligência artificial para autenticação, controle de acesso ou gerenciamento de identidades. Também não constitui objetivo do trabalho desenvolver ou implementar uma solução baseada em IA.

A proposta consiste em considerar a necessidade de diretrizes institucionais para situações em que ferramentas de inteligência artificial possam ser utilizadas futuramente no desenvolvimento, na implementação, na manutenção ou na administração de uma possível solução de identificação individual. Um exemplo é a eventual utilização de ferramentas de IA por profissionais responsáveis pela segurança ou administração da infraestrutura tecnológica. Dependendo das atividades desempenhadas, esses profissionais poderão ter acesso a configurações internas, registros técnicos, informações de usuários, políticas de segurança e outros dados cuja exposição inadequada possa comprometer a instituição.

Nesse cenário, o uso de ferramentas de IA deverá ser previamente avaliado e delimitado, especialmente quando envolver o compartilhamento de informações com serviços externos. O NIST AI Risk Management Framework (AI RMF 1.0) apresenta uma estrutura voluntária para orientar a identificação, a avaliação e o gerenciamento de riscos relacionados aos sistemas de inteligência artificial (NIST, 2023). De forma complementar, a ISO/IEC 42001:2023 estabelece requisitos para sistemas de gestão de inteligência artificial, contemplando a definição de políticas, responsabilidades e processos relacionados ao desenvolvimento e à utilização desses sistemas (ISO/IEC, 2023).

Esses referenciais poderão subsidiar a proposição de diretrizes preventivas compatíveis com o escopo do projeto, sem pressupor a necessidade de implantação integral de um sistema de gestão de IA.

A análise complementar deverá considerar:

- definição das finalidades permitidas para a utilização de ferramentas de IA;
- identificação dos profissionais autorizados a utilizar essas ferramentas em atividades relacionadas à infraestrutura;
- restrições ao compartilhamento de credenciais, informações pessoais e configurações institucionais;
- avaliação dos riscos relacionados à utilização de serviços externos;
- proteção das informações submetidas às ferramentas;
- verificação humana das recomendações e dos resultados produzidos;
- definição de responsabilidades sobre decisões e ações realizadas com apoio de IA;
- necessidade de aprovação institucional antes de eventual utilização de IA em processos críticos de segurança.

A utilização de ferramentas de IA não deverá substituir a responsabilidade dos profissionais autorizados pelas decisões relacionadas à infraestrutura tecnológica. Assim, a Governança de IA será incorporada ao projeto como uma consideração preventiva sobre o uso futuro de ferramentas inteligentes em atividades relacionadas à gestão de identidades e acessos, sem ampliar o objeto central da pesquisa.

## 7. Delimitação do estudo

O projeto será desenvolvido como um estudo de caso de natureza aplicada, apresentado na modalidade de Relato Tecnológico. Nesta primeira etapa, a pesquisa estará limitada ao levantamento do cenário atual, à coleta e validação de informações, à identificação dos riscos, ao levantamento de requisitos e à avaliação das alternativas tecnológicas. Também serão elaboradas recomendações e um plano de melhoria considerando as necessidades e restrições identificadas durante a pesquisa.

A Governança de IA será contemplada exclusivamente como uma dimensão complementar da análise, relacionada à definição de diretrizes preventivas para o eventual uso de ferramentas inteligentes em atividades que envolvam informações institucionais ou processos de gestão de identidades. Não fazem parte desta etapa a implementação de sistemas, a alteração do ambiente de produção, a implantação de mecanismos de autenticação, a aquisição de equipamentos ou a realização de testes invasivos. Os resultados deverão fornecer subsídios técnicos e gerenciais para apoiar a avaliação de possíveis melhorias futuras, sem pressupor sua aprovação ou implementação pela instituição.

---

## Referências bibliográficas

As referências completas utilizadas na fundamentação deste documento estão disponíveis em:

[Referências bibliográficas do projeto](../08-bibliografia/referencias.md)
