---
name: anti-alucinacao-recuperacao-extrajudicial
description: "Confere existência e rastreabilidade de fatos, citações, eventos e cálculos antes e depois das entregas de RE; bloqueia afirmações sem suporte."
---

# Guard de existência e rastreabilidade

Receber rascunho real/matriz, documentos, fontes e memória de cálculo. Sem rascunho, revisar apenas pendências, sem fabricar peça para simular revisão. Guidance only: controle por instrução, não hook. Este guard confere suporte; subsunção pertence ao validador.

1. Numerar afirmações; separar fato documentado, relato atribuído, norma literal, paráfrase, inferência identificada e proposta. Relato não prova pagamento, assinatura, poderes, protocolo, publicação, decisão ou adesão.
2. Fatos: arquivo, página/trecho, emissor/data, crédito/parte e alcance. Conferir efetivamente documento antes de afirmar evento externo. Dados faltantes permanecem desconhecidos.
3. Normas: localizar dispositivo e texto em `context/`; conservar negadores, incisos, ressalvas, tachados e números. Pode normalizar espaços/NFC só para comparação, sem alterar o arquivo. Não transformar cabeçalho editorial em artigo; não preencher remissão externa nem norma ética/LGPD por memória.
4. Precedentes: inteiro teor oficial capturado, identificação/situação/alcance; URL, notícia e ementa isolada não certificam tese. Ausência recebe 🟡 e impede citação dependente; nenhum processo/súmula inventado.
5. Cálculos: prova de cada valor, moeda, vencimento, data, taxa, unidade e fórmula. Deduplicar créditos/adesões por identificação documentada; não fabricar denominador, cotação ou poder de novar/transigir. Conferir aritmética exata em centavos, sem contagem por cabeça ou arredondamento que transforme metade em mais da metade.
6. Confrontar versões e redações tachadas: não usar 3/5 superado no 163 caput nem 83 IV/V como classes vigentes. Preservar “art. 43 deste artigo” como remissão anômala, sem editar corpus. Distinguir data do pedido, assinatura, edital e decisão.
7. Retirar afirmação sem suporte ou bloquear etapa dependente, sem substituir por outra suposição e sem esconder impedimento no rodapé.

Âncoras prioritárias: `context/lei-11101-recuperacao-extrajudicial.md` 161–167; `context/lei-11101-disposicoes-comuns.md` 20-A–20-D/43; demais fontes indicadas pelo rascunho, com índice/manifesto. CPC 305 e Lei 13.140 16–17 existem no corpus, mas 306–310 não são supridos. Hash do corpo identifica integridade local se conferido contra manifesto; hash HTML não é o hash do Markdown nem garantia de vigência atual.

Saída: **ID → afirmação/tipo → arquivo/trecho → suporte → correção/bloqueio**, lista de retiradas/provas faltantes e versão efetivamente corrigida. Quando em cadeia, retornar ao chamador; chamada direta de revisão passa ao `validador-recuperacao-extrajudicial` e `suprema-corte-recuperacao-extrajudicial`, sem recursão. Não simular correção material que não foi realizada.

## Fontes, sigilo e estado de entrega

Usar exclusivamente texto literal de `context/`, documentos do caso e relatos atribuídos. Índice, URL, memória e resumo não suprem artigo ausente. Não consultar Jusbrasil/Escavador nem completar o corpus pela internet nesta execução. Registrar arquivo, dispositivo, linhas/trecho, versão, data de captura e alcance. ✅ significa texto conferido no recorte; 🟡 significa fonte, prova, atualização ou interpretação pendente; 🔴 significa contradição ou hipótese bloqueada. Captura não certifica atualização posterior nem fato do caso. Buscas podem comparar Unicode em NFC apenas em memória: preservar os originais verbatim, tachados e remissões; cabeçalho editorial não é norma. Hash do HTML identifica snapshot, não prova texto atual.

Dados ficam em workspace privado, separados por cliente e matéria, fora do source e de repositórios compartilhados. Não enviar documentos a conectores/serviços sem autorização específica; não inventar integração disponível. Norma ética/LGPD não capturada recebe 🟡 sem número de artigo inventado. Não representar lados opostos no mesmo caso. Minuta é proposta: envio, assinatura, negociação, protocolo e decisões exigem atuação humana autorizada. Suporte: suporte@iapx.pro.

Entregar cliente/lado, empresa/atividade, objetivo/modalidade, data de corte, créditos/grupos, valores e origem, garantias, adesões/poderes, cronologia comprovada e matriz **requisito → fonte → fato → prova/trecho → resultado → pendência/responsável**. Fechar com `PREPARAÇÃO CONDICIONADA À REVISÃO HUMANA`, `PENDENTE DE PROVA`, `BLOQUEADO` ou `FORA DO RECORTE`, indicando próxima providência e limite da automação. Não afirmar homologação, suspensão, vinculação ou assinatura válida sem prova e fundamento.
