# Site de Prestação de Contas do Clube de Atletismo

Este é um site estático pronto para hospedagem. A página pública mostra receitas, despesas, saldo, lançamentos e comprovantes. O painel `/admin` permite que pessoas autorizadas atualizem os lançamentos pelo navegador.

## Como hospedar

1. Crie um repositório no GitHub e envie esta pasta para ele.
2. Crie um site na Netlify apontando para esse repositório.
3. Em **Site configuration > Identity**, ative o Netlify Identity.
4. Em **Services > Git Gateway**, ative o Git Gateway.
5. Convide as pessoas que poderão publicar em **Identity > Invite users**.
6. Depois de publicado, acesse `https://seu-site.netlify.app/admin/`.

## Como publicar

No painel `/admin`, abra **Prestação de contas > Lançamentos financeiros**. Adicione ou edite receitas e despesas, anexe comprovantes quando necessário e clique em publicar. O site público será atualizado após a publicação.

## Arquivos principais

- `index.html`: página pública.
- `styles.css`: visual do site.
- `app.js`: leitura dos dados e cálculos de resumo.
- `data/lancamentos.json`: lista de receitas e despesas.
- `admin/config.yml`: configuração do painel de publicação.
