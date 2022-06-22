---
layout: post
title:  "Caneca no Blender 3D"
date:   2019-03-10 01:00:00 -0300
image: blender-caneca.jpg

categories:  [Tutorial, Blender]
tags:        [CG, 3D Arte]
description: Tutorial simples e rápido para iniciantes de como fazer uma caneca no blender 3d.
---


Se você ainda não se sente íntimo com o blender 3d, esse tutorial vai ajudá-lo a melhor entender o processo de criação.

### Modelagem

Inicie o blender e delete o cubo que vem por padrão. Crie um cilindro com 12 lados(SHIFT+A), escalone no eixo Z para 1.2(S->Z) e rotaciona na vista top em 45°(R).

![Caneca Blender Tutorial 01](/images/tutoriais/blender/00/blender-tutorial-caneca-01.gif){:title="Caneca Blender Tutorial 01" alt=""}

Crie 4 edge loops(CTRL+R) e posicione como na imagem em seguida crie mais um edge loop no meio.
Delete a parte de baixo, e faça duas extrusões na saída da alça... Esse ponto pode parecer confuso, vamos usar a ferramenta Spin para gerar uma curva na extrusão.
Posicione o cursor logo abaixo da última extrusão da alça, clique na spin  e configure seus valores para 3 e 90°.

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

![Caneca Blender Tutorial 02](/images/tutoriais/blender/00/blender-tutorial-caneca-02.gif){:title="Caneca Blender Tutorial 02" alt=""}

Aplique o modificador Mirror para espelhar a parte de cima, marque a opção Clipping para soldar os vértices que se unem e extruda uma última vez a alça, dessa vez para baixo. Após unir delete a face desnecessária e aplique o modificador.

Agora vamos trabalhar a parte interna, faça uma extrusão e clique com o botão direito do mouse para cancelar o movimento, em seguida escalone para dentro com a tecla S. Com mais uma extrusão leve a face para baixo criando a cavidade interna.

![Caneca Blender Tutorial 03](/images/tutoriais/blender/00/blender-tutorial-caneca-03.gif){:title="Caneca Blender Tutorial 03" alt=""}

Com isso praticamente concluímos o modelo, aplique o modificador Subdivision Surface e configure para 3 subdivisões. Perceba que nossa malha ainda não possui uma estrutura muito sólida então quando suavizamos a malha ela fica com esse aspecto horrível.
Vamos adicionar mais loops afim de dar consistência a malha, desative o subdivision surface, não precisa deletar, só desativar.
Agora crie mais 4 loops na parte interna e um quinto loop bem próximo da borda, é este quem garante que a malha não distorça com o uso do modificador.

![Caneca Blender Tutorial 04](/images/tutoriais/blender/00/blender-tutorial-caneca-04.gif){:title="Caneca Blender Tutorial 04" alt=""}

Adicione mais 2 loops nas bordas externas também e de uma atenção a base da caneca. No meu caso eu criei vários loops mas você pode fazer algo mais profissional como colocar menos loop onde não é necessário e trabalhar com faces quadradas, removendo os triângulos.

![Caneca Blender Tutorial 05](/images/tutoriais/blender/00/blender-tutorial-caneca-05.gif){:title="Caneca Blender Tutorial 05" alt=""}

Crie também mais dois loops, um para cada saída da alça como na imagem, e ative o Subdivision surface novamente, basicamente sua caneca esta pronta.

![Caneca Blender Tutorial 06](/images/tutoriais/blender/00/blender-tutorial-caneca-06.gif){:title="Caneca Blender Tutorial 06" alt=""}

### Cena

Para compor a cena eu fiz apenas um plano que vai simular a superfície de uma mesa, você pode ser bem mais criativo que isso.
Crie um primeiro plano e com a tecla (S) escalone para 10. O segundo plano vai servir como emissor de luz da cena, posicione como na imagem.


![Caneca Blender Tutorial 07](/images/tutoriais/blender/00/blender-tutorial-caneca-07.gif){:title="Caneca Blender Tutorial 07" alt=""}

### Material

Primeiro renomeie o plano do solo para mesa, crie um material (Difuse) com o nome mesa e uma cor meio amarronzada.
Mesmo procedimento com a luz porém o material é (Emission) e o Strenght 8

![Caneca Blender Tutorial 08](/images/tutoriais/blender/00/blender-tutorial-caneca-08.gif){:title="Caneca Blender Tutorial 08" alt=""}

E por fim crie o material da caneca, use um (Mix Shader) que vai nos dar a opção de mesclar dois shaders diferente.
Para o primeiro vamos usar um (Difuse) e para o segundo (Glossy) No glossy reduza o roughness para 0 e no Factor o valor é 0.150.

Selecione a câmera e ative o Lock Camera To View para posicionar a câmera onde você quiser, não esqueça de desativar depois.
Mude a resolução do seu render e aumente os samples para ter uma imagem de qualidade.

![Caneca Blender Tutorial 09](/images/tutoriais/blender/00/blender-tutorial-caneca-09.gif){:title="Caneca Blender Tutorial 09" alt=""}

Com isso a gente conclui esse tutorial... Fácil não?



