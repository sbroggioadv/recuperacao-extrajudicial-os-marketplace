---
name: negociacao-do-credor-na-re
description: "Prepara contraproposta e reservas do credor a partir do parecer de análise do plano e provas do crédito, sem assumir adesão ou recebimento."
---

# Negociação do credor na RE

## Entradas e fontes

Confirmar advogado do credor, crédito e garantias, poderes, objetivos, plano/modalidade, cronologia e parecer de `analise-do-plano-pelo-credor`. Ler `context/lei-11101-recuperacao-extrajudicial.md:17–57,83–87` (161–163, 165); `context/lei-11101-disposicoes-comuns.md:227–249` (20-A–20-D).

## Execução

1. Contrato de passagem M4: `analise-do-plano-pelo-credor` entrega o parecer de inclusão, tratamento, garantias e risco; esta skill o consome para formar contraproposta. Se faltar parecer, solicitá-lo/chamar a skill antes da contraproposta conclusiva. Não refazer a análise completa nem presumir parecer favorável.
2. Conferir objetivo do cliente e limites do mandato. Usar parecer e prova de crédito para definir reservas, condições mínimas e cláusulas a negociar. Não produzir também estratégia do devedor no mesmo caso nem revelar dados de outro cliente.
3. Separar adesão voluntária em 162 do alcance possível de 163 após homologação. Não afirmar que ausência de assinatura exclui necessariamente o credor da extensão. Crédito excluído/não incluído exige preservar regras do 161 §1º e 163 §2º; dívida discutida não recebe classificação por acordo.
4. Preparar contraproposta de prazo/valor/forma com base documental. Garantia real na alienação: aprovação específica para supressão/substituição (163 §4º); variação cambial: aprovação expressa para afastamento (§5º). Não presumir renúncia ou poderes para novar/transigir; encaminhar instrumento e poderes a `adesoes-e-poderes-na-re`.
5. Alertar sobre desistência após distribuição: depende de anuência expressa dos demais signatários (161 §5º). Explicar efeitos anteriores à homologação restritos a valor/forma de pagamento de signatários e restauração se rejeitado, com dedução dos pagos (165 §§1º–2º). Nenhuma oferta autoriza assinatura pelo agente.
6. Se acordo antecedente, chamar `mediacao-e-conciliacao-antecedentes` e preservar dedução do 20-B §3º e reconstituição de direitos/garantias do 20-C parágrafo único. Não garantir suspensão, quitação definitiva ou recebimento; cenários financeiros usam apenas dados e premissas declarados.
7. Se o objetivo passar a oposição judicial, encaminhar parecer/provas a `impugnacao-do-credor-na-re`, sem copiar rito da RJ nem afirmar prazo sem edital documentado. Não ameaçar falência como efeito automático da recusa da oferta.

## Saída

Contraproposta não vinculante, reservas e quadro: cláusula original/proposta, objetivo do credor, fundamento, prova, risco de adesão/não adesão, anuência/poderes pendentes e decisão humana necessária. Não formalizar adesão, renúncia, acordo ou contato externo.

## Controles e entrega

Em toda chamada, inclusive direta, aplicar `triagem-recuperacao-extrajudicial`: fixar cliente/lado, atividade, etapa, modalidade (162/163), data de corte e objetivo. Lado indefinido limita a coleta; representação dos lados opostos no mesmo caso bloqueia produção. Administrador judicial está fora do recorte. Guardar dados somente em workspace privado por cliente/matéria, nunca no source; nenhum envio externo sem autorização específica.

Ler os anexos literais indicados em `context/`, com `INDICE.md` e `manifesto-captura.json`; registrar dispositivo, linhas, trecho, versão/captura e documento do caso. Captura de 01/10/2026 não prova vigência posterior. Buscas podem normalizar Unicode para NFC em memória, preservando os originais verbatim. Artigo, remissão ou prova ausente = 🟡; contradição ou hipótese vedada = 🔴. Não usar memória ou fonte externa para preencher norma ausente.

Ao encerrar, chamar nesta ordem `anti-alucinacao-recuperacao-extrajudicial`, `validador-recuperacao-extrajudicial` e `suprema-corte-recuperacao-extrajudicial` (R1→R4). Registrar achados e correções: R1 fatos/provas/lado; R2 fundamentos e tensões; R3 tese, objeções e requisitos; R4 completude, sigilo e fronteiras. Falta de controle impede entrega conclusiva; não dizer que uma revisão foi executada sem registro. São instruções ao agente (guidance only), sem enforcement automático comprovado.

Entregar quadro **requisito → fonte → fato → prova/arquivo/trecho → resultado → pendência**, identificando cliente/lado, atividade, operação/modalidade, data de corte, créditos/grupos, valores/origem, garantias, adesões/poderes, cronologia comprovada, fontes e responsável por cada falta. Emitir `PREPARAÇÃO CONDICIONADA À REVISÃO HUMANA`, `PENDENTE DE PROVA`, `BLOQUEADO` ou `FORA DO RECORTE`, com motivo, etapa afetada e próxima providência. Minuta não é protocolo, assinatura, comunicação ou negociação pelo cliente; não afirmar homologação, suspensão ou vinculação sem ato e fundamento comprovados. Suporte: suporte@iapx.pro.
