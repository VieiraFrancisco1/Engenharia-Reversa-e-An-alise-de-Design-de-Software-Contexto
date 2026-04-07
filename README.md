#Engenharia Reversa e Análise de designe de Software 

PARTE 1 – Compreensão do Sistema
01. Qual é o objetivo do sistema?

O sistema tem como objetivo realizar o controle básico de pedidos de uma pastelaria, permitindo que o usuário selecione produtos, informe a quantidade e visualize o valor total da compra.

Trata-se de uma aplicação simples, voltada para simular um cenário real de vendas.

02. Quais são suas principais funcionalidades?
Seleção de produtos (pastel, caldo, refrigerante, etc.)
Inserção da quantidade desejada
Adição de itens ao pedido
Listagem dos itens adicionados
Cálculo automático do valor total
Finalização do pedido
03. Como o usuário interage com o sistema?

O usuário interage por meio de uma interface web simples, onde:

Seleciona o produto em um campo de escolha
Informa a quantidade
Clica no botão para adicionar o item
Visualiza os itens adicionados na lista
Acompanha o valor total sendo atualizado

A interação é direta e de fácil entendimento.

PARTE 2 – Identificação de Elementos
01. Quais são as principais funções do sistema?

Com base no funcionamento, as principais funções envolvem:

Adicionar itens ao pedido
Atualizar a lista de itens
Calcular o valor total
Finalizar o pedido
02. Quais dados são manipulados?

O sistema trabalha com os seguintes dados:

Nome do produto
Quantidade
Preço unitário
Subtotal de cada item
Valor total do pedido

Esses dados são utilizados para compor a lógica do sistema.

03. Quais entidades podem ser extraídas?

Mesmo sem uso explícito de classes, é possível identificar algumas entidades importantes:

Produto
ItemPedido
Pedido

Essas entidades representam a estrutura lógica do sistema.

PARTE 3 – Arquitetura
01. O sistema possui arquitetura definida?

O sistema não apresenta uma arquitetura formal definida.

Ele é composto por arquivos separados de HTML, CSS e JavaScript, porém a lógica está concentrada no JavaScript sem divisão em camadas.

02. Ele segue algum padrão (MVC, camadas, etc.)?

Não há evidências da aplicação de padrões como MVC.

A lógica de negócio e a manipulação da interface estão diretamente conectadas.

03. Como você classificaria esse sistema?

O sistema pode ser classificado como uma aplicação simples, com estrutura monolítica, adequada para fins educacionais e de aprendizado.

PARTE 4 – Modelagem (UML)

Considerando uma melhor organização, o sistema poderia ser modelado com as seguintes classes:

Produto
nome
preco
ItemPedido
produto
quantidade
subtotal
Pedido
itens
total
Relacionamentos:
Um Pedido possui vários ItemPedido
Um ItemPedido está associado a um Produto

Essa modelagem representa de forma mais estruturada os dados do sistema.

PARTE 5 – Análise de Problemas
Coesão

A coesão pode ser considerada média, pois algumas funções podem estar realizando mais de uma responsabilidade ao mesmo tempo.

Acoplamento

O acoplamento é relativamente alto, já que o sistema depende diretamente da estrutura do HTML para funcionar corretamente.

Interface

A interface é simples e funcional, porém pode ser aprimorada em alguns aspectos:

Falta de validação de dados de entrada
Ausência de mensagens de erro ou feedback ao usuário
Possibilidade de exibição de valores inconsistentes
Lógica

A lógica do sistema está diretamente integrada com a interface, o que pode dificultar a manutenção e evolução do código.

Organização geral

O sistema apresenta uma estrutura funcional, porém com pouca separação de responsabilidades, o que pode impactar sua organização em cenários mais complexos.

PARTE 6 – Propostas de Melhoria
Separar a lógica da interface (melhor organização do código)
Criar classes para representar as entidades do sistema
Aplicar padrões de projeto, como Factory e Singleton
Implementar validações de entrada
Melhorar o feedback visual para o usuário
Organizar melhor as funções, evitando múltiplas responsabilidades
