# Requisitos funcionais

Este documento reúne os requisitos funcionais identificados a partir do diagnóstico do ambiente e das necessidades dos usuários.

Os requisitos deverão descrever as funcionalidades esperadas de uma possível solução de identificação individual e controle de acesso aos computadores dos laboratórios.

---

## 1. Estrutura Padrão dos Requisitos
Cada Requisito Funcional contém as seguintes propriedades:
* **ID:** Identificador único do requisito.
* **Descrição:** O que a solução deve realizar.
* **Origem / Evidência:** Código da necessidade ou evidência apurada na coleta de dados.
* **Justificativa:** Motivo técnico/acadêmico da implementação.
* **Prioridade:** Alta, Média ou Baixa.
* **Dependências:** Requisitos ou infraestruturas pré-existentes.
* **Forma de Verificação:** Como o cumprimento será testado no piloto.

---

## 2. Lista de Requisitos Funcionais

| ID | Descrição | Origem / Evidência | Justificativa | Prioridade | Dependências | Forma de Verificação |
| :---: | :--- | :---: | :--- | :---: | :---: | :--- |
| **RF01** | **Autenticação Individualizada no AD:** O sistema deve autenticar individualmente estudantes e docentes através do Active Directory (AD DS), substituindo contas locais genéricas. | `COL-001` | Garantir a individualização e a responsabilidade pelo uso das estações de trabalho, em conformidade com a LGPD. | **Alta** | Infraestrutura de DC (Domain Controller) ativa | Tentativa de logon no domínio `fatec.local` com credencial pessoal do aluno/docente. |
| **RF02** | **Sincronização AD x GLPI via LDAPS:** O GLPI deve sincronizar automaticamente a base de utilizadores do Active Directory através de ligação encriptada. | `COL-003` | Evitar o recadastro manual de utilizadores na plataforma de ITSM e automatizar a gestão de identidades. | **Alta** | `RF01`, Serviço LDAPS na porta 636 | Consulta de utilizadores no GLPI validando a importação direta dos diretórios do AD. |
| **RF03** | **Abertura e Vínculo Automático de Chamados:** Ao abrir um chamado no GLPI a partir de um perfil autenticado, o sistema deve associar automaticamente o utilizador, o laboratório e a máquina. | `COL-003` | Eliminar o suporte informal de balcão e garantir o histórico e rastreabilidade de falhas por equipamento. | **Média** | `RF01`, `RF02` | Submissão de chamado no GLPI por utilizador autenticado verificando o autopreenchimento dos campos. |
| **RF04** | **Registo e Auditoria de Acessos (*Logon/Logoff*):** O Active Directory deve registar centraladamente os eventos de *logon* e *logoff*, armazenando utilizador, IP, máquina e data/hora. | `COL-004` | Permitir auditoria técnica em caso de incidentes de segurança ou danos materiais nas bancadas. | **Alta** | `RF01` | Leitura dos logs de auditoria no Visualizador de Eventos do Windows Server. |
| **RF05** | **Perfis de Usuário e Redirecionamento de Pastas:** O sistema deve aplicar Políticas de Grupo (GPOs) para redirecionar pastas do utilizador (ex: Documentos) para um diretório de rede persistente. | `COL-005` | Evitar a perda de ficheiros decorrente do reinício (*reboot*) das máquinas com congelamento de disco. | **Alta** | `RF01`, Servidor de Ficheiros (File Server) | Gravação de ficheiro na pasta Documentos, reinício do computador e verificação do ficheiro pós-logon. |
