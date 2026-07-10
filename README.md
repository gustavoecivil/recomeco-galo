# Quando uma coleção vira parte de um recomeço

Página pessoal criada para contar a história por trás da venda de uma coleção especial do Galo.

O projeto não foi pensado como uma loja ou landing page tradicional. A proposta é apresentar uma narrativa pessoal sobre memória, reconstrução profissional e continuidade dos estudos, deixando as peças e os valores em segundo plano.

## Sobre o projeto

A página reúne:

- uma história pessoal sobre recomeço profissional;
- cinco camisas especiais do Galo, nunca usadas, com etiqueta e embalagem original;
- uma jaqueta Parka Topper rara e muito bem conservada;
- informações essenciais sobre tamanhos e valores;
- um contato discreto pelo WhatsApp;
- uma apresentação breve da Cultura Data Driven;
- um convite para colecionadores que desejem organizar suas coleções em formato de acervo digital.

## Estrutura do repositório

```text
.
├── index.html
├── netlify.toml
├── README.md
└── assets/
    ├── allblack_gallery.webp
    ├── favicon.svg
    ├── jaqueta_gallery.webp
    ├── manto1_gallery.webp
    ├── manto2_gallery.webp
    ├── manto4_gallery.webp
    ├── manto5_gallery.webp
    └── og-cover.jpg
```

## Tecnologias

- HTML5
- CSS3
- JavaScript mínimo
- Netlify para hospedagem e publicação contínua

Não há framework, banco de dados ou etapa de compilação. O site é totalmente estático.

## Executar localmente

Você pode abrir o arquivo `index.html` diretamente no navegador.

Para testar com um servidor local, use uma das opções abaixo.

### Python

```bash
python -m http.server 8000
```

Depois, abra:

```text
http://localhost:8000
```

### VS Code

Use a extensão **Live Server** e clique em **Open with Live Server** no arquivo `index.html`.

## Publicar no Netlify a partir do GitHub

1. Entre no Netlify.
2. Clique em **Add new project**.
3. Escolha **Import an existing project**.
4. Selecione **GitHub**.
5. Autorize o acesso ao GitHub, caso seja solicitado.
6. Escolha o repositório `gustavoecivil/recomeco-galo`.
7. Configure:
   - **Branch to deploy:** `main`
   - **Base directory:** deixe vazio
   - **Build command:** deixe vazio
   - **Publish directory:** `.`
8. Clique em **Deploy site**.

Depois da conexão, cada alteração enviada para a branch `main` será publicada automaticamente pelo Netlify.

## Atualizar o site depois da publicação

Faça as alterações nos arquivos, envie um novo commit para a branch `main` e aguarde o deploy automático.

Exemplo pelo terminal:

```bash
git add .
git commit -m "Atualiza conteúdo da página"
git push origin main
```

## Configuração do Netlify

O arquivo `netlify.toml` define a pasta publicada e alguns cabeçalhos básicos de segurança e cache.

Como o projeto é estático, não existe comando de build.

## Contato

**Gustavo**  
WhatsApp: **31 99198-8289**

Projeto profissional relacionado: **Cultura Data Driven**  
https://www.culturadatadriven.com

## Observação

As imagens e os textos desta página fazem parte de um projeto pessoal. Não reutilize o material comercialmente sem autorização.