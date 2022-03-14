# <p> Síntese de estudos em Python <img  alt="Logo Python" src="https://media.giphy.com/media/LMt9638dO8dftAjtco/giphy.gif" width="60"> </p>

### 1. **O que é Python? Quais são os benefícios de usar Python?**
Python é uma linguagem de programação de alto nível, interpretada e de propósito geral. Sendo uma linguagem de uso geral, pode ser usada para construir quase qualquer tipo de aplicativo com as ferramentas/bibliotecas certas. Além disso, o python suporta objetos, módulos, threads, tratamento de exceções e gerenciamento automático de memória que ajudam na modelagem de problemas do mundo real e na criação de aplicativos para resolver esses problemas.

### Benefícios de usar Python:

Python é uma linguagem de programação de uso geral que possui uma sintaxe simples e fácil de aprender que enfatiza a legibilidade e, portanto, reduz o custo de manutenção do programa. Além disso, a linguagem é capaz de criar scripts, é totalmente de código aberto e suporta pacotes de terceiros, incentivando a modularidade e a reutilização de código.
Suas estruturas de dados de alto nível, combinadas com tipagem dinâmica e vinculação dinâmica, atraem uma enorme comunidade de desenvolvedores para desenvolvimento e implantação de aplicativos rápidos.


### 2. **O que é uma linguagem tipada dinamicamente?**
Antes de entendermos uma linguagem tipada dinamicamente, devemos aprender o que é digitação. Digitação refere-se à verificação de tipos em linguagens de programação. Em uma linguagem fortemente tipada , como Python, "1" + 2 resultará em um erro de tipo, pois essas linguagens não permitem "coerção de tipo" (conversão implícita de tipos de dados). Por outro lado, uma linguagem de tipagem fraca , como Javascript, simplesmente produzirá "12" como resultado.

A verificação de tipo pode ser feita em duas etapas -

- **Estático** - Tipos de dados são verificados antes da execução.
- **Dinâmico** - Os tipos de dados são verificados durante a execução.
Python é uma linguagem interpretada, executa cada instrução linha por linha e, portanto, a verificação de tipo é feita em tempo real, durante a execução. Portanto, Python é uma linguagem tipada dinamicamente.

### 3. **O que é uma linguagem interpretada?**
Uma linguagem interpretada executa suas instruções linha por linha. Linguagens como Python, Javascript, R, PHP e Ruby são os principais exemplos de linguagens interpretadas. Programas escritos em uma linguagem interpretada são executados diretamente do código-fonte, sem etapa de compilação intermediária.

### 4. **O que é PEP 8 e por que é importante?**
PEP significa **Proposta de Aprimoramento do Python**. Um PEP é um documento oficial de design que fornece informações para a comunidade Python ou descreve um novo recurso para Python ou seus processos. O PEP 8 é especialmente importante, pois documenta as diretrizes de estilo para o código Python. Aparentemente, contribuir para a comunidade de código aberto do Python exige que você siga essas diretrizes de estilo de forma sincera e rigorosa.

### 5. **O que é Escopo em Python?**
Cada objeto em Python funciona dentro de um escopo. Um escopo é um bloco de código onde um objeto em Python permanece relevante. Os namespaces identificam exclusivamente todos os objetos dentro de um programa. No entanto, esses namespaces também têm um escopo definido para eles, onde você pode usar seus objetos sem nenhum prefixo. Alguns exemplos de escopo criado durante a execução de código em Python são os seguintes:

Um escopo local refere-se aos objetos locais disponíveis na função atual.
Um escopo global refere-se aos objetos disponíveis em toda a execução do código desde o início.
Um escopo de nível de módulo refere-se aos objetos globais do módulo atual acessíveis no programa.
Um escopo mais externo refere-se a todos os nomes internos que podem ser chamados no programa. Os objetos neste escopo são pesquisados ​​por último para localizar o nome referenciado.
Observação: objetos de escopo local podem ser sincronizados com objetos de escopo global usando palavras-chave como global .

### 6. **O que são listas e tuplas? Qual é a principal diferença entre os dois?**
Listas e Tuplas são tipos de dados de sequência que podem armazenar uma coleção de objetos em Python. Os objetos armazenados em ambas as seqüências podem ter diferentes tipos de dados . As **listas** são representadas com **colchetes** ``['sara', 6, 0.19]`` , enquanto as **tuplas** são representadas com **parênteses** ``('ansh', 5, 0.97)`` .
Mas qual é a real diferença entre os dois? A principal diferença entre os dois é que, enquanto as **listas são mutáveis** , as **tuplas são objetos imutáveis**. Isso significa que as listas podem ser modificadas, anexadas ou divididas em movimento, mas as tuplas permanecem constantes e não podem ser modificadas de nenhuma maneira. Você pode executar o seguinte exemplo no Python IDLE para confirmar a diferença:

```
my_tuple = ('sara', 6, 5, 0.97)
my_list = ['sara', 6, 5, 0.97]
print(my_tuple[0])     # output => 'sara'
print(my_list[0])     # output => 'sara'
my_tuple[0] = 'ansh'    # modifying tuple => throws an error
my_list[0] = 'ansh'    # modifying list => list modified
print(my_tuple[0])     # output => 'sara'
print(my_list[0])     # output => 'ansh'
```

### 7. **Quais são os tipos de dados internos comuns em Python?**
Existem vários tipos de dados integrados em Python. Embora o Python não exija que os tipos de dados sejam definidos explicitamente durante as declarações de variáveis, erros de tipo provavelmente ocorrerão se o conhecimento dos tipos de dados e sua compatibilidade entre si forem negligenciados. Python fornece ``type()`` e ``isinstance()`` funções para verificar o tipo dessas variáveis. Esses tipos de dados podem ser agrupados nas seguintes categorias:

- **None Type:**
A palavra-chave ``None`` representa os valores nulos em Python. A operação de igualdade booleana pode ser executada usando esses objetos NoneType.

- **Numeric Types:**
Existem três tipos numéricos distintos: **números inteiros**, **ponto flutuante** e **números complexos**. Além disso, **booleanos** são um subtipo de inteiros.  
*int* - Armazena literais inteiros incluindo números hexadecimais, octais e binários como inteiros.  
*float* -	Armazena literais contendo valores decimais e/ou sinais de expoente como números de ponto flutuante.  
*complex* - Armazena números complexos na forma (A + Bj) e possui atributos: realeimag.  
*bool* - Armazena o valor booleano (True ou False).

 ***Nota:*** *A biblioteca padrão também inclui **frações** para armazenar números racionais e **decimal** para armazenar números de ponto flutuante com precisão definida pelo usuário.*

- **Tipos de sequência:**
De acordo com o Python Docs, existem três tipos básicos de sequência: **listas**, **tuplas** e **range**. Os tipos de sequência têm os operadores ``in`` e ``not in`` definidos para percorrer seus elementos. Esses operadores compartilham a mesma prioridade que as operações de comparação.  
*tupla* - Sequência imutável usada para armazenar coleção de itens.  
*lista* - Sequência mutável usada para armazenar coleção de itens.  
*range* - Representa uma sequência imutável de números gerados durante a execução.  
*str* -	Sequência imutável de pontos de código Unicode para armazenar dados textuais.  

***Nota:*** A biblioteca padrão também inclui tipos adicionais para processamento:
1. Dados binários como ``bytearray bytes``, ``memoryview``, e
2. Strings de texto  como ``str``.