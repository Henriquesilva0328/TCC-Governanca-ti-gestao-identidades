# 3. Metodologia de Pesquisa

Este capítulo apresenta a fundamentação e os procedimentos metodológicos adotados para a condução do estudo de caso na FATEC Barueri. O objetivo é estabelecer a rastreabilidade entre a coleta de dados empíricos, o diagnóstico do cenário atual de acesso aos laboratórios de informática e a posterior especificação dos Requisitos Funcionais (RF) e Não Funcionais (RNF) para a integração do Active Directory (AD) com o GLPI.

---

### 3.1. Natureza e Tipologia da Pesquisa

A pesquisa caracteriza-se como um **estudo de caso aplicado**, de abordagem **mista (qualitativo-quantitativa)** e com objetivos **exploratório-descritivos**:

* **Exploratório-Descritiva:** Dedica-se a mapear e descrever a operação real dos laboratórios de informática, identificando gargalos no processo de *login*, fragilidades na gestão de identidades e impactos no tempo didático.
* **Estudo de Caso Aplicado:** Foca no ambiente computacional específico da FATEC Barueri com a finalidade de fundamentar uma proposta de melhoria prática e tecnicamente viável.

Para assegurar a confiabilidade do diagnóstico, adotou-se o método de **triangulação de dados**, confrontando relatos dos usuários finais, evidências técnicas trazidas pela equipe de TI e observação direta do ambiente.

---

### 3.2. População, Amostragem e Perfis Mapeados

A amostragem foi definida por conveniência e acessibilidade no campus. A investigação cobriu quatro perfis complementares para capturar diferentes perspectivas da operação:

1. **Estudantes (Usuários Finais):** Foco na experiência prática de acesso, tempo de início/término de sessão, retenção de arquivos locais, percepção de privacidade e frequência de troca de estações por falhas.
2. **Docentes:** Foco no impacto do modelo de acesso sobre a dinâmica das aulas, estabilidade do sistema de projeção (*datashow*), disponibilidade de softwares específicos e perda de tempo letivo.
3. **Equipe de TI / Suporte (Diagnóstico Operacional):** Foco nas rotinas de manutenção, atendimento a chamados, gestão de contas locais, procedimento de congelamento/restauração de disco e problemas mais recorrentes.
4. **Equipe de TI / Gestão (Planejamento Estratégico):** Foco na infraestrutura de servidores, diretórios de usuários, políticas de grupo (GPO), requisitos de rede, conformidade com a LGPD e viabilidade de integração AD + GLPI.

---

### 3.3. Instrumentos de Coleta e Validação

A coleta combinou múltiplos instrumentos estruturados no repositório do projeto:

```text
docs/03-coleta-de-dados/
├── plano-de-coleta.md
├── metodologia.md
├── roteiro-entrevista-suporte.md
├── roteiro-entrevista-docentes.md
├── roteiro-estudantes.md
└── checklist-laboratorio.md
Validação e Ajustes dos Instrumentos
Antes da aplicação oficial, os questionários do Google Forms passaram por revisão técnica e pedagógica junto ao orientador, resultando em:

Perspectiva Docente: Readequação das perguntas para capturar a observação do professor sobre o comportamento e as dificuldades da turma durante a aula.

Aspectos Didático-Visuais: Inclusão de indicadores sobre problemas de conexão e exibição via datashow.

Padronização Técnica: Substituição de nomes comerciais de softwares de restauração por descrições funcionais do mecanismo de congelamento de disco.

Categorização de Infraestrutura: Transformação de questões abertas sobre variações entre laboratórios em caixas de seleção fechadas (sistemas operacionais, softwares e permissões).

3.4. Execução da Coleta de Dados
A fase de campo ocorreu de forma estruturada, compreendendo a elaboração dos instrumentos, validação com a orientação, limpeza de dados de teste e ampla divulgação junto aos públicos-alvo por meio de canais institucionais. O processo de coleta foi oficialmente encerrado em 10/10/2026, momento em que o recebimento de novas submissões nos formulários foi travado para dar início imediato à tabulação dos resultados, exportação dos dados brutos e análise temática.

3.5. Diretrizes de Privacidade, Segurança e LGPD
Em estrita observância à Lei Geral de Proteção de Dados (Lei nº 13.709/2018) e aos limites éticos da pesquisa acadêmica:

Minimização de Dados e Anonimato: Não foram solicitados dados pessoais identificáveis (nomes, e-mails pessoais, CPFs, RAs ou senhas) nos formulários de Estudantes e Docentes.

Segurança da Informação: A consulta técnica à equipe de TI abrangeu apenas aspectos arquiteturais e operacionais, sem exposição de credenciais, listas de usuários ou vulnerabilidades de servidores.

Limites Operacionais: A pesquisa não realizou testes de invasão, exploração de falhas, alteração de configurações de estações ou coleta não autorizada de logs.

3.6. Classificação da Informação, Triangulação e Tratamento de Lacunas
Os dados obtidos foram classificados segundo a sua origem e grau de confirmação:

Relato: Informação declarada por estudantes, docentes ou equipe de TI.

Observação: Informação constatada diretamente no ambiente por meio do checklist-laboratorio.md.

Evidência Documental / Informação Validada: Informação confirmada pelo cruzamento de duas ou mais fontes compatíveis (ex: Relato do Suporte + Observação do Ambiente = Informação Validada).

Plaintext
[Relato dos Usuários]  \
[Relato do Suporte]    --->  TRIANGULAÇÃO DE DADOS  --->  [Informação Validada / Requisito]
[Observação Direta]   /
Tratamento de Divergências e Limitações
Discrepâncias de Relato: Caso ocorra divergência entre o relato dos usuários e a configuração declarada pela TI (ex: aluno afirmando salvar arquivos localmente versus TI reportando disco congelado), a divergência é tratada como uma lacuna de comunicação/percepção do modelo atual, fundamentando Requisitos Não Funcionais (RNF) de usabilidade e governança.

Tratamento de Instrumentos sem Resposta: Diante da ausência de submissões diretas em um dos formulários previstos, a lacuna informacional foi tratada mediante triangulação por observação direta e análise da documentação técnica, garantindo o atendimento integral aos critérios de suficiência da pesquisa sem comprometer o cronograma do projeto.

3.7. Rastreabilidade para as Próximas Etapas
Cada dado validado nesta etapa recebe um identificador de origem (COL-xxx para coleta, OBS-xxx para observação e EV-xxx para evidências). Esses identificadores serão mapeados diretamente para a Matriz de Riscos (RIS) e para os Requisitos Funcionais (RF) e Não Funcionais (RNF), garantindo que toda decisão de projeto seja estritamente fundamentada em evidências empíricas do ambiente da FATEC Barueri.
