# 🍕 Pizzaria

## 📌 Descrição

O sistema permite criar pizzas personalizadas combinando:

* **Tamanho**: Brotinho, Tradicional ou Grande
* **Borda**: Tradicional, Catupiry ou Sem borda
* **Sabores**: Até 3 opções

Utilizando o padrão **Bridge**, o projeto separa a abstração (Pizza) da sua implementação (Montador), permitindo criar diferentes combinações sem gerar excesso de classes.

---

**Nome:** Paulo Roberto Santos Elias
**RA:** 2171392511011

---

## ⚙️ Tecnologias utilizadas

* JavaScript (Node.js)

---

## 🚀 Como utilizar

1. Clone o repositório:

```bash id="gk4q9y"
git clone https://github.com/seu-usuario/pizzaria.git
```

2. Acesse a pasta do projeto:

```bash id="l3m8x2"
cd pizzaria
```

3. Execute o arquivo:

```bash id="y8p2dw"
node index.js
```

---

## 💻 Exemplo de uso

```javascript id="v2k1sa"
const montador = new MontadorPizza("Catupiry", [
  "Calabresa",
  "Frango",
  "Mussarela"
]);

const pizza = new PizzaGrande(montador);
console.log(pizza.criarPizza());
```

### 🧾 Saída esperada:

```id="6qj3bt"
Pizza Grande -> Borda: Catupiry | Sabores: Calabresa, Frango, Mussarela
```

---

## 🧠 Padrão de Projeto

Este projeto utiliza o padrão **Bridge**, que permite separar a abstração da implementação, facilitando a manutenção e expansão do sistema.

