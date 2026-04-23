# una-blazor-lista12.

# 🌱 EcoMonitor

## 👤 Identificação
- Nome: André Vitor de Andrade Santos  
- Curso: Ciência da computação 

---

## 🧠 Heurísticas de Nielsen aplicadas

### 1. Visibilidade do Status do Sistema
O componente EcoStatus exibe claramente o título da ação ecológica e seu peso, permitindo que o usuário visualize rapidamente o impacto de cada ação.

### 2. Consistência e Padrões
O mesmo componente é reutilizado para diferentes ações ecológicas (Reciclagem, Plantio, Descarte), mantendo um padrão visual consistente na interface.

▶️ Guia de Execução
Siga os passos abaixo para executar o projeto:

Abra o terminal na pasta do projeto

Execute o comando para restaurar as dependências:

dotnet restore
Compile o projeto:

dotnet build
Execute a aplicação:

dotnet run
Abra o navegador no endereço informado no terminal (geralmente https://localhost:5001/)

⚙️ Explicação Técnica
O componente foi desenvolvido utilizando o recurso [Parameter] do Blazor, que permite tornar componentes reutilizáveis.

🔹 Como funciona:
A propriedade marcada com [Parameter] permite que valores sejam passados do componente pai para o componente filho.
Isso possibilita reutilizar o mesmo componente em diferentes partes do sistema com conteúdos diferentes.
🔹 Exemplo:
[Parameter]
public string Titulo { get; set; }
🔹 Uso no componente:
<h3>@Titulo</h3>
🔹 Uso ao chamar o componente:
<MeuComponente Titulo="Meu Primeiro Componente" />
➡️ Dessa forma, o componente se torna dinâmico e reutilizável, pois o valor do título pode ser alterado conforme a necessidade.

✅ Conclusão
O uso de componentes reutilizáveis com parâmetros melhora a organização do código, reduz duplicação e facilita a manutenção do sistema.
