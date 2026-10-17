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
