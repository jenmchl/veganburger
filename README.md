# Como rodar esse site localmente

## Instale o framework Hugo

Instale Hugo de acordo com as [instruções do site](https://gohugo.io/getting-started/installing/). Execute `hugo version` para verificar se o framewrk foi instalado corretamente.

## Clone o repositório

Usando o terminal, vá para a pasta onde você deseja guardar o repositório deve ficar e execute:
```bash
git clone https://github.com/jenmchl/veganburger.git
cd veganburger
```

## Adicione o submódulo do tema

O site Vegan Burger usa um tema que está em outro repositório do GitHub. Para clonar essa pasta, execute:
```bash
cd themes
git clone https://github.com/digitalcraftsman/hugo-creative-theme
```

## Adicione uma API Key para o Google Maps

Se você quer renderizar o mapa do Google Maps localmente, precisa utilizar uma *API Key*. [Clique aqui](https://developers.google.com/maps/gmp-get-started) e saiba mais.

Com sua chave criada, crie um novo arquivo em `config/development/config.toml`. Você pode fazer isso executando:
``
mkdir -p config/development/
touch config/development/config.toml
```

Adicione o seguiinte conteúdo ao novo arquivo, supondo que sua chave seja `xyz`, por exemplo:
```toml
[params]
	 [params.location]
		maps_api_key = "xyz"

```

## Rode o servidor

O último passo é rodar `hugo server` no diretório `veganburger/`. Agora você pode ver o site no seu navegador acessando [http://localhost:1313/](http://localhost:1313/).
