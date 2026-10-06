Desenvolvimento Web

Usabilidade, Dev. Web, Mobile e Jogos

Professor Daniel Henrique Matos de Paiva

## Lista de Exercícios

## Esta lista de exercício deve:

- \- Ser realizada em equipes de até 05 alunos.

- \- Ser entregue no prazo proposto.

- \- Ter os algoritmos pedidos escritos em linguagem .NET.

- \- Ter todos os algoritmos devidamente indentados.

## Exercícios:

Crie um novo projeto chamado: SiteDoisBlazor

Crie um novo repositório no github: site-dois-blazor

Lembre-se de ao criar seu repositório no GitHub, adicione o arquivo readme, o gitignore do Visual Studio e licença MIT.

Lista de Exercícios Práticos: Blazor Nível 2 (Interatividade + Navegação)

Lembrete importante: Todos os novos componentes interativos devem incluir a diretiva @rendermode InteractiveServer na segunda linha (logo abaixo do @page).

## Exercício 1: Conversor de Temperatura Simples

Objetivo: Praticar a leitura e manipulação de formulários básicos (@bind) e botões com interatividade.

## Instruções:

- 1. Crie o arquivo Conversor.razor com a rota @page "/conversor".

- 2. Adicione @rendermode InteractiveServer.

- 3. Na seção @code:

- o Declare duas variáveis double: celsius e fahrenheit.


Usabilidade, Dev. Web, Mobile e Jogos

## Professor Daniel Henrique Matos de Paiva

- o Crie um método Converter que aplique a fórmula: 𝐹 = (𝐶 × 9/5) + 32.

## 4. Na marcação HTML:

- o Crie um campo de texto <input type="number" @bind="celsius" />.

- o Crie um botão com @onclick="Converter" para realizar o cálculo.

- o Exiba o resultado: Temperatura em Fahrenheit: @fahrenheit °F.

## Exercício 2: Calculadora de Média do Aluno

Objetivo: Trabalhar com múltiplos inputs, validações condicionais simples e estados de aprovado/reprovado.

## Instruções:

- 1. Crie o arquivo Media.razor com a rota @page "/media".

- 2. Adicione @rendermode InteractiveServer.

- 3. Na seção @code:

- o Declare duas variáveis double: nota1 e nota2.

- o Declare uma variável double? chamada media (nula no início).

- o Crie um método CalcularMedia que tire a média aritmética das duas notas.

## 4. Na marcação HTML:

- o Crie dois inputs numéricos vinculados às notas usando @bind.

- o Crie um botão "Calcular Média" com o evento @onclick.

- o Se a media tiver valor (não for nula):

- Mostre o valor da média.

- Se a média for maior ou igual a 7.0, exiba a mensagem em verde: "Aprovado!".

- Caso contrário, exiba em vermelho: "Reprovado!".


Desenvolvimento Web

Usabilidade, Dev. Web, Mobile e Jogos

Professor Daniel Henrique Matos de Paiva

## Exercício 3: Sorteador de Números

Objetivo: Utilizar bibliotecas padrão do C# (System.Random) dentro de métodos de evento Blazor.

## Instruções:

- 1. Crie o arquivo Sorteio.razor com a rota @page "/sorteio".

- 2. Adicione @rendermode InteractiveServer.

- 3. Na seção @code:

- o Declare uma variável int? chamada numeroSorteado.

- o Crie um método SorteiaNumero que gere um número aleatório entre 1 e 100 usando a classe Random.

- 4. Na marcação HTML:

- o Crie um botão com o texto "Gerar Número Aleatório" que dispara o sorteio via @onclick.

- o Exiba o número sorteado na tela em um título <h2>.

- Exercício 4: Integrando as Páginas no Menu Lateral (NavMenu.razor)

Objetivo: Aprender a cadastrar novas rotas no menu de navegação principal da aplicação utilizando o componente <NavLink>.

## Instruções:

- 1. Abra o arquivo Layout/NavMenu.razor (ou Shared/NavMenu.razor dependendo do template).

- 2. Observe a estrutura existente dos links <div class="nav-item px- 3">...</div>.

- 3. Adicione três novos itens de menu para acessar as páginas criadas nesta lista:

- o Conversor (apontando para href="conversor")

- o Calculadora de Média (apontando para href="media")

- o Sorteador (apontando para href="sorteio")


Desenvolvimento Web

Usabilidade, Dev. Web, Mobile e Jogos

Professor Daniel Henrique Matos de Paiva

Exemplo de sintaxe do <NavLink>:

<div class="nav-item px-3">

<NavLink class="nav-link" href="conversor">

<span class="bi bi-calculator-fill-nav-menu" aria-hidden="true"></span>

Conversor

</NavLink>

</div>

Execute o projeto com dotnet watch ou F5 e confirme se é possível navegar por todas as páginas através da barra lateral sem precisar digitar a URL manualmente.

Ao concluir a atividade, suba seu projeto para o repositório no GitHub.
