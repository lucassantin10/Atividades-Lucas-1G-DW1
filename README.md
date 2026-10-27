# Atividades-Lucas-1G-DW1
Atividades do Lucas Santin 1G

1) O contêiner organiza os itens dentro dele. O item é cada elemento dentro do contêiner. Usamos `display: flex;` no contêiner.

2) O eixo principal é horizontal, da esquerda para a direita (`row`).

3) É o espaço livre que sobra no contêiner. Se todos os itens têm `flex-grow: 0`, ninguém recebe essa sobra.

4) O valor padrão é `0`, o que significa que o item não cresce para ocupar o espaço livre.

5) A mesa representa o contêiner; o prato representa cada item; a sobra representa o espaço livre; e o peso do `flex-grow` representa a proporção da sobra recebida por cada item.

6) style.css:

.marca {
    flex-grow: 1;
}

A declaração vai no elemento da marca.

7) Soma dos pesos: 2+3+1=6. Uma parte vale 600÷6=100 px. Item 1: 2×100=200 px; item 2: 3×100=300 px; item 3: 1×100=100 px.

8) Espaço ocupado: 3×100=300 px. Sobra: 600-300=300 px. Larguras finais: item 1 = 100 px; item 2 = 200 px; item 3 = 300 px.

9) O `flex-shrink` entra em ação quando falta espaço. Seu valor padrão é `1`.

10) Faltam 800-600=200 px. Cada item perde 100 px e fica com 300 px.

11) O primeiro item fica com 400 px e o segundo com 200 px. Sim, o conjunto cabe exatamente na faixa de 600 px.

12) Um logotipo pode ter `flex-shrink: 0;` para não diminuir de tamanho quando faltar espaço.
