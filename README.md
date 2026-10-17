# [Caio Ladislau](http://ladislau.me)

Site pessoal estático em HTML e CSS.

Instale as dependências com o npm, respeitando o `package-lock.json`:

```sh
npm ci
```

Para visualizar localmente, execute na raiz do projeto:

```sh
python3 -m http.server 8000
```

Abra <http://localhost:8000>. A publicação deve incluir `index.html`, `css/`,
`img/`, o CSS do Bootstrap e os arquivos de CSS e fontes do Font Awesome
nos caminhos usados em `node_modules/`. A página não utiliza JavaScript.

## Atualização em produção

Se o servidor publica diretamente uma cópia deste repositório, execute na
raiz do projeto, com a branch `master` selecionada e sem alterações locais:

```sh
git pull --ff-only origin master && npm ci --omit=dev --ignore-scripts
```

O comando baixa as alterações publicadas na `master` e reinstala as dependências
nas versões do `package-lock.json`. O site é estático e não exige build nem
reinicialização da aplicação.
