# Funções

- Dificilmente devem ter 20 linhas
- 1 ou 2 níveis de identação
- 1 level de abstração
- Single Responsibility/ Doing one thing
- Devs devem conseguir entender sem olhar a assinatura da função


## Argumentos
- No máximo 2 argumentos. Idealmente zero.
- Argumentos dificultam testes: Como cobrir tudo?
- Evitar argumentos para saídas

## 1 Argumento
- Responder perguntas:
```java
boolean fileExists("MyFile");
```
- Transformar algo:
```java
InputStream fileOpen("MyFile");
```

## 2 Argumentos
- Qual a ordem?
```java
assertEquals(expected, actual)
```

```java
// writeField(outputStream, name)
outputStream.writeField(name)
```

- Ordem natural
```java
Point p = new Point(0,0)
```

## 3 Argumentos
```java
assertEquals(message, expected, actual)
```

## Argumentos Objetos

Quando se precisa de mais de dois ou três argumentos, é provável que esses argumentos deveriam **estar em uma classe própria**

```java
// Circle makeCircle(double x, double y, double radius)
Circle makeCircle(Point center, double radius)
```