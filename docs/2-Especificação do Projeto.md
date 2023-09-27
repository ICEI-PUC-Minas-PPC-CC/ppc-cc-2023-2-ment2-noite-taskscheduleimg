# Especificações do Projeto

<span style="color:red">Pré-requisitos: <a href="1-Documentação de Contexto.md"> Documentação de Contexto</a></span>

## Personas

**PRIMEIRA PERSONA**

|**João Silva**|           |                             | 
|-------------------|-----------|-----------------------------|
<img src="https://github.com/ICEI-PUC-Minas-PPC-CC/ppc-cc-2023-2-ment2-noite-taskscheduleimg/blob/main/docs/img/download.jpeg?raw=true" width="200" height="200"/>|**Idade:** 42 anos. **Naturalidade:** Belo Horizonte - Minas Gerais. **Ocupação:** Coordenador de Suporte Técnico.       |**Atribuições:** João é responsável por coordenar a equipe de suporte técnico da faculdade, alocando funcionários para tarefas de assistência e garantindo que as solicitações sejam tratadas de forma eficiente. 
|**Motivações:** Ele busca otimizar a alocação de recursos, melhorar a eficiência do suporte e proporcionar uma experiência de suporte mais rápida e eficaz para a comunidade acadêmica.  |**Frustações:** João frequentemente lida com a sobrecarga de trabalho e o desafio de priorizar tarefas com base na gravidade e urgência das solicitações. Ele também enfrenta dificuldades em identificar rapidamente as solicitações que requerem conhecimento específico.   |**Hobbies, história:** João gosta de ler sobre inovações tecnológicas e dedica seu tempo livre a atividades ao ar livre, como caminhadas.

**SEGUNDA PERSONA**

|**Maria Oliveira**|           |                             | 
|-------------------|-----------|-----------------------------|
<img src="https://github.com/ICEI-PUC-Minas-PPC-CC/ppc-cc-2023-2-ment2-noite-taskscheduleimg/blob/main/docs/img/download%20(1).jpeg?raw=true" width="200" height="200"/>|**Idade:** 29 anos. **Naturalidade:** São Paulo - São Paulo. **Ocupação:** Funcionária de Suporte Técnico.       |**Atribuições:**  Maria trabalha no suporte técnico da faculdade, onde recebe solicitações de assistência de alunos e professores. Ela precisa avaliar as solicitações, designar tarefas aos funcionários apropriados e fornecer suporte eficaz.
|**Motivações:** Maria busca fornecer um suporte de alta qualidade e contribuir para a satisfação dos usuários. Ela deseja reduzir o tempo de resposta e garantir que as solicitações sejam atendidas de forma eficiente.  |**Frustações:** Maria fica frustrada quando não consegue designar tarefas rapidamente devido à falta de informações claras nas solicitações. Ela também se sente sobrecarregada quando as tarefas não são distribuídas de forma eficaz.   |**Hobbies, história:** Nos fins de semana, Maria gosta de participar de grupos de teatro amador e é apaixonada por literatura clássica.

## Histórias de Usuários

Com base na análise das personas, foram identificadas as seguintes histórias de usuários:

Exemplo:

|EU COMO... `PERSONA`| QUERO/PRECISO ... `FUNCIONALIDADE` |PARA ... `MOTIVO/VALOR`                 |
|--------------------|------------------------------------|----------------------------------------|
| João Silva | Otimizar a alocação de recursos da equipe de suporte técnico | Melhorar a eficiência do suporte acadêmico da faculdade. |
| Maria Oliveira | De uma interface de usuário intuitiva | Identificar rapidamente palavras-chave nas solicitações de suporte e designar tarefas de forma rápida e precisa. |

### Requisitos Funcionais

|ID    | Descrição do Requisito  | Prioridade |
|------|-----------------------------------------|----|
|RF-001| O sistema deverá automatizar a designação de tarefas conforme a área do problema (EX: Hardware / Software) | ALTA | 
|RF-002| O sistema deverá estabelecer uma relação entre Título e Descrição da ocorrência para uma maior assertividade na designação | ALTA |
|RF-003| O sistema deverá, ao final de cada prestação de serviço, gerar um relatório do que foi feito | ALTA |
|RF-004| O sistema deverá apresentar uma ferramenta de filtragem, relacionando respectivos prestadores de serviços e suas funções| MÉDIA | 


### Requisitos não Funcionais

|ID     | Descrição do Requisito  |Prioridade |
|-------|-------------------------|----|
|RNF-001| O sistema deverá usar a ferramenta de machine learning C.L.U | ALTA | 
|RNF-002| O sistema deverá ser integrado ao CRC da PUC MINAS |  ALTA | 
