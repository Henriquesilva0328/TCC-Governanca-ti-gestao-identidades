3. Metodologia de Pesquisa
Este capítulo descreve os procedimentos metodológicos adotados para a elaboração deste Trabalho de Graduação, detalhando o tipo de pesquisa, a seleção dos participantes, os instrumentos utilizados para a coleta de dados e as técnicas de análise aplicadas para fundamentar a proposta de integração entre o Active Directory (AD) e o GLPI na FATEC Barueri.

3.1. Natureza e Tipologia da Pesquisa
A presente investigação caracteriza-se como um estudo de caso aplicado, de natureza mista (qualitativo-quantitativa) e com objetivos exploratório-descritivos.

Exploratório e Descritivo: Procura mapear e descrever detalhadamente o cenário atual de gestão de identidades nos laboratórios de informática, identificando gargalos operacionais e os impactos diretos na dinâmica pedagógica.

Estudo de Caso Aplicado: Centra-se no ambiente real da FATEC Barueri, com o intuito de propor uma solução tecnológica prática e viável para o problema identificado.

Para garantir a validade dos resultados, a metodologia baseou-se na triangulação de dados, cruzando as percepções dos usuários finais (docentes e estudantes) com as evidências técnicas fornecidas pela equipe de Tecnologia da Informação (TI) e a observação direta do ambiente.

3.2. População e Amostragem
A amostragem foi definida por conveniência, focando-se nos intervenientes diretos no uso e na administração dos laboratórios de informática. A população do estudo foi segmentada em quatro perfis distintos, cada um com um propósito específico na coleta de dados:

Estudantes: Usuários finais dos laboratórios. O objetivo foi avaliar a experiência de uso, os tempos de espera no início da sessão, a frequência de troca de computadores por falhas e as preocupações com a privacidade dos dados ao utilizar contas genéricas.

Docentes: Responsáveis pela condução das aulas. A consulta a este grupo visou medir o impacto das falhas de acesso no tempo letivo, a estabilidade das projeções (datashow) e a disponibilidade dos softwares necessários.

Equipe de TI / Suporte (Diagnóstico): Focada no levantamento das rotinas atuais de manutenção, na gestão de contas locais, nos métodos de congelamento de disco e no volume de chamados informais.

Equipe de TI / Gestão (Planejamento): Focada na validação técnica da solução proposta, avaliando os pré-requisitos de infraestrutura, as políticas de grupo (GPO) e a viabilidade operacional da implementação do AD integrado ao GLPI.

3.3. Instrumentos de Coleta de Dados
A coleta de dados primários foi realizada através da aplicação de questionários estruturados online, desenvolvidos na plataforma Google Forms. A estruturação dos instrumentos foi dividida em duas fases:

Fase 1 (Diagnóstico do Cenário Atual): Três questionários distintos direcionados a Estudantes, Docentes e equipe de Suporte de TI, com perguntas de escolha múltipla, caixas de seleção e campos abertos para recolher relatos específicos.

Fase 2 (Validação da Solução): Um questionário direcionado à Gestão de TI, focado exclusivamente no planejamento e na arquitetura da nova infraestrutura.

Adequação e Validação dos Instrumentos:
Antes da aplicação definitiva, os formulários passaram por um ciclo de revisão com o orientador do projeto, resultando nos seguintes aprimoramentos metodológicos:

Reajuste da perspectiva das perguntas dirigidas aos docentes, focando-se na sua observação da turma em sala de aula.

Inclusão de variáveis referentes aos atrasos na configuração da projeção (datashow).

Substituição de jargões comerciais (ex.: marcas de softwares de restauração) por descrições do comportamento funcional do sistema, evitando ambiguidades para a equipe técnica.

Transformação de questões abertas sobre infraestrutura em categorias fechadas (sistemas operacionais, softwares, hardware e permissões), facilitando a posterior tabulação quantitativa.

3.4. Procedimentos Éticos e Conformidade (LGPD)
O planejamento da pesquisa obedeceu a rigorosos critérios éticos e aos princípios da Lei Geral de Proteção de Dados Pessoais (Lei nº 13.709/2018). Os instrumentos foram desenhados para garantir o anonimato total dos docentes e estudantes.
Não foram coletados dados sensíveis ou identificadores diretos, tais como nomes, números de Registro Acadêmico (RA), CPFs, e-mails pessoais ou senhas. As informações coletadas junto da TI restringiram-se a aspectos operacionais e de arquitetura, sem exposição de credenciais ou dados sigilosos da instituição.

3.5. Plano de Coleta: Planejado vs. Realizado
O cronograma de execução da coleta de dados decorreu conforme sistematizado na tabela abaixo, distinguindo as etapas previstas das efetivamente realizadas:

Etapa	Atividade	Execução	Status
1. Desenho	Elaboração dos 4 instrumentos de pesquisa segmentados por perfil.	28/09 a 03/10/2026	Concluído
2. Validação	Revisão técnica e pedagógica com o Orientador; ajustes de terminologia.	04/10 a 06/10/2026	Concluído
3. Limpeza	Exclusão das respostas de teste para garantir a integridade da base de dados.	06/10/2026	Concluído
4. Aplicação	Divulgação dos links junto da comunidade acadêmica e TI via Microsoft Teams.	06/10 a 09/10/2026	Concluído
5. Fecho	Encerramento da coleta e bloqueio de novas submissões.	10/10/2026	Concluído
6. Tabulação	Exportação dos dados e estruturação para análise e levantamento de requisitos.	10/10 a 11/10/2026	Em andamento
3.6. Tratamento e Análise de Dados
Para a interpretação dos resultados, os dados brutos foram exportados da plataforma de coleta e submetidos a duas abordagens de análise:

Análise Quantitativa (Estatística Descritiva): As respostas a perguntas fechadas foram tabuladas automaticamente, gerando gráficos de frequências e percentagens. Este método permitiu quantificar as métricas de usabilidade, como o tempo médio de login, a recorrência de atrasos no início das aulas e a porcentagem de falhas de hardware/software.

Análise Qualitativa (Categorização Temática): As respostas abertas e as observações foram agrupadas em eixos temáticos: (1) Agilidade e Usabilidade no início das aulas; (2) Continuidade Pedagógica; (3) Suporte Técnico; e (4) Governança e Privacidade.

Tratamento de Divergências:
No caso de discrepâncias entre os relatos dos usuários (estudantes/docentes) e as configurações relatadas pela equipe técnica, aplicou-se o método de triangulação. Tais divergências (por exemplo, a percepção de que os arquivos são guardados localmente versus a política de congelamento da máquina) foram registradas não como erros de coleta, mas como indicadores de lacunas na comunicação ou na compreensão do funcionamento atual do ambiente por parte dos usuários. Estes achados servirão de base direta para a formulação dos Requisitos Não Funcionais (RNF) do novo sistema.
