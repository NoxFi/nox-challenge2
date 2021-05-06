
![N|Solid](https://www.noxbitcoin.com.br/wp-content/uploads/2021/05/nox-logo-desafio.png)

Neste desafio será avaliado tanto seu conhecimento técnico, quanto a sua capacidade de entender um domínio de problema.
Todos as questões pedidas abaixo são **opcionais**, não haverá problema em enviar a solução parcialmente feita. Porém, quanto mais completa a sua solução, mais pontos sua avaliação terá! 

### 🟡 Competências avaliadas
- Organização e comentários;
- Boas práticas de programação web;
- Conhecimento em orientação a objetos;
- Boas práticas de integridade e segurança de dados


### 🟡  Cenário/Problema
A empresa Nox Bitcoin executa, entre outras diversas atividades, a compra e venda da moeda que carrega em seu nome. 

Em determinado momento, se fez necessário utilizar a tecnologia em seu favor para o correto armazenamento de dados pertinentes e relevantes, possibilitando a geração de informações que apoiem o nível estratégico da empresa na tomada de decisões.

Você agora é o desenvolvedor e precisamos que você, seguindo as competências supracitadas, nos ajude a resolver alguns problemas ligados ao registro de nossas ordens de compra e venda através dos tópicos orientadores infracitados, considerando que o usuário possui um saldo inicial de **R$10.000,00** e para que sejam realizadas as suas negociações,  serão necessários:

**1.** Desenvolvimento de uma api através de HTTP Rest para captação, através de formulário a ser preenchido pelo usuário (nos campos pertinentes, não em todos), com as seguintes informações:

        1.1. CÓDIGO DA TRANSAÇÃO;
        1.2. E-MAIL DO USUÁRIO DA TRANSAÇÃO;
        1.3. VALOR DA TRANSAÇÃO EM REAIS (UTILIZAR 10 CASAS DECIMAIS);
        1.4. TIPO DA  ORDEM (COMPRA OU VENDA);
        1.5. DATA E HORA DA TRANSAÇÃO;
        1.6. STATUS DA TRANSAÇÃO (ABERTA, EXECUTADA OU REJEITADA)

**2.** Armazenamento das informações em uma lista ordenada contendo o objeto completo da transação (sugestão: dicionário);

**3.** Elaborar um relatório, em texto, sem necessidade de geração de arquivo .PDF ou correlato, exibido na própria página, com o valor total (R$), em 4 casas decimais com arredondamento para cima, de todas as transações realizadas em um período composto por data inicial e data final a serem informadas pelo usuário solicitante através de formulário;

**4.** Desenvolver uma ação específica para possibilitar a modificação do status, entre as possibilidades mencionadas no item 1.6, de uma ou várias transações através de comando único, não esquecendo que no caso de erro em apenas uma, todas devem ser desfeitas.


### 🟡  Observações
- **Não** será observado o design/layout escolhido para os formulários, tendo em vista que objetivo é a avaliação da capacidade técnica voltada para o  âmbito do back-end, entretanto: será observada a prudente escolha dos componentes para cada finalidade de captação dos dados via formulários;
- Fica facultada ao usuário a possibilidade de realizar diversas transações de compra e venda em paralelo. Isso posto, deve se considerar que caso alguma transação venha a dar errado, todas as outras transações devem respeitar a fila através de correta ordenação através do campo de data e hora citado no item 1.5;
- O usuário **não poderá** realizar transações que, somadas, superem o seu saldo mencionado no enunciado;
- O status padrão de uma transação, no momento de sua criação, é **aberta**;
- Toda transação, ao ter seu status modificado de **aberta** para **executada**, deve movimentar o saldo do usuário  negativamente;
- Toda transação, ao ter seu status modificado de **rejeitada** para **executada**, deve movimentar o saldo do usuário  negativamente;
- Toda transação, ao ter seu status modificado de **executada** para **rejeitada**, deve movimentar o saldo do usuário positivamente;
- Toda transação, ao ter seu status modificado de **aberta** para **rejeitada**, não deve movimentar o saldo;
- As transações abertas não movimentam o saldo do usuário, mas devem servir de base para o **total de transações** que ele poderá executar e criar, ou seja, a soma de todas as transações em aberto, não deverá ultrapassar o saldo total do usuário; 
- Será observado o **correto tratamento de erros e exceções**;
- O código backend deverá ser escrito em **C# ASP.NET**;
- O uso de outras linguagens como complemento para elaboração do frontend é facultativa;
- O uso de banco de dados é facultativo;

### 🟡  Dúvidas
Quaisquer dúvidas que você venha a ter, entre em contato através do email andreza@nox.trading.


