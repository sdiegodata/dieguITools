### Tipos de Dados em Computação

Quando programamos, precisamos dizer ao computador que tipo de dado estamos lidando para que ele saiba como armazená-lo e manipulá-lo. Esses tipos de dados indicam duas coisas principais:

1. **O que o dado representa**: É um número inteiro, um número decimal, texto, etc.?
2. **Quanto espaço na memória esse dado ocupa**: Diferentes tipos de dados ocupam diferentes quantidades de espaço.

### Notação dos Tipos Numéricos

Em Rust e Polars (que usa Rust por baixo do capô), existem tipos de dados específicos para números inteiros e números de ponto flutuante. Vamos ver o que significa cada uma das notações:

#### Números Inteiros

- **`i32`**: 
  - **Significa**: Inteiro de 32 bits.
  - **O que isso quer dizer**: Um número inteiro que pode ser positivo, negativo ou zero. Usa 32 bits (ou 4 bytes) de memória. Pode representar valores de aproximadamente -2 bilhões a +2 bilhões.

- **`i64`**:
  - **Significa**: Inteiro de 64 bits.
  - **O que isso quer dizer**: Similar ao `i32`, mas usa 64 bits (ou 8 bytes), o que permite representar números muito maiores, de aproximadamente -9 quintilhões a +9 quintilhões.

#### Números de Ponto Flutuante

- **`f32`**:
  - **Significa**: Número de ponto flutuante de 32 bits.
  - **O que isso quer dizer**: Um número com casas decimais. Usa 32 bits de memória. Tem precisão limitada, o que significa que nem todos os números decimais podem ser representados com exatidão, mas é mais leve e rápido para cálculos que não precisam de muita precisão.

- **`f64`**:
  - **Significa**: Número de ponto flutuante de 64 bits.
  - **O que isso quer dizer**: Como o `f32`, mas usa 64 bits. Tem uma precisão muito maior, o que é importante quando você precisa de cálculos mais precisos com números decimais.

### Por Que Usamos Diferentes Tipos?

A escolha entre esses tipos depende das necessidades do seu programa:

- **Precisão**: Se você precisa representar números muito grandes ou cálculos muito precisos, você usa tipos com mais bits (`i64`, `f64`).
- **Eficiência**: Tipos com menos bits (`i32`, `f32`) são mais rápidos e usam menos memória, o que pode ser importante quando você tem muitos dados ou está em um dispositivo com recursos limitados.

### Resumo Visual

Para ajudar a visualizar, pense nos tipos de dados como recipientes de diferentes tamanhos:

- **`i32`** é como uma caixa de tamanho médio, suficiente para a maioria dos números inteiros do dia a dia.
- **`i64`** é uma caixa maior, para quando você precisa guardar números bem grandes.
- **`f32`** é como um copo para líquidos, mas que não consegue segurar todas as gotas de água exatamente no mesmo lugar.
- **`f64`** é um copo maior e mais preciso, capturando mais detalhes do líquido (número decimal) que você está tentando medir.
