
<p align="center">
  <img src="Bentodog.jpg" width="210" alt="Bentodog">
</p>

#  Perceptron Simples em Java

Este projeto é uma implementação bem direta de um Perceptron de camada única (Single Layer Perceptron) em Java puro, sem bibliotecas externas, só o básico mesmo.  
A ideia aqui é mostrar como funciona o mecanismo de aprendizado do modelo, passo a passo, do jeito mais simples possível.

---

##  O que é um Perceptron?

É a unidade básica de uma rede neural.  
Ele pega valores de entrada, multiplica por pesos, soma tudo, aplica uma função de ativação e diz se o resultado é 1 ou 0.

Pensa como um "funcionário da pizzaria":
- Ele recebe os pedidos (entradas),
- Consulta a ficha dele com as regras (pesos),
- Decide se entrega pizza ou não (saída).

---

##  Objetivo do projeto

O foco é didático:

- Mostrar como o perceptron ajusta os pesos ao longo do treino  
- Implementar o algoritmo clássico  
- Exemplificar usando o problema lógico OR  
- Ser fácil de ler, entender e adaptar  

---

##  Como funciona o aprendizado?

O perceptron treina usando a regra do erro:

novo_peso = peso_atual + taxaAprendizado * erro * entrada

Onde:
- erro = saída esperada – previsão  
- Se errar, ajusta os pesos  
- Se acertar, nada muda  
- O treinamento para quando não houver mais erros

---

##  Estrutura do código

- Perceptron.java  
  Contém tudo:
  - inicialização dos pesos  
  - função de ativação  
  - previsão  
  - treinamento  
  - teste final  
  - exemplos usando OR  

---

##  Como rodar

Compile:

javac Perceptron.java

Execute:

java Perceptron

---

##  Exemplo: Tabela OR

Entradas usadas no teste:

X1 | X2 | Saída  
0  | 0  | 0  
0  | 1  | 1  
1  | 0  | 1  
1  | 1  | 1  

---

##  Resultado esperado

O programa mostra:
- pesos iniciais  
- erros por época  
- pesos finais  
- previsão para todos os valores da tabela OR  

---

##  Observações

- Funciona apenas para problemas linearmente separáveis (como AND e OR).  
- Não resolve problemas como XOR — para isso precisa de mais camadas (MLPs).  
- Ideal para fins didáticos e entendimentos iniciais de redes neurais.

---

