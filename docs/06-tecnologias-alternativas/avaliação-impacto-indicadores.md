# Avaliação do Impacto Acadêmico das Alternativas e Indicadores para Piloto

---

## 1. Avaliação do Impacto Acadêmico e Cotidiano das Alternativas

Com base nas alternativas de arquitetura levantadas pela frente de Governança e Riscos (Lucas), avalia-se o impacto direto na experiência do usuário (estudantes e docentes) e na rotina das aulas práticas:

### Alternativa A: Manutenção do Modelo Atual (Contas Genéricas Locais)
* **Utilização Cotidiana:** O aluno escolhe qualquer máquina e acessa imediatamente com uma conta genérica local.
* **Dificuldades e Impactos:**
  * Inexistência de rastreabilidade e de responsabilidade individual por acções na máquina.
  * Perda inevitável de arquivos no *reboot* devido ao congelamento de disco sem drive de rede.
  * Abertura informal de chamados, gerando atrasos na resolução de falhas recorrentes.
* **Avaliação de UX:** **Inadequada** para o cenário acadêmico atual.

### Alternativa B: Solução Cloud Nativa (Entra ID / Azure AD)
* **Utilização Cotidiana:** Autenticação via nuvem integrada ao e-mail institucional do estudante.
* **Dificuldades e Impactos:**
  * Dependência crítica de conectividade externa constante com a Internet para autenticação no início da aula.
  * Maior complexidade de usabilidade para gestão de privilégios locais de software de laboratório sem infraestrutura híbrida.
* **Avaliação de UX:** **Viável**, porém sujeita a instabilidades de link externo de Internet.

### Alternativa C (Proposta): Active Directory On-Premise + GLPI via LDAPS
* **Utilização Cotidiana:** Autenticação individual rápida na rede local, com mapeamento automático de pasta de documentos persistente e abertura simples de chamados no GLPI.
* **Dificuldades e Impactos:**
  * Necessidade inicial de orientação e comunicação transparente quanto ao uso de senhas individuais e boas práticas de logout.
* **Avaliação de UX:** **Ideal**, pois garante alta disponibilidade na rede local, rapidez no login e proteção dos dados dos discentes.

---

## 2. Orientações de Usabilidade e Comunicação de Mudanças

Para assegurar uma transição suave na adoção da solução proposta:
1. **Guia Rápido de Primeiro Acesso:** Material impresso/digital simples nas bancadas detalhando a estrutura das credenciais e a importância de salvar arquivos no diretório de rede.
2. **Alertas Visuais na Tela de Logout:** Avisos para reforçar o encerramento formal da sessão para evitar que o perfil permaneça aberto.
3. **Procedimento de Redefinição de Senha:** Fluxo simplificado para que o suporte de TI possa restaurar o acesso em menos de 5 minutos durante a aula.

---

## 3. Indicadores Propostos para Validação em Piloto Futuro

Para medir objetivamente o sucesso do piloto nos laboratórios, propõem-se os seguintes indicadores (KPIs):

| Indicador | Métrica Target | Método de Coleta | Limitações da Coleta |
| :--- | :---: | :--- | :--- |
| **1. Tempo Médio de Logon (TMA)** | $\le 30$ segundos | Scripts automatizados de auditoria no Active Directory e cronometragem em amostragem. | Varia de acordo com a carga de rede e a quantidade de logins simultâneos no início da aula. |
| **2. Taxa de Retenção e Perda de Arquivos** | $0$ incidentes de perda relatados | Questionário curto aplicado aos estudantes ao final do período do piloto. | Depende da adesão do aluno em salvar os arquivos na pasta de rede correta. |
| **3. Volume de Chamados por Falha de Acesso** | Redução de $50\%$ | Relatórios e métricas extraídos diretamente da plataforma GLPI. | Requer que 100% dos incidentes sejam registrados formalmente na ferramenta. |
| **4. Usabilidade Percebida (SUS)** | Pontuação $> 75/100$ | Escala SUS (*System Usability Scale*) aplicada a discentes e docentes. | Medição baseada na percepção subjetiva dos participantes. |
