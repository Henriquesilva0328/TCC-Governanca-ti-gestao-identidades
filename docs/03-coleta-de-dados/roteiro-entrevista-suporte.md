# 🛠️ Formulário / Roteiro de Pesquisa: Equipe de Suporte e Gestão de TI

**Objetivo:** Mapear tecnicamente a infraestrutura atual dos laboratórios, serviços de diretório/autenticação existentes, políticas de segurança e restrições operacionais/orçamentárias para o projeto.

---

## 📋 Perguntas e Opções do Formulário

### 1. Como funciona atualmente o processo completo de acesso de um aluno a um computador do laboratório?
* ( ) Auto-login (o sistema entra direto sem pedir credenciais).
* ( ) Conta genérica local sem senha ou com senha compartilhada.
* ( ) Conta individual por aluno na rede.
* ( ) Outro: [ Resposta de texto curto ]

### 2. Quais contas ou perfis locais existem configurados nos computadores e quais são suas permissões? *(Marque todas que se aplicam)*
* [ ] Administrador Local (para TI/Professores).
* [ ] Usuário Padrão/Restrito (para Alunos).
* [ ] Conta de Convidado (Guest).
* [ ] Alunos possuem privilégios de Administrador.

### 3. Todos os laboratórios utilizam o mesmo modelo de imagem e padrão de configuração?
* ( ) Sim, ambiente 100% padronizado.
* ( ) Não, existem diferenças técnicas entre salas/laboratórios.

### 4. Como funciona o mecanismo de restauração/congelamento dos computadores (ex: Deep Freeze, Reboot Restore)?
* ( ) A máquina perde TUDO (arquivos, logs e perfis) a cada reinicialização.
* ( ) A máquina é congelada, mas mantém uma partição de dados (ex: Disco D:).
* ( ) Não utilizamos software de congelamento.

### 5. Existe algum serviço centralizado de diretório ou autenticação operando na instituição? *(Marque todos que se aplicam)*
* [ ] Active Directory (AD) On-Premise.
* [ ] Microsoft Entra ID (Azure AD).
* [ ] Google Workspace Educacional.
* [ ] LDAP / FreeIPA.
* [ ] Nenhum (gerenciamento local / Workgroup).

### 6. Os alunos já possuem uma identidade/conta institucional (e-mail ou RA) que possa ser integrada aos computadores?
* ( ) Sim.
* ( ) Não.

### 7. Como é feito o ciclo de vida dessas contas hoje (criação, alteração e bloqueio)?
* ( ) 100% manual pela equipe de TI.
* ( ) Semi-automatizado (scripts em lote via planilhas).
* ( ) 100% automatizado/integrado ao sistema acadêmico.

### 8. Com o modelo atual, as informações salvas ou registradas permitem identificar individualmente quem usou cada computador?
* ( ) Não, os logs são apagados ou não identificam o usuário real.
* ( ) Sim, por meio de logs centralizados de rede/autenticação.
* ( ) Parcialmente (exige cruzamento com câmeras ou lista do professor).

### 9. Quais incidentes técnicos consomem mais tempo do suporte nos laboratórios? *(Marque até 3)*
* [ ] Reset de senhas e bloqueio de contas.
* [ ] Falhas no sistema de congelamento / Atualizações do Windows.
* [ ] Remoção de vírus/malware.
* [ ] Alunos alterando configurações não autorizadas / BIOS.
* [ ] Problemas físicos de hardware e periféricos.

### 10. Quais restrições a futura solução OBRIGATORIAMENTE precisa respeitar?
* [ ] Orçamento zero / Uso exclusivo de ferramentas Open Source ou existentes.
* [ ] Limitação de Hardware legado nos laboratórios.
* [ ] Equipe de TI reduzida (necessidade de baixa manutenção).
* [ ] Regras institucionais de conformidade/LGPD.

### 11. Qual funcionalidade é considerada indispensável em um novo modelo de login individual?
* [ Resposta de texto longo / Parágrafo ]
