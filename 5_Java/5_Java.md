<p align="center">
  <img src="../img/java.svg" width="300">
</p>

## Java

Regra geral para printf

- #f = float (ponto flutuante)

- %d = inteiro

- %s = texto

- %n = quebrar linha


### This
É uma referência para o próprio objeto, ele diferencia atributos de variáveis locais.

### Construtores

Usos comuns:
- Iniciar valores dos atributos.
- Permitir ou obrigar que o objeto receba dados/dependências no momento de sua instaciação(injeção de dependência).
- Se um construtor customizado não for especificado, a classe disponibiliza o construtor padrão:
```java
Product p = new Product();
```

Exemplo:
```java
public class Product {
  public String name;
  public double price;
  public int quantity;

  public Product(String name, double price, int quantity){
    this.name = name;
    this.price = price
    this.quantity = quantity;
  }
}

Product product = new Product(name, price, quantity)
```
