# Nomes Significativos

- Por que existe
- O que faz
- Como é utilizada
- Não precisa de comentários adicionais

Qual o significado de d?

```c
int d; // elapsed time in days
```

Nomes mais significativos:

```c
int elapsedTimeInDays;

int daysSinceCreation;

int daysSinceModification;

int fileAgeInDays;
```

## Nomes pronunciáveis
```java
Date genymdhms;
```

```java
Date generationTimestamp;
```

## Nomes Pesquisáveis
Letras ou vogais são difíceis de se pesquisar
```java
String n
```

## Evitar ambiguidades e palavras vazias: Info, Data, variable, object
```c
getClient();
getClientInfo();
getClientObject();
```
Onde obtenho o nome completo do cliente?

## Evitar nomes com tipos

```java
String clientNameString
```

### Evitar mapas mentais

```java
String n = customer.getName()
[...]
display(n) // n era o que mesmo?
```

## Classes devem usar Nomes (não verbos)

_Customer, WikiPage,Account, AddressParser_.

Evitar palavras como _Manager, Processor, Data, Info_ 

## Funções devem usar verbos

_postPayment, deletePage, save_

- Accessors, mutators e predicates devem ser nomeados de acordo com o valor + _set,get_, ou _is_.

```java
String name = employee.getName();
customer.setName("mike");
if (paycheck.isPosted())
```

- When constructores are overloaded, use static factory methods with names that describe their arguments:

```java
Complex pivotPoint = Complex.fromRealNumber(23.0);
// Complex pivotPoint = new Complex(23.0);
```

## Não faça piadas

Não escreva
```java
holyHandGrenade
```
quando você quer dizer:
```java
deleteItems
```
```java
kill() // whack()
abort() // eatMyShorts()
```