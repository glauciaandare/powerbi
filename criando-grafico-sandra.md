🧹ETAPA 1 — Filtrar linhas nulas

1. No Power Query, selecione a coluna Mês.
2. Clique na setinha de filtro (ao lado do nome da coluna).
3. Desmarque (null) e, se quiser, também desmarque os valores duplicados que aparecem indevidos.
4. Clique em OK.

💡 Isso já remove as linhas onde Mês está nulo — e consequentemente elimina as linhas 8 e 15 da sua imagem.
______________________________________________________________________


⚙️ ETAPA 2 — Remover linhas com erro (aquelas que aparecem como “Error”)

1. Vá em Página Inicial → Remover Linhas → Remover Erros.
🔸 Isso exclui automaticamente as linhas com erros em qualquer coluna.

______________________________________________________________________

🧽 ETAPA 3 — Remover duplicadas (porque aparecem repetições como Apr, May, etc.)

1. Ainda no Power Query, com a tabela selecionada:
Vá em Página Inicial → Remover Linhas → Remover Duplicadas.
2. Ele vai manter apenas a primeira ocorrência de cada mês.

______________________________________________________________________

🔢 ETAPA 4 — Verifique o tipo das colunas

Depois de limpar, certifique-se de que as colunas numéricas estão corretamente definidas:

1. Abertos → número inteiro (Int64)
2. Fechados → número inteiro (Int64)
3. Backlog Mensal → número inteiro (Int64)
4. Backlog Acumulado → número inteiro (Int64)

Se houver erros depois disso, é porque o Power Query tentou converter texto (como “Error”) em número.
Como já removemos as linhas com erro, agora tudo deve converter normalmente.

______________________________________________________________________

✅ ETAPA FINAL

Depois que fizer isso:
1. Clique em Fechar e Aplicar no canto superior esquerdo.
2. O Power BI atualizará e manterá apenas as linhas válidas e únicas.

