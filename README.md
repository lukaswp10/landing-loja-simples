# landing-loja-simples

Página simples de landing para uma loja ? único arquivo HTML com CSS inline.

Arquivos:
- `index.html` ? página principal (HTML + CSS inline).

Como substituir as imagens
- `logo.png`: coloque uma imagem quadrada (recomendado 300×300px) no mesmo diretório onde está o HTML, com nome `logo.png`. Formato recomendado: PNG ou SVG. O HTML já referencia `logo.png` no topo.
- `photo.jpg`: substitua pela foto da fachada com nome `photo.jpg` (recomendado 1600×900px) no mesmo diretório. Formato recomendado: JPG ou WebP.

Dicas:
- Substitua apenas os arquivos `logo.png` e `photo.jpg` ? mantenha os nomes exatos para que a página mostre automaticamente as imagens.
- Se preferir, use `<img src="logo.svg">` mantendo o nome `logo.png` ou edite o `src` no HTML para apontar outro arquivo.

Como rodar localmente (rápido)
1. Abra um terminal na pasta do projeto:

```bash
cd ~/landing-loja-simples
```

2. Servir localmente com Python:

```bash
python3 -m http.server 8000
# então abra: http://localhost:8000/index.html
```

Deploy rápido (drag & drop no Netlify)
1. Compacte a pasta (opcional) ou abra `~/landing-loja-simples` no seu gerenciador de arquivos.  
2. Acesse o painel do Netlify e arraste o conteúdo da pasta para a área "Sites" ? "Drag & drop your site output folder here".  
3. O Netlify publicará sem necessidade de build (é um site estático).

Conectar ao Netlify usando GitHub (passos mínimos)
1. Crie um repositório no GitHub com nome desejado (ex.: `landing-loja-simples`).  
2. No seu computador:

```bash
cd ~/landing-loja-simples
git init -b main
git add index.html README.md
git commit -m "add landing page html + README"
git remote add origin git@github.com:SEU_USUARIO/landing-loja-simples.git
git push -u origin main
```

3. No Netlify: "New site" ? "Import from Git" ? escolha GitHub e selecione o repositório ? Deploy.

Upload via FTP (cPanel)
- Conectar via FTP/FTPS ao host do seu provedor (ex.: `ftp.seudominio.com`).
- Usuário e senha: informe seu usuário/senha do hosting no cliente FTP.
- Subir os arquivos para a pasta pública do site (geralmente `public_html` ou `www`).
- Exemplo de passos:
  1. Conectar: host = `seu_host_ftp`, user = `SEU_USUARIO`, password = `SUA_SENHA` (você insere manualmente).  
  2. Navegar até `public_html`.  
  3. Arrastar `index.html`, `logo.png` e `photo.jpg` para `public_html`.  
  4. Acessar `https://seudominio.com/index.html`.

Observações
- Não execute deploys automáticos; os comandos acima são para você rodar manualmente.  
- Commit sugerido: `add landing page html + README`.
