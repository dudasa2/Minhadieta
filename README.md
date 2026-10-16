# Minha Dieta

App pessoal de acompanhamento da dieta — um único arquivo HTML, sem dependências externas, que funciona como um app simples no navegador (inclusive no iPhone, via "Adicionar à Tela de Início").

## O que tem dentro

- **Hoje**: suplementos do dia e as refeições prescritas pela nutricionista, com opções de troca (swaps) para cada refeição, e um botão para marcar cada uma como feita.
- **Preparo**: checklist de tarefas de preparo da semana (porcionar, fazer sanduíches, etc.). As marcações ficam salvas até você tocar em **Nova semana**, que desmarca tudo.
- **Despensa**: referência do que normalmente tem na geladeira/despensa, por categoria.
- **Mais**: regras rápidas (refrigerante, sucos, salada, ceia), rotina diária e um registro de peso.

Tudo o que é marcado fica salvo no `localStorage` do navegador, ou seja, no próprio aparelho:

- refeições e suplementos: separados por dia (à meia-noite o app começa um dia novo, mesmo se estiver aberto);
- tarefas de preparo: até tocar em **Nova semana**;
- peso: um registro por dia (as 10 datas mais recentes aparecem na tela).

Os dados não vão para nenhum servidor e não passam de um aparelho para outro. Se você apagar os dados do site no navegador, eles se perdem.

## Como usar localmente

Não precisa de servidor nem de instalação. Basta abrir o arquivo `index.html` em qualquer navegador moderno (Chrome, Safari, Firefox).

## Como publicar com GitHub Pages (link público gratuito)

1. Envie `index.html` e `README.md` **soltos na raiz** do repositório, na branch `main` (não envie um `.zip`: o GitHub Pages não abre arquivos compactados).
2. No repositório, vá em **Settings → Pages**.
3. Em "Source", escolha **Deploy from a branch**, depois a branch `main` e a pasta `/ (root)`.
4. Salve. Em alguns minutos o GitHub mostra o link público (algo como `https://seu-usuario.github.io/nome-do-repositorio/`).
5. Abra esse link no Safari do iPhone e, no menu de compartilhar, escolha **Adicionar à Tela de Início**. O app passa a abrir em tela cheia, como um aplicativo.

> **Atenção:** repositórios públicos e sites do GitHub Pages podem ser vistos por qualquer pessoa. Os dados que você marca no app (refeições, peso) ficam só no seu aparelho e não vão para o GitHub, mas tudo o que está escrito no `index.html` fica público.

## Estrutura

```
.
├── index.html   # o app completo (HTML + CSS + JS em um único arquivo)
└── README.md    # este arquivo
```
