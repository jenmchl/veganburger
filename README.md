# Como rodar esse site localmente

## Clone o repositório

Usando o terminal, vá para a pasta onde o repositório deve ficar e execute `git clone https://github.com/jenmchl/veganburger.git`.

## Instale o framework Hugo

Instale Hugo de acordo com as [instruções do site](https://gohugo.io/getting-started/installing/). Execute `hugo version` para verificar se o framewrk foi instalado corretamente.

## Adicione o submódulo do tema

O site Vegan Burger usa um tema que está em outro repositório do GitHub. Para clonar o tema, dentro de `veganburger/themes`, execute `git clone https://github.com/digitalcraftsman/hugo-creative-theme`.

## Rode o servidor

O último passo é rodar `hugo server` no diretório `veganburger/`. Agora você pode ver o site no seu navegador acessando [http://localhost:1313/](http://localhost:1313/).
