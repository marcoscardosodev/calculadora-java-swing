# 🧮 Super Calculadora Java Swing

Projeto de uma calculadora com interface gráfica, desenvolvida em **Java** com **Swing**, que vai além das quatro operações básicas. Ela realiza cálculos úteis em contextos matemáticos diversos, como:

- **Valor Absoluto**
- **Raiz Quadrada**
- **Potência**
- **Parte Inteira**
- **Inverso do número**

Ideal para quem está aprendendo a trabalhar com interfaces gráficas em Java ou deseja estudar manipulação de números e `Math` em um projeto prático.

---

## 🖼️ Interface Gráfica

A interface foi construída utilizando o **editor visual do NetBeans**, o que facilita o posicionamento de botões, rótulos e caixas de entrada.

A tela principal contém:

- Campo para inserir o número
- Botão "Calcular"
- Painel que exibe os resultados formatados com ícones

---

## ⚙️ Como funciona o código

A lógica do programa está concentrada na ação do botão "Calcular". Quando clicado:

1. O valor digitado é capturado como `int`:
   ```java
   int num = Integer.parseInt(txtNum.getValue().toString());
Os seguintes cálculos são feitos com a classe Math:

java
Copiar
Editar
int resto = num % 2;
double cubo = Math.pow(num, 3);
double raizQ = Math.sqrt(num);
double raizC = Math.cbrt(num);
int abs = Math.abs(num);
Os resultados são exibidos nos JLabels correspondentes:

java
Copiar
Editar
lblResto.setText(Integer.toString(resto));
lblCubo.setText(String.format("%.2f", cubo));
...
O painel de resultados (panCalc) é exibido com:

java
Copiar
Editar
panCalc.setVisible(true);
🛠️ Tecnologias e ferramentas
Java JDK 8+

Swing (javax.swing)

NetBeans IDE (Editor visual)

🚀 Como executar o projeto
Clone o repositório:

bash
Copiar
Editar
git clone https://github.com/marcoscardosodev/calculadora-java-swing.git
Abra o projeto no NetBeans.

Execute o arquivo TelaCalculadora.java como aplicação.

🧠 O que você aprende com esse projeto
Manipulação de interfaces gráficas com Swing

Integração entre elementos visuais e lógica de programação

Uso da classe Math para cálculos matemáticos

Boas práticas com tratamento de tipos e exibição de resultados

👨‍💻 Autor
Feito com dedicação por Marcos Cardoso
Se te ajudou, ⭐ dá uma estrela no repositório!
