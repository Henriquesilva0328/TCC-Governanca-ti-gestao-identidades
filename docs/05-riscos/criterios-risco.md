# Critérios de avaliação de riscos

1. Finalidade e referenciais

Este documento registra, antes da construção da matriz de riscos, as regras que serão usadas para classificar cada risco identificado nos laboratórios de informática da Fatec Barueri. Definir os critérios previamente evita que a classificação seja ajustada para confirmar uma solução já escolhida e permite que qualquer leitor refaça a avaliação e chegue ao mesmo resultado. A abordagem adotada é qualitativa e segue os princípios da ABNT NBR ISO 31000:2018 (gestão de riscos), as orientações da ISO/IEC 27005:2022 (gestão de riscos de segurança da informação) e as escalas de probabilidade e impacto propostas pelo NIST SP 800-30 Revisão 1 (2012), mantendo alinhamento com o objetivo de gestão APO12 (Gestão de Riscos) do COBIT 2019, que é a base de governança deste trabalho. Para os aspectos de privacidade, considera-se a Lei Geral de Proteção de Dados Pessoais (Lei nº 13.709/2018), em especial o dever de adotar medidas de segurança previsto em seu artigo 46. Em termos simples, risco é a combinação entre a chance de um problema acontecer (probabilidade) e o tamanho do prejuízo que ele causaria (impacto).

2. Escala adotada e justificativa

Optou-se por uma escala de três níveis (Baixo, Médio e Alto) para probabilidade e para impacto, em vez das escalas de cinco níveis sugeridas pelo NIST. A razão é a natureza das evidências disponíveis: os dados vêm de 20 respostas de estudantes, 3 de docentes e 1 da equipe de TI, sem registros históricos de incidentes. Com esse volume, distinguir cinco graus de probabilidade daria uma aparência de precisão que os dados não sustentam. Três níveis são suficientes para separar o que exige ação prioritária do que pode ser apenas acompanhado, e são de fácil compreensão para gestores e docentes que não atuam com segurança da informação.

3. Critérios de impacto

O impacto é avaliado pela consequência mais grave que o evento pode produzir em qualquer uma das cinco dimensões: atividade acadêmica, operação da TI, integridade dos equipamentos e sistemas, rastreabilidade e proteção de dados pessoais.

Nível	Consequências que caracterizam o nível
Baixo	incômodo pontual, resolvido pelo próprio usuário em poucos minutos, sem perda de trabalho, sem necessidade de acionar a TI e sem exposição de dados pessoais.
Médio	Interrompe parte da aula ou obriga a troca de máquina; exige atendimento da TI; causa perda de trabalho que pode ser refeito; permite uso indevido sem dano permanente; dificulta, mas não impede, a apuração de um incidente.
Alto	compromete a aula ou o laboratório inteiro; causa perda de trabalho sem possibilidade de recuperação; permite alteração ou dano persistente em equipamentos e configurações; expõe dados pessoais de estudantes; impede que a instituição apure responsabilidades sobre um incidente.

4. Critérios de probabilidade

A probabilidade é estimada a partir das informações coletadas, e não da opinião isolada dos autores. Consideram-se a frequência relatada pelos estudantes, a percepção dos docentes, as respostas da equipe de TI e a existência de condições que facilitam o evento, como a senha genérica compartilhada informada pela TI.

Nível	Informações que sustentam o nível

Baixo -	Não há relato do evento e sua ocorrência depende de conhecimento técnico específico ou da combinação de vários fatores.

Médio - O evento foi relatado como raro ou ocasional, ou foi citado por apenas um grupo de respondentes, ou a condição existe, mas exige ação deliberada para ser explorada.

Alto -	O evento foi relatado como frequente, ou foi citado por mais de um grupo (estudantes, docentes e TI), ou a condição está sempre presente e pode ser explorada por qualquer usuário sem conhecimento técnico.

5. Consideração dos controles atuais

A classificação considera o cenário real, isto é, já levando em conta os controles existentes. Cada controle é registrado como efetivo, parcial ou inexistente e só reduz em um nível a probabilidade ou o impacto quando houver evidência de que funciona. Por exemplo, a conta de estudante sem permissão para instalar programas é um controle existente, porém a própria TI relata alunos burlando restrições e acessando a BIOS, o que caracteriza um controle parcial. Da mesma forma, a identificação de usuários pelo cruzamento de câmeras com o mapa de sala do professor é um controle compensatório manual, que depende da colaboração do docente e não substitui um registro automático de quem utilizou cada máquina.

6. Situações sem histórico suficiente

A ausência de registro não será interpretada como ausência de risco. Os dados mostram que os chamados são feitos de forma verbal ou presencial e que os registros do sistema não identificam o estudante porque a conta é genérica. Portanto, a falta de histórico é, ela própria, consequência do problema estudado. Nesses casos, a probabilidade será estimada pela existência e pela facilidade de exploração da condição, e o risco será marcado na matriz como "estimado por condição", indicando que deve ser confirmado com a equipe de TI. Os riscos que poderiam ser introduzidos por uma alternativa futura, como dependência da rede para o login ou aumento de pedidos de redefinição de senha, seguirão as mesmas regras, usando como evidência as preocupações já manifestadas por docentes e pela TI.

7. Classificação final, tratamento e qualidade das evidências

A classificação resulta do cruzamento entre probabilidade e impacto: é Alta quando ambos forem Altos ou quando um for Alto e o outro Médio; é Moderada quando ambos forem Médios ou quando um for Alto e o outro Baixo; e é Baixa nos demais casos. Riscos de classificação Alta terão tratamento prioritário na recomendação; os Moderados serão tratados quando a medida respeitar as restrições informadas pela TI, que exigem custo zero ou ferramentas já licenciadas e baixa manutenção diária; os Baixos poderão ser aceitos e monitorados. As opções de tratamento seguem a ISO/IEC 27005:2022: modificar o risco com controles, retê-lo, evitá-lo ou compartilhá-lo. Cada item da matriz também indicará se se trata de uma limitação do ambiente, de um risco possível ou de um incidente efetivamente relatado. Quando as fontes divergirem, prevalece a fonte mais direta sobre o assunto, a equipe de TI para infraestrutura e os docentes para impacto em aula, e a divergência será registrada. Esse cuidado já se mostrou necessário: o resumo consolidado afirma haver software de congelamento dos discos, enquanto a TI e os docentes responderam que esse mecanismo não é utilizado atualmente.
