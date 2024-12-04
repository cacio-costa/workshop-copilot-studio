# Jornada IA TecBan - Workshop Copilot Studio

## Case 1 - FAQ RH
Elaborar um agente que ofereça ajuda aos colaboradores da sua organização

O RH elaborou uma base de conhecimento, que pode ser acessada neste link: [Link para a base de conhecimento do FAQ](bases-de-conhecimento/faq-rh.txt).

>A base é pequena por fins didáticos e de desempenho (carregamento no Copilot Studio).Ela mescla vários tópicos que, por si só, dariam FAQs próprias (e tópicos também).

### Diretrizes
- Utilize _quick replies_ (respostas rápidas) para facilitar a interação do usuário com os assuntos da FAQ.

## Case 2 - Suporte ao usuário e registro de chamados
Desenvolver um agente para oferecer um primeiro contato de suporte ao usuário.

O agente deve classificar o problema do usuário da seguinte forma:
- Prioridade: [Baixa/Média/Alta]
- Complexidade: [Simples/Moderada/Complexa]

Caso o problema seja de complexidade "Simples" ou "Moderada", o agente deve oferecer alternativas para o usuário tentar resolver o problema por si só. Caso contrário, deve integrar com o sistema de registro de chamados para criar um chamado para o usuário.

> No nosso cenário, realizaremos a integração com o Trello, um software de gestão de tarefas e projetos gratuito.\
>
>Aqui estão os dados necessários para realizar a integração:
>- **URL:** https://api.trello.com/1/cards?idList=67266a505f1e1e9ddc232518&key=cc0d72aa9c80c4ba250686ab91fb9408&token=ATTAd9bf3c10bdf57ef059d99bef4142f79396250287f72eea97092bdc67a8816405D5C3612E
>- **Header:** _Accept: application/json_
>- **Body:**
```json
{
    "name": "[SEU NOME]"
    "desc": "Criado via Copilot Studio"
}
```


## Case 3 - Base de conhecimento para técnicos de campo
Desenvolver um agente para ajudar técnicos de suporte a consultar a base de conhecimento organizacional para resolver problemas com agilidade. 

Também deve dar a possibilidade dos técnicos registrarem soluções para atualizar essa base de conhecimento.

Use esta base de conhecimento: [base de suporte](bases-de-conhecimento/suporte.txt)


## Case 4 - Análise de caso da TecBan
Faça uma análise do cenário atual da TecBan de algum processo ou atividade que você acha que pode ser automatizado com um Agente Copilot.

Implemente uma versão inicial desse chatbot (não precisa ser completo). 

**Dica:** Desenhar o fluxo do processo ajuda a identificar os recursos necessários para implementação da automação:

- Integração com sistemas
- Pontos de interação humana (aprovações, revisões)
- Bases de dados e arquivos necessários

Além disso, fica mais fácil de planejar e implementar o agente de forma iterativa.