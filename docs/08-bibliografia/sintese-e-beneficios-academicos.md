adêmicos Esperados

**Projeto:** Gestão de Identidades e Controle de Acesso aos Laboratórios de Informática  
**Instituição:** FATEC Barueri  
**Responsável (Frente Metodologia e UX):** Pedro Henrique  
**Caminho no Repositório:** `docs/08-bibliografia/sintese-e-beneficios-academicos.md`  

---

## 1. Encadeamento Lógico: Coleta $\rightarrow$ Requisitos $\rightarrow$ Benefícios

A proposta de valor do TCC fundamenta-se na rastreabilidade total entre o diagnóstico empírico e a solução tecnológica recomendada:

[Diagnóstico de Campo]  --->  [Requisito Especificado]  --->  [Benefício Acadêmico Direto]
Contas genéricas / anônimas  -> RF01 (Autenticação AD)     -> Rastreabilidade e conformidade LGPD
Lentidão de 10-15 min/aula   -> RNF01 (Logon <= 30s)       -> Recuperação do tempo letivo útil
Perda de dados pós-reboot    -> RF05 (GPO Redirecionada)   -> Segurança e integridade de trabalhos
Suporte informal sem registro-> RF02/03 (AD + GLPI)        -> Gestão eficiente e histórico de TI


---

## 2. Distinção Metodológica: Diagnóstico Real vs. Projeções Futuras

Para rigor acadêmico na elaboração do TCC, estabelece-se a separação formal entre os fatos observados e os ganhos projetados:
* **Diagnóstico Real Apurado (Fato):** Constatação da perda de tempo pedagógico, invisibilidade de chamados no GLPI, ausência de logs individuais e insatisfação com a perda acidental de arquivos locais.
* **Projeção de Benefícios Futuros (Hipótese Validada no Piloto):** Aumento de até 15% no aproveitamento do tempo prático de aula, redução do volume de chamados repetitivos de suporte e conformidade legal total com a LGPD.

---

## 3. Diretrizes para Ações de Comunicação e Orientação (Entregável para o Henrique)

Para garantir a adesão dos usuários na transição de modelo, recomenda-se à frente de Comunicação a preparação dos seguintes materiais:
1. **Guia de Boas Práticas do Usuário (1 página PDF/Impresso):**
   * Como realizar o primeiro acesso com a credencial institucional.
   * Onde salvar os arquivos para garantir backup na nuvem/servidor de rede (Redirecionamento de Pastas).
   * Importância do *Logoff* ao término da aula para proteger os dados pessoais.
2. **Procedimento de Suporte Rápido para Docentes:**
   * Orientações para abertura rápida de chamados via GLPI em caso de falhas em bancadas específicas.

---

## 4. Estrutura Base para a Apresentação Técnica do TCC

A apresentação das frentes de Metodologia, UX e Requisitos deve seguir a sequência:
1. **Problema e Contexto:** A rotina atual dos laboratórios da FATEC Barueri e o impacto no tempo letivo.
2. **Metodologia de Pesquisa:** Triangulação (Estudantes, TI e Docentes) e conformidade ética (LGPD).
3. **Achados Principais:** Percentuais, matriz de necessidades e delimitação do escopo.
4. **Requisitos e Indicadores:** Como os requisitos (RF/RNF) respondem diretamente aos problemas diagnosticados e como o piloto será medido.
