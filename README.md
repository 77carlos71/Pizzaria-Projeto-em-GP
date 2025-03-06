# Sistema de Gerenciamento de Pizzaria

Este é um sistema desenvolvido em Python utilizando o framework Flet para criar uma interface gráfica de gerenciamento de uma pizzaria. Ele permite o cadastro de clientes, pizzas e pedidos, além de funcionalidades como exportação de dados para Excel, geração de PDFs para pedidos e envio de mensagens automáticas via WhatsApp.

## Funcionalidades

### Cadastro de Clientes
- Adicionar, editar e deletar clientes.
- Campos: Nome, Telefone, CPF, CEP, Endereço e Número.
- Pesquisa automática de endereço via API do ViaCEP com base no CEP informado.
- Pesquisa de clientes por nome.

### Cadastro de Pizzas
- Adicionar, editar e deletar pizzas.
- Campos: Nome e Ingredientes.
- Pesquisa de pizzas por nome.

### Gerenciamento de Pedidos
- Criar, visualizar e cancelar pedidos.
- Campos: Código (gerado automaticamente), Cliente, Pizza, Quantidade, Tamanho, Forma de Pagamento, Entrega, Valor Total, Status e Data/Hora.
- Cálculo automático do valor total com base no tamanho, quantidade, taxa de entrega e forma de pagamento.
- Atualização de status do pedido (Preparando → Entregando → Concluído ou Cancelado).
- Filtros por mês, ano e tipo de entrega.
- Geração de PDF com detalhes do pedido.
- Envio de mensagens automáticas via WhatsApp para o cliente em diferentes etapas do pedido (salvo, enviado, concluído, cancelado).

### Exportação de Dados
- Exporta os dados de clientes, pizzas e pedidos para arquivos Excel.

### Interface Gráfica
- Interface amigável construída com Flet.
- Suporte a temas claro e escuro com ajustes automáticos de cores.
- Tabelas paginadas com botões de ação (editar, deletar, visualizar).

## Tecnologias Utilizadas
- **Python 3.x**
- **Flet**: Framework para interface gráfica.
- **SQLite3**: Banco de dados leve para armazenamento.
- **Pandas**: Manipulação e exportação de dados para Excel.
- **Requests**: Integração com a API ViaCEP.
- **Selenium**: Automação do envio de mensagens via WhatsApp.
- **FPDF**: Geração de PDFs para pedidos.

## Pré-requisitos
- Python 3.8 ou superior instalado.
- Firefox instalado (necessário para o Selenium enviar mensagens via WhatsApp).
- Perfil do Firefox configurado (necessário ajustar o caminho do perfil no código).
