# Plano de Coleta de Dados

## 1. Objetivo da coleta

A etapa de coleta de dados tem como objetivo obter informações suficientes para compreender o funcionamento atual dos laboratórios de informática da FATEC Barueri, especialmente em relação ao processo de acesso aos computadores, identificação dos usuários, permissões, rastreabilidade, operação do ambiente e controles existentes.

As informações obtidas nesta etapa servirão como base para o diagnóstico do cenário atual e para as etapas posteriores do projeto, incluindo:

- identificação e classificação dos riscos;
- levantamento dos requisitos;
- identificação de limitações técnicas e institucionais;
- análise das tecnologias disponíveis;
- avaliação das alternativas de identificação individual;
- comparação das alternativas;
- elaboração de recomendações;
- elaboração do plano de melhoria.

A coleta não possui como objetivo testar ou implantar uma solução neste momento. Seu propósito é compreender o ambiente existente de forma estruturada e reunir evidências suficientes para fundamentar as análises posteriores.

---

## 2. Escopo da coleta

A coleta será direcionada aos aspectos diretamente relacionados ao uso dos computadores dos laboratórios e ao processo de identificação dos usuários.

Serão investigados os seguintes temas:

### 2.1 Ambiente tecnológico

Levantamento das principais características do ambiente dos laboratórios, incluindo:

- quantidade e organização dos laboratórios;
- quantidade aproximada de equipamentos;
- sistemas operacionais utilizados;
- configurações relevantes;
- softwares utilizados nas atividades acadêmicas;
- possíveis diferenças entre os laboratórios;
- dependências de rede;
- mecanismos de gerenciamento dos equipamentos.

### 2.2 Modelo atual de acesso

Levantamento do processo utilizado pelos estudantes para acessar os computadores, incluindo:

- perfis disponíveis;
- credenciais utilizadas;
- processo de início de sessão;
- processo de encerramento de sessão;
- permissões existentes;
- restrições aplicadas aos usuários;
- utilização de contas compartilhadas;
- possíveis diferenças entre ambientes.

### 2.3 Gestão de identidades

Identificação das estruturas institucionais já disponíveis para gerenciamento de usuários, incluindo:

- contas institucionais existentes;
- identificadores utilizados pela instituição;
- utilização do Registro Acadêmico;
- existência de diretórios de usuários;
- mecanismos centralizados de autenticação;
- criação e desativação de contas;
- integração entre sistemas acadêmicos e infraestrutura de TI.

### 2.4 Rastreabilidade

Levantamento dos mecanismos atualmente disponíveis para registrar a utilização dos recursos tecnológicos, incluindo:

- registros de login;
- registros de sessão;
- identificação do equipamento utilizado;
- registros de rede;
- logs disponíveis;
- retenção dos registros;
- possibilidade de associação de uma atividade a um usuário específico;
- limitações existentes.

### 2.5 Restauração das estações

Compreensão do funcionamento dos mecanismos utilizados para restaurar os computadores após sua utilização, considerando:

- momento em que a restauração ocorre;
- informações eliminadas;
- informações preservadas;
- alterações de configuração;
- arquivos armazenados localmente;
- registros de sessão;
- possíveis impactos sobre a rastreabilidade.

### 2.6 Operação e suporte

Identificação de aspectos relacionados ao funcionamento cotidiano dos laboratórios, incluindo:

- problemas mais frequentes;
- dificuldades de acesso;
- necessidade de suporte;
- indisponibilidade dos equipamentos;
- procedimentos utilizados em caso de falha;
- impacto dos problemas durante as aulas;
- capacidade da equipe responsável pelo suporte.

### 2.7 Segurança

Levantamento dos controles existentes relacionados à segurança do ambiente, quando disponíveis e autorizados, incluindo:

- controle de acesso;
- gerenciamento de permissões;
- proteção das contas;
- restrições dos usuários;
- registros de eventos;
- procedimentos relacionados a incidentes.

### 2.8 Privacidade

Identificação dos dados necessários para uma eventual solução de identificação individual, considerando:

- quais identificadores já estão disponíveis;
- necessidade real de utilização de dados pessoais;
- possibilidade de utilização do RA;
- necessidade ou não da utilização do CPF;
- minimização da coleta de dados;
- acesso às informações;
- proteção dos dados utilizados.

### 2.9 Restrições

Identificação de fatores que deverão ser considerados durante a análise das alternativas, como:

- infraestrutura existente;
- disponibilidade de servidores;
- rede;
- equipamentos;
- recursos financeiros;
- licenciamento;
- equipe disponível;
- capacidade de suporte;
- políticas institucionais;
- limitações administrativas;
- requisitos da instituição.

---

## 3. Fontes de informação

A coleta será realizada utilizando diferentes fontes para reduzir a dependência de uma única perspectiva.

As principais fontes previstas são:

| Fonte | Finalidade |
| --- | --- |
| Suporte / Gestão de TI | Obter informações técnicas, operacionais e institucionais sobre o ambiente |
| Docentes | Identificar impactos do modelo atual nas atividades acadêmicas |
| Estudantes | Compreender a experiência prática de utilização dos laboratórios |
| Observação direta | Verificar características do ambiente e complementar as entrevistas |
| Documentação | Confirmar informações e identificar procedimentos formalmente estabelecidos |

A utilização de múltiplas fontes também permitirá comparar informações e identificar possíveis divergências entre o funcionamento previsto e o funcionamento observado na prática.

---

## 4. Instrumentos de coleta

Os instrumentos utilizados nesta etapa estão organizados em arquivos específicos.

```text
03-coleta-dados/
├── plano-coleta.md
├── roteiro-entrevista-suporte.md
├── roteiro-entrevista-docentes.md
├── roteiro-estudantes.md
└── checklist-laboratorio.md
```

### 4.1 Roteiro de entrevista com suporte e gestão

O arquivo `roteiro-entrevista-suporte.md` será utilizado para obter informações técnicas sobre:

- funcionamento atual do acesso;
- contas e perfis existentes;
- permissões;
- identidades institucionais;
- autenticação;
- integrações;
- registros e rastreabilidade;
- restauração das estações;
- problemas recorrentes;
- limitações técnicas;
- restrições institucionais;
- alternativas anteriormente avaliadas.

### 4.2 Roteiro de entrevista com docentes

O arquivo `roteiro-entrevista-docentes.md` será utilizado para compreender:

- funcionamento dos laboratórios durante as aulas;
- dificuldades observadas;
- impactos do modelo atual;
- situações que demandariam identificação do usuário;
- necessidades específicas de disciplinas e softwares;
- possíveis impactos de uma alteração no processo de login;
- requisitos relacionados à utilização acadêmica.

### 4.3 Roteiro para estudantes

O arquivo `roteiro-estudantes.md` será utilizado para compreender:

- experiência atual de acesso;
- dificuldades encontradas;
- necessidade de suporte;
- problemas percebidos durante a utilização;
- percepção sobre a utilização de contas individuais;
- possíveis impactos de uma alteração no processo de acesso.

### 4.4 Checklist de observação

O arquivo `checklist-laboratorio.md` será utilizado para registrar informações diretamente observáveis no ambiente.

A observação será utilizada principalmente para complementar ou validar informações obtidas nas entrevistas.

---

## 5. Estratégia de coleta

A coleta será realizada em etapas para permitir que informações obtidas inicialmente orientem verificações posteriores.

### Etapa 1 — Levantamento inicial

Inicialmente será realizado o levantamento das informações já conhecidas sobre o ambiente.

O objetivo desta etapa é identificar:

- informações já disponíveis;
- informações ainda desconhecidas;
- pessoas que poderão contribuir com a pesquisa;
- documentos existentes;
- pontos que necessitam de confirmação.

### Etapa 2 — Consulta ao suporte e responsáveis

