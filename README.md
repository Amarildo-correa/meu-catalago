# Catálogo Digital — Use Isis

Catálogo digital para venda de produtos femininos via WhatsApp.

## Acesse o catálogo

[https://amarildo-correa.github.io/meu-catalago](https://amarildo-correa.github.io/meu-catalago)

---

## Estrutura de arquivos

```
catalogo/
├── index.html        ← página principal
├── produtos.json     ← 👈 EDITE AQUI para gerenciar produtos
├── css/style.css     ← estilos
└── js/catalogo.js    ← lógica (edite o número de WhatsApp aqui)
```

---

## Como editar os produtos

Abra o arquivo **`produtos.json`** e edite os campos:

```json
{
  "id": 1,
  "nome": "Nome do Produto",
  "categoria": "Vestidos",
  "preco": 89.90,
  "descricao": "Descrição curta do produto",
  "disponivel": true,
  "imagem": "https://link-da-foto.jpg"
}
```

| Ação | Como fazer |
|---|---|
| **Marcar esgotado** | Mude `"disponivel": true` para `false` |
| **Alterar preço** | Edite o valor em `"preco"` (use ponto: `89.90`) |
| **Trocar foto** | Substitua o link em `"imagem"` |

---

## Configurar WhatsApp

Abra **`js/catalogo.js`** e edite a primeira linha:

```js
const WHATSAPP = "5551999999999"; // 55 + DDD + número
```