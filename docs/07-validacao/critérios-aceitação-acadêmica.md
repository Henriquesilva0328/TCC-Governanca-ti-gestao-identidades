# Condições de Utilização Acadêmica e Critérios de Aceitação

---

## 1. Objetivo
Esta seção especifica as condições reais e cotidianas de utilização dos laboratórios de informática durante as aulas práticas, estabelecendo os critérios de aceitação toleráveis para que a solução integrada (Active Directory + GLPI) atenda às expectativas de discentes e docentes sem criar gargalos operacionais.

---

## 2. Cenários Acadêmicos Concretos e Critérios de Aceitação

### A. Troca de Estação de Trabalho durante a Aula
* **Cenário:** Um estudante precisa mudar de computador durante a aula devido a falha pontual no monitor, periférico ou bancada.
* **Comportamento Esperado:** O perfil móvel/redirecionado deve carregar a área de trabalho e os ficheiros do aluno na nova máquina de forma ágil.
* **Critério de Aceitação:** O tempo total de login e disponibilização das pastas de rede na nova estação deve ser **$\le 20$ segundos**, sem perda dos dados salvos na sessão anterior.

### B. Esquecimento de Senha e Conta Bloqueada
* **Cenário:** O estudante ou professor esquece a palavra-passe ou bloqueia a conta por tentativas incorretas consecutivas no início da aula.
* **Comportamento Esperado:** O procedimento de redefinição de credencial deve ser simples e operado pela equipe de TI via painel centralizado ou ferramenta de autoatendimento.
* **Critério de Aceitação:** O tempo médio de resolução e retorno do aluno às atividades letivas deve ser de no máximo **5 minutos**.

### C. Estudante Recém-Ingresso ou Não Cadastrado
* **Cenário:** Aluno matriculado recentemente ou transferido que ainda não possui credencial gerada no Active Directory.
* **Comportamento Esperado:** A GPO deve prever uma conta temporária com privilégios restritos e expiração automática, ou permitir a criação/importação em lote rápida via script.
* **Critério de Aceitação:** A liberação de acesso temporário autorizado deve ocorrer em até **3 minutos** durante a aula.

### D. Execução de Softwares Acadêmicos Específicos
* **Cenário:** Disciplinas práticas que exigem ferramentas de desenvolvimento, máquinas virtuais ou pacotes com acesso a portas/serviços específicos.
* **Comportamento Esperado:** As Políticas de Grupo (GPOs) devem conceder as permissões necessárias para a execução dos softwares da ementa sem conceder privilégios de Administrador Local permanente ao aluno.
* **Critério de Aceitação:** 100% dos softwares das disciplinas de GTI e DSM devem ser executados sem mensagens de erro de permissão negada.

---

## 3. Justificativa dos Valores e Tolerâncias

| Parâmetro | Valor Definido | Justificativa Acadêmica |
| :--- | :---: | :--- |
| **Tempo de Login Inicial** | $\le 30$ segundos | Garantir que o início da aula não seja impactado (restringindo a perda ao limite aceitável de 1 minuto por turma). |
| **Troca de Máquina** | $\le 20$ segundos | Impedir que falhas de periféricos paralisem o andamento do exercício prático do aluno. |
| **Reset de Senha** | $\le 5$ minutos | Evitar que o estudante perca a explicação de um bloco de aula por pendência de credencial. |
