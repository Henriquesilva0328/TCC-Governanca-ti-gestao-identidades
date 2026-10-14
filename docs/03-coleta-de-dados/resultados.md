# Resultados da Coleta de Dados por Eixos Temáticos

---

## 1. Introdução e Agrupamento Temático
Esta seção consolida e agrupa as respostas obtidas na pesquisa de campo com estudantes, equipe de TI e corpo docente, dividindo-as por eixos temáticos críticos para a operação e a experiência de uso nos laboratórios da FATEC Barueri.

---

## 2. Análise detalhada por Eixos Temáticos

### A. Início das Aulas e Tempo de Logon
* **Respostas Agrupadas:** Alunos e professores relataram morosidade generalizada ao iniciar as estações de trabalho.
* **Necessidade Recorrente:** Reduzir o tempo de espera no início do período letivo.
* **Evidências:** 80% dos estudantes respondentes apontaram extrema lentidão no login como principal entrave; docentes estimam uma perda de 10 a 15 minutos úteis de aula.
* **Corroboração:** A observação direta in loco confirmou o travamento e a demora no carregamento associados aos perfis locais genéricos.

### B. Preservação de Arquivos e Armazenamento (Congelamento de Disco)
* **Respostas Agrupadas:** Preocupação unânime com a perda de ficheiros decorrente do reinício das máquinas.
* **Necessidade Recorrente:** Garantir a persistência de dados acadêmicos sem comprometer a política de limpeza e restauração do sistema operacional.
* **Evidências:** Relatos recorrentes de perda de trabalhos práticos que não foram salvos externamente antes do *reboot* das bancadas.

### C. Suporte Técnico e Gestão de Chamados
* **Respostas Agrupadas:** Forma de tratamento de falhas e abertura de ocorrências.
* **Necessidade Recorrente:** Rastreabilidade e histórico centralizado de incidentes vinculados à máquina e ao utilizador.
* **Evidências:** Entrevistas com a equipe de TI indicaram a ausência de vínculo automatizado de chamados no GLPI, predominando o suporte verbal de balcão.

### D. Permissões, Softwares e Perfil de Acesso
* **Respostas Agrupadas:** Necessidade de utilização de ferramentas de desenvolvimento e pacotes específicos sem conceder privilégios indevidos de administrador local aos discentes.

### E. Privacidade, Expectativas e Mudanças
* **Respostas Agrupadas:** Expectativa amplamente positiva quanto à individualização de contas, desde que os procedimentos de recuperação de credenciais sejam ágeis e respeitem as diretrizes da LGPD.

---

## 3. Síntese de Necessidades e Evidências

| Eixo Temático | Necessidade Identificada | Evidência / Fonte | Tipo de Ocorrência |
| :--- | :--- | :--- | :--- |
| **Autenticação** | Contas individuais para auditoria e segurança | `COL-001` (Formulário Discente) | Recorrente (80%) |
| **Desempenho** | Logon rápido ($\le 30$ segundos) para preservar o tempo de aula | `COL-002` (Formulário e Docentes) | Recorrente |
| **Armazenamento** | Diretório de rede persistente contra limpeza pós-reboot | `COL-005` (Entrevista TI e Alunos) | Recorrente |
| **Gestão de TI** | Integração AD-GLPI para chamados rastreáveis | `COL-003` (Entrevista TI) | Corroborada |

---

## 4. Limitações da Coleta
* **Amostra:** Os dados quantitativos fundamentam-se em 20 respostas discentes dos cursos de GTI e DSM, representando uma amostra indicativa e analítica, e não a totalidade do corpo discente da FATEC Barueri.
* **Viés de Autorrelato:** As respostas qualitativas refletem a perceção subjetiva e a experiência relatada pelos participantes no momento da aplicação dos instrumentos.
