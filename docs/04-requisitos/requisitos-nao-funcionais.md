# Requisitos não funcionais

Este documento apresenta os requisitos relacionados à qualidade, desempenho, disponibilidade, usabilidade e compatibilidade de uma possível solução.

O objetivo é estabelecer condições que deverão ser consideradas na avaliação das alternativas tecnológicas, respeitando as características do ambiente institucional.

## 1. Lista de Requisitos Não Funcionais

| ID | Categoria | Descrição Técnica e Métrica | Origem / Evidência | Justificativa | Prioridade | Forma de Verificação |
| :---: | :--- | :--- | :---: | :--- | :---: | :--- |
| **RNF01** | **Desempenho** | **Tempo de Logon:** O tempo total de autenticação e carregamento inicial do perfil do utilizador deve ser **$\le 30$ segundos** nas estações do laboratório. | `COL-002` | Evitar o desperdício de 10 a 15 minutos de tempo útil de aula no início de cada período. | **Alta** | Cronometragem do tempo entre a submissão das credenciais e a disponibilidade do ambiente de trabalho. |
| **RNF02** | **Segurança e Criptografia** | **Comunicação LDAPS:** Toda a comunicação de autenticação e consulta de diretório entre o GLPI e o AD deve utilizar o protocolo LDAPS encriptado (TLS/SSL na porta 636). | `OBS-001` | Proteger credenciais e dados de consulta contra a interceção (*sniffing*) na rede local. | **Alta** | Análise de tráfego de rede via Wireshark confirmando encriptação TLS na porta 636. |
| **RNF03** | **Privacidade e LGPD** | **Limpeza Local Pós-Sessão:** O sistema não deve manter cópias locais permanentes de ficheiros ou dados pessoais dos utilizadores no disco local pós-*logoff*. | `COL-005` | Cumprir as diretrizes da Lei Geral de Proteção de Dados (Lei nº 13.709/2018) e assegurar a privacidade. | **Alta** | Verificação da pasta local de perfis pós-logoff constatando a remoção de dados temporários. |
| **RNF04** | **Disponibilidade** | **Disponibilidade do Serviço:** O serviço de autenticação do Active Directory na rede local deve manter uma disponibilidade de **99,5%** durante o horário letivo. | `COL-002` | Impedir a paralisação das atividades letivas em caso de falha pontual de rede ou servidor. | **Alta** | Verificação de logs de uptime do controlador de domínio no período de teste do piloto. |
| **RNF05** | **Usabilidade** | **Facilidade de Uso e Acessibilidade:** As ecrãs de autenticação e abertura de chamados devem manter o padrão de mercado (Windows logon e interface Web responsiva). | `OBS-001` | Minimizar a curva de aprendizagem de discentes e docentes sem necessidade de treino complexo. | **Média** | Aplicação de teste de usabilidade percebida com formulário simplificado pós-uso. |
