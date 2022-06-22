---
layout: post
title:  "Monólito Blender 2.8"
date:   2019-04-19 01:00:00 -0300
image: monolito.jpg
categories:  [Tutorial, Blender2.8]
tags:        [2d arte, CG, 3D Arte]
description: Esta começando no blender 2.8? Esse é um tutorial simples e rápido que mostra um pouco do poder da ferramenta.
---

Tutorial extremamente simples de como fazer um Monólito e renderizar usando o Eevee no blender 2.8.

Eu gerei uma imagem de grade com o JSplacement e a partir dela eu também gerei o color map e o normal map, essas foram minhas configurações, mais sinta se livre para explorar a sua própria criatividade.

![Monolito Blender Tutorial 01](/images/tutoriais/blender/01/blender-tutorial-monolito-01.jpg){:title="Monolito Blender Tutorial 01" alt=""}

No gimp eu adicionei uma textura de metal para deixar o monolito mais real.
A textura que eu usei você pode [baixar aqui ](https://cc0textures.com/view.php?tex=Metal19){:target="_blank"}, e eu recomendo demais o site [CC0Textures](http://cc0textures.com/) que contém texturas em 8k  com altíssima qualidade e de graça.

Eu apenas coloquei o mapa de cores acima da textura de metal e mudei a operação para Screen.

<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
     style="display:block; text-align:center;"
     data-ad-layout="in-article"
     data-ad-format="fluid"
     data-ad-client="ca-pub-6962200783353455"
     data-ad-slot="2866622444"></ins>
<script>
     (adsbygoogle = window.adsbygoogle || []).push({});
</script>

![Monolito Blender Tutorial 02](/images/tutoriais/blender/01/blender-tutorial-monolito-02.jpg){:title="Monolito Blender Tutorial 02" alt=""}

Vamos usar o box padrão do blender e fazer algumas modificações para ter a forma super complexa do monolito.
Essas são  as proporções que eu defini:

![Monolito Blender Tutorial 03](/images/tutoriais/blender/01/blender-tutorial-monolito-03.jpg){:title="Monolito Blender Tutorial 03" alt=""}

Aplique a rotação e escala, use o atalho CTRL+A. Mapeie o objeto com a tecla U e a opção Smart UV Projection. E organize a malha para que fique da melhor maneira possível

![Monolito Blender Tutorial 04](/images/tutoriais/blender/01/blender-tutorial-monolito-04.jpg){:title="Monolito Blender Tutorial 04" alt=""}

![Monolito Blender Tutorial 05](/images/tutoriais/blender/01/blender-tutorial-monolito-05.jpg){:title="Monolito Blender Tutorial 05" alt=""}

Agora precisamos de mais vértices para trabalhar com o displacement map, quanto mais vértices, maior o nível de realismo e mais efetivo o displacement porém o render time também será maior.
Manter a malha com quadrados uniformes é o segredo do sucesso, use CTRL+R para adicionar novos edge loops e deixar sua malha como a seguinte:

![Monolito Blender Tutorial 06](/images/tutoriais/blender/01/blender-tutorial-monolito-06.jpg){:title="Monolito Blender Tutorial 06" alt=""}

E em seguida subdivida todo o bloco por 10 vezes:

![Monolito Blender Tutorial 07](/images/tutoriais/blender/01/blender-tutorial-monolito-07.jpg){:title="Monolito Blender Tutorial 07" alt=""}

Agora adicione o modificador Displace e crie uma textura dentro do modificador:

![Monolito Blender Tutorial 08](/images/tutoriais/blender/01/blender-tutorial-monolito-08.jpg){:title="Monolito Blender Tutorial 08" alt=""}

Na aba Texture clique em Open e abra o height map criado no JSplacement e de volta ao modificador, mude as coordenadas da textura para UV e a força para -0.050.

![Monolito Blender Tutorial 09](/images/tutoriais/blender/01/blender-tutorial-monolito-09.jpg){:title="Monolito Blender Tutorial 09" alt=""}

Com isso você já tem o monólito praticamente pronto, se preferir você pode mudar a posição do UV Map, rotacionar e escalonar etc e ver o melhor resultado para você.

Esse foi o material que eu criei para o meu monolito:

![Monolito Blender Tutorial 10](/images/tutoriais/blender/01/blender-tutorial-monolito-10.jpg){:title="Monolito Blender Tutorial 10" alt=""}

Eu usei a mesma textura do displace como fator para definir as áreas que emitem luz, e ativei o Bloom na aba render.

![Monolito Blender Tutorial 11](/images/tutoriais/blender/01/blender-tutorial-monolito-11.jpg){:title="Monolito Blender Tutorial 11" alt=""}




