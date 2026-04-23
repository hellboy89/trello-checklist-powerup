# Checklist Progress Badge — Trello Power-Up

Power-Up para o Trello que exibe **badges de progresso de checklists** diretamente nos cartões do quadro, sem precisar abrir cada cartão para saber o status.

![Exemplo de funcionamento](images/exemplo_funcionamento.png)

---

## Como funciona

O Power-Up lê os dados de checklist de cada cartão e exibe um badge colorido indicando o estado de conclusão:

| Badge | Cor | Condição |
|---|---|---|
| `Tudo feito!` | 🟢 Verde | Todos os itens marcados |
| `X pendente(s)` | 🟡 Amarelo | ≥ 50% concluído, ainda há pendências |
| `X pendente(s)` | 🟠 Laranja | < 50% concluído |
| `⚠ NADA MARCADO!` | 🔴 Vermelho | Nenhum item marcado |

> Cartões sem checklist não exibem badge.

---

## Badges disponíveis

### No quadro (card-badges)
Exibe um único badge resumido por cartão, mostrando a quantidade de itens pendentes e a porcentagem geral de conclusão.

### Dentro do cartão (card-detail-badges)
Ao abrir um cartão, cada checklist recebe seu próprio badge individual com nome, progresso e cor correspondente ao estado.

---

## Instalação

1. Acesse o [Trello Power-Up Admin](https://trello.com/power-ups/admin) e crie um novo Power-Up.
2. Preencha a **Connector URL** com a URL onde o `index.html` está hospedado (ex: GitHub Pages).
3. Ative as capabilities: `card-badges` e `card-detail-badges`.
4. No seu quadro do Trello, vá em **Power-Ups** e ative o **Checklist Progress Badge**.

---

## Hospedagem com GitHub Pages

1. Faça o fork ou clone deste repositório.
2. Ative o **GitHub Pages** nas configurações do repositório (branch `main`, pasta raiz).
3. Use a URL gerada (ex: `https://seu-usuario.github.io/trello-checklist-powerup/`) como Connector URL no admin do Trello.

---

## Estrutura do projeto

```
trello-checklist-powerup/
├── index.html       # Lógica principal do Power-Up
├── icon.svg         # Ícone do Power-Up
├── images/
│   └── exemplo_funcionamento.png
└── README.md
```

---

## Licença

MIT