A equipe de suporte e os responsáveis pelo ambiente serão utilizados como principal fonte para compreender a estrutura técnica e operacional dos laboratórios.

Essa etapa deverá fornecer informações sobre:

- configuração atual;
- processo de autenticação;
- administração das contas;
- infraestrutura;
- registros existentes;
- mecanismos de restauração;
- problemas conhecidos;
- limitações;
- possíveis alternativas.

### Etapa 3 — Consulta aos docentes

As entrevistas com docentes serão utilizadas para verificar como o ambiente tecnológico afeta as atividades acadêmicas.

A coleta deverá identificar principalmente:

- dificuldades recorrentes;
- impacto de falhas;
- necessidades específicas;
- comportamento dos estudantes durante as aulas;
- requisitos que uma eventual solução não poderá prejudicar.

### Etapa 4 — Consulta aos estudantes

A consulta aos estudantes será utilizada para complementar a visão técnica e acadêmica com a experiência dos usuários finais.

O objetivo não será realizar levantamento de dados pessoais, mas compreender situações relacionadas ao uso dos computadores.

### Etapa 5 — Observação do ambiente

Quando autorizada, será realizada observação direta dos laboratórios.

A observação terá como finalidade:

- verificar informações relatadas;
- identificar diferenças entre laboratórios;
- compreender o fluxo real de acesso;
- registrar características relevantes;
- identificar pontos que necessitem de investigação adicional.

### Etapa 6 — Validação das informações

Após a coleta inicial, as informações serão consolidadas e comparadas.

Informações consideradas relevantes para o diagnóstico deverão ser confirmadas sempre que possível utilizando:

- outra entrevista;
- observação direta;
- documentação;
- responsável pelo ambiente.

---

## 6. Condução das entrevistas

As entrevistas deverão ser conduzidas de forma semiestruturada.

Os roteiros apresentam as perguntas principais que deverão orientar a conversa, mas perguntas adicionais poderão ser utilizadas quando forem necessárias para esclarecer uma resposta.

As entrevistas não deverão seguir obrigatoriamente uma estrutura rígida.

Caso uma resposta já contemple uma pergunta posterior, não será necessário repetir a mesma questão.

Também poderão ser utilizadas perguntas de aprofundamento, como:

- Pode explicar como isso funciona na prática?
- Pode apresentar um exemplo?
- Isso acontece com frequência?
- Isso ocorre em todos os laboratórios?
- Existem exceções?
- Quem é responsável por esse processo?
- Existe algum registro ou documento relacionado?
- Qual impacto essa situação causa?
- Como esse problema normalmente é resolvido?

Essas perguntas não fazem parte do roteiro principal e devem ser utilizadas apenas quando necessário.

---

## 7. Limitação do tempo dos participantes

Considerando a disponibilidade limitada dos docentes, estudantes e profissionais responsáveis pelo ambiente, os instrumentos foram organizados para reduzir o tempo necessário para cada coleta.

As entrevistas deverão priorizar perguntas capazes de fornecer informações úteis para mais de uma etapa da pesquisa.

Sempre que possível:

- evitar perguntas redundantes;
- não solicitar informações que possam ser obtidas por observação;
- não solicitar ao participante informações que possam ser obtidas em documentos;
- não repetir perguntas já respondidas durante a conversa;
- utilizar perguntas complementares somente quando necessário;
- registrar pendências para posterior verificação em vez de prolongar excessivamente a entrevista.

A qualidade da coleta deverá ser priorizada em relação à quantidade de perguntas realizadas.

---

## 8. Registro das atividades de coleta

Cada atividade deverá receber um identificador próprio.

### Padrão sugerido

```text
COL-001
COL-002
COL-003
```

Para observações diretas:

```text
OBS-001
OBS-002
OBS-003
```

O registro deverá conter, quando aplicável:

- identificador;
- data;
- responsável pela coleta;
- método utilizado;
- objetivo;
- participante ou fonte;
- papel institucional;
- local;
- perguntas aplicadas;
- síntese das respostas;
- documentos consultados;
- evidências relacionadas;
- informações confirmadas;
- informações não confirmadas;
- limitações;
- pendências;
- próximas verificações necessárias.

---

## 9. Classificação das informações

As informações obtidas deverão ser classificadas conforme sua origem e nível de confirmação.

### Relato

Informação fornecida verbalmente ou por escrito por um participante.

Exemplo:

> Um docente relata que o acesso aos computadores algumas vezes atrasa o início da aula.

Esse relato não deverá ser tratado automaticamente como comprovação de que o problema ocorre frequentemente.

### Observação

Informação verificada diretamente pelos pesquisadores.

Exemplo:

> Durante a observação foi identificado que a estação apresenta apenas os perfis definidos para utilização no laboratório.

### Evidência documental

Informação obtida em documento, procedimento, sistema ou registro autorizado.

### Informação validada

Informação confirmada por duas ou mais fontes compatíveis.

Por exemplo:

```text
Relato do suporte
       +
Observação do ambiente
       +
Documento ou registro
       =
Informação validada
```

### Hipótese

Possível explicação para determinado comportamento ou problema que ainda não possui confirmação suficiente.

### Pendente

Informação necessária para o estudo que ainda não foi obtida ou confirmada.

---

## 10. Validação e triangulação

Sempre que possível, informações importantes deverão ser verificadas utilizando mais de uma fonte.

Esse processo será utilizado principalmente para informações que influenciem:

- identificação de riscos;
- classificação de riscos;
- definição de requisitos;
- descarte de alternativas;
- recomendação de tecnologias.

Exemplo:

```text
Suporte informa que determinado registro não existe
                  |
                  v
       Verificação documental
                  |
                  v
       Observação ou confirmação
                  |
                  v
         Resultado consolidado
```

Quando não for possível obter confirmação suficiente, a informação deverá permanecer identificada como relato, hipótese ou pendência.

---

## 11. Evidências

Durante a coleta poderão ser produzidas ou consultadas evidências que auxiliem na validação das informações.

Podem ser consideradas evidências:

- registros de observação;
- documentos institucionais autorizados;
- procedimentos existentes;
- inventários;
- diagramas;
- registros de chamados;
- informações fornecidas formalmente pelos responsáveis;
- capturas de tela autorizadas;
- fotografias autorizadas do ambiente;
- registros técnicos autorizados.

A existência de uma evidência não significa que ela deverá obrigatoriamente ser adicionada ao repositório.

Documentos internos ou informações sensíveis poderão ser apenas consultados e referenciados na pesquisa.

---

## 12. Rastreabilidade das evidências

Sempre que uma informação utilizada no diagnóstico possuir uma evidência associada, deverá ser possível identificar sua origem.

Exemplo:

```text
COL-003
Entrevista com suporte
        |
        v
Informação identificada
        |
        v
EV-005
Evidência relacionada
        |
        v
RIS-002
Risco identificado
```

Essa relação permitirá demonstrar posteriormente como os riscos, requisitos e recomendações foram derivados das informações coletadas.

---

## 13. Relação com as próximas etapas

Os dados coletados não constituirão apenas registros descritivos.

Após a coleta, as informações deverão ser utilizadas para alimentar as etapas seguintes do projeto.

### Coleta para diagnóstico

```text
Coleta
   |
   v
Cenário atual
```

### Coleta para riscos

```text
Problema identificado
        |
        v
Risco associado
        |
        v
Avaliação do risco
```

### Coleta para requisitos

```text
Necessidade ou limitação
          |
          v
Requisito
```

### Coleta para alternativas

```text
Requisitos + Restrições
          |
          v
Pesquisa de alternativas
          |
          v
Comparação
```

Dessa forma, cada informação relevante deverá possuir relação clara com algum elemento posterior da pesquisa.

---

## 14. Documentos a consultar

Quando existentes e mediante autorização, poderão ser consultados documentos relacionados a:

- inventário dos equipamentos;
- configuração dos laboratórios;
- documentação dos perfis;
- políticas de acesso;
- políticas de segurança;
- procedimentos de suporte;
- procedimentos de criação de contas;
- documentação das contas institucionais;
- documentação de autenticação;
- documentação de diretórios;
- documentação de integrações;
- mecanismo de restauração;
- registros de chamados;
- registros de incidentes;
- normas de utilização dos laboratórios.

Não será necessária a inclusão desses documentos no repositório caso contenham informações internas ou sensíveis.

---

## 15. Proteção das informações

A coleta deverá respeitar os princípios de minimização e necessidade.

Não deverão ser solicitados ou armazenados:

- senhas;
- credenciais de acesso;
- CPF de estudantes;
- RA associado à identidade real do estudante;
- listas de usuários;
- dados pessoais sem necessidade para a pesquisa;
- configurações sensíveis que possam comprometer a segurança da instituição.

Quando for necessário demonstrar um processo que utilize informações desse tipo, deverão ser utilizados dados fictícios ou anonimizados.

---

## 16. Limites da coleta

Esta etapa possui finalidade exclusivamente acadêmica e de levantamento.

Não fazem parte da coleta:

- testes de invasão;
- exploração de vulnerabilidades;
- tentativa de quebra de autenticação;
- obtenção de credenciais;
- utilização de contas de terceiros;
- alterações no ambiente;
- instalação não autorizada de programas;
- alteração das configurações das estações;
- interferência nos mecanismos de segurança;
- coleta indiscriminada de logs;
- acesso a informações sem autorização.

Qualquer observação técnica deverá ocorrer dentro das permissões concedidas pela instituição.

---

## 17. Critério de suficiência da coleta

A coleta será considerada suficientemente completa quando houver informações capazes de responder, com nível adequado de confiança, às seguintes questões:

1. Como funciona atualmente o processo de acesso aos computadores?

2. Quais perfis e permissões existem?

3. Quais identidades institucionais estão disponíveis?

4. Como essas identidades são criadas, administradas e desativadas?

5. Quais mecanismos de autenticação já existem?

6. Existem mecanismos de integração que possam ser aproveitados?

7. Quais informações são registradas durante a utilização dos computadores?

8. Qual nível de rastreabilidade existe atualmente?

9. Como a restauração das estações interfere nos dados e registros?

10. Quais problemas relacionados ao modelo atual realmente são observados?

11. Qual é o impacto desses problemas?

12. Quais necessidades são identificadas pela equipe de suporte?

13. Quais necessidades são identificadas pelos docentes?

14. Quais dificuldades são percebidas pelos estudantes?

15. Quais restrições técnicas existem?

16. Quais restrições operacionais existem?

17. Quais restrições institucionais existem?

18. Quais requisitos uma futura solução deverá atender?

19. Quais critérios deverão ser utilizados para avaliar as alternativas?

20. Quais informações ainda permanecem sem confirmação?

Caso questões consideradas essenciais permaneçam sem resposta, deverão ser registradas como pendências e incluídas nas atividades posteriores de coleta.

---

## 18. Resultado final da etapa

Ao final da etapa de coleta deverão ser produzidos insumos suficientes para elaboração de:

- descrição estruturada do cenário atual;
- mapeamento do processo de acesso;
- identificação dos atores envolvidos;
- levantamento dos controles existentes;
- identificação das limitações;
- identificação dos problemas observados;
- matriz de riscos;
- levantamento dos requisitos;
- identificação das restrições;
- definição dos critérios de comparação das alternativas;
- análise das tecnologias disponíveis;
- elaboração das recomendações.

O encerramento desta etapa não significa que novas informações não possam ser coletadas posteriormente.

Caso durante a análise de riscos, requisitos ou alternativas seja identificada alguma lacuna relevante, poderá ser realizada uma coleta complementar, desde que registrada e justificada.

