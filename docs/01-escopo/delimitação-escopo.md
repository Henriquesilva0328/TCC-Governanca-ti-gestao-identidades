## 1. Objetivo da Delimitação
Esta seção define claramente a fronteira do projeto de TCC. O propósito é examinar cada dificuldade relatada durante a pesquisa de campo e responder a duas questões centrais:
1. *Esta dificuldade continuaria a existir com a adoção de contas individuais via Active Directory e integração com o GLPI?*
2. *Quais medidas específicas da proposta enfrentam essa dificuldade, e o que funciona bem atualmente e deve ser preservado?*

---

## 2. Matriz de Relação entre Dificuldades e Proposta (AD + GLPI)

| Dificuldade Relatada na Coleta | Pertence ao Escopo da Proposta? | Como a Proposta (AD + GLPI) Enfrenta o Problema? | O que Funciona Atualmente e Precisa Ser Preservado? |
| :--- | :---: | :--- | :--- |
| **Uso de contas genéricas e anônimas** nas bancadas de laboratório. | **Sim** | Implementação de diretório centralizado com autenticação individual obrigatória para cada aluno e docente. | A infraestrutura física das bancadas e os computadores atuais. |
| **Perda de arquivos** no reinício dos computadores (*reboot* por congelamento de disco). | **Sim** | Aplicação de Políticas de Grupo (GPOs) com redirecionamento de pastas para um diretório de rede persistente. | O software de restauração do sistema operacional (congelamento) que protege contra alterações indevidas no sistema. |
| **Falta de rastreabilidade** de incidentes e abertura informal de chamados. | **Sim** | Sincronização automatizada de utilizadores via LDAPS e abertura de chamados no GLPI vinculados ao perfil e à máquina. | A cordialidade e a disponibilidade do suporte presencial de balcão. |
| **Lentidão extrema de logon** e falhas gerais de hardware/rede. | **Parcial** | O AD otimiza o carregamento de perfis de rede, mas gargalos de hardware físico dependem de manutenções locais. | As manutenções preventivas e rotinas periódicas de limpeza física realizadas pela TI. |
| **Dificuldade de execução de softwares** específicos sem privilégios de administrador. | **Sim** | Configuração centralizada de permissões e políticas de segurança via GPO para perfis acadêmicos específicos. | O isolamento de segurança que impede modificações destrutivas no sistema operacional. |

---

## 3. Conclusão da Delimitação
* **Dentro do Escopo:** Tudo o que diz respeito à **gestão de identidades, autenticação centralizada, segurança de perfis de rede, auditoria de acessos e integração com o sistema de chamados (GLPI)**.
* **Fora do Escopo (Demandam outras melhorias):** Substituição de ativos físicos de hardware, reestruturação da cablagem de rede estruturada e atualizações de licenças de software de terceiros que não dependem do serviço de diretório.
