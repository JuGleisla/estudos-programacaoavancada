# Programação Avançada 

## Memória e ponteiros:

> Variáveis e endereços

É uma posição de memória e que toda variável tem um endereço (bytes).

- int: usada para números inteiros.
- double: usada para números reais.

Exemplos:

- nome_var: se refere ao conteúdo da variável.<br> 
- &nome_var: se refere ao endereço da variável.<br>
- tipo_var nome_var: cria uma variável denominada "nome_var" e do tipo "tipo_var", sem definir um valor inicial específico para a variável.<br> 
- tipo_var nome_var(val): define (cria) uma variável denominada "nome_var" do tipo "tipo_var", com valor inicial "val". Equivalente a "tipo_var nome_var = val;"<br>
- const tipo_var nome_var (val): define (cria) uma variável com valor inicial val que não poderá ser modificado.
- auto nome_var (val): cria uma variável denominada nome_var do mesmo tipo e com valor inicial igual a val. Equivalente a auto nome_var = val;
- sizeof (nome_var) ou sizeof (tipo_var): retorna o número de bytes ocupados pela variável nome_var ou por uma variável do tipo_var. 
> Ponteiros e arrays

Variáveis do tipo ponteiro correspondem a informações do tipo endereço: 

- O endereço do ponteiro (&nome_var). As variáveis do tipo ponteiro, como toda cariável, também residem em um bloco de bytes da memória e tem endereço.
- O conteúdo do ponteiro (nome_var), que é o endereço armazenado na variável.

Sintaxe específica para variáveis do tipo ponteiro: 

- *nome_var: operação de desreferenciação (exclusiva de ponteiros). Refere-se ao conteúdo da área de memória para onde o conteúdo da variável aponta. 
- tipo_var* nome_var: define (cria) uma variável ponteiro denominada nome_var que aponta para uma variável (área de memória) do tipo tipo_var
- void* nome_var: define (cria) um ponteiro genérico (não pode ser desreferenciado, ou seja, não se pode usar *nome_var)<br>

Observação: Para evitar o risco de desreferenciar ponteiros selvagens (wild pointers), é recomendável que todos os ponteiros, ao serem criados sem que se possa definir seu valor correto, sejam inicializados com a constante "nullptr", que é um "endereço" que não aponta para nenhuma posição de memória válida e que encerrará o programa de forma ordenada caso seja desreferenciado: (int* pti (nullptr); // ou int* pti=nullptr;) 

- NÃO SE PODE SOMAR PONTEIROS COM PONTEIROS, MAS SIM PONTEIROS COM INTEIROS!!!<br>

Referências: 

- Uma referência é um nome alternativo para uma variável existente. Ela não possui um bloco próprio de bytes na memória, pois ela pe aoenas outeono nome par ao mesmo bloco de memória ocupado pela variável previamente existente. O endereço de uma referência é o mesmo endereço da variável original. 
- Sintaxe: (tipo_var& nome_var2(nome_var1): define (cria) uma variável denominada nome_var2 que faz referência (é um apelido) para a variável nome_nvar1, ambas do tipo tipo_var. Temos também, tipo_var& nome_var2 = nome_var1;)
- Elas precisam ser inicializadas!
> Alocação dinâmica de memória

## Funções
## Novos tipos de dados
## Entrada e saída de dados (arquivos)
## POO e Classes 
## Tratamento de erros 
## Templates 
## Introdução às estruturas de dados:
> Biblioteca STL
## Programação visual:
> Qt
## Herança entre classes 
## Polimorfismo e métodos virtuais
## Introdução à programação concorrente:
> Threads
## Introduçãp à programação distribuída:
> Sockets
