---
name: cabimento-e-requisitos-da-re
description: "Avalia requisitos e impedimentos da recuperação extrajudicial, inclusive cabimento do produtor rural, para advogado do devedor ou do credor."
---

# Cabimento e requisitos da RE

## Entradas e fontes

Receber identificação empresarial pseudonimizada, atividade/PF ou PJ, registros e início da atividade regular, histórico de falência, RJ/RE, datas de concessão/homologação, trânsito em julgado e situação de administradores/controladores. Relato é entrada identificada, não prova de inexistência de impedimento.

Ler `context/lei-11101-disposicoes-comuns.md:15–25` (arts. 1º–3º); `context/lei-11101-recuperacao-judicial.md:17–35` (48 e §§1º–5º); `context/lei-11101-recuperacao-extrajudicial.md:15–23` (161 e §§1º–4º).

## Execução

1. Conferir empresário/sociedade empresária pelo art. 1º e exclusões do art. 2º, incluindo empresa pública, sociedade de economia mista e entidades do inciso II. Não enquadrar pela existência isolada de CNPJ. Competência pelo principal estabelecimento ou filial de empresa estrangeira (art. 3º), com prova, sem presumir foro da sede formal.
2. Pela remissão de 161 ao 48, testar cumulativamente: atividade regular há mais de dois anos; não falido ou responsabilidades extintas por sentença transitada; ausência de concessão de RJ há menos de cinco anos, inclusive plano especial (II/III); ausência de condenação por crime da Lei do devedor, administrador ou controlador (IV). Registrar prova por requisito, sem fabricar certidão negativa ou tratar silêncio como inexistência.
3. Acrescentar 161 §3º: RJ pendente impede requerer homologação; RJ ou outro plano de RE homologado há menos de dois anos também impede. O intervalo de cinco anos do 48 II/III cumula com o de dois anos do 161 §3º; RJ concedida há três anos não passa pelo simples decurso de dois. Não confundir negociação preliminar com aptidão ao pedido de homologação.
4. Esta skill é dona do cabimento da RE rural. Para PJ rural, conferir ECF ou obrigação substitutiva entregue tempestivamente (48 §2º). Para PF rural, conferir LCDPR ou substituto, DIRPF e balanço patrimonial, todos tempestivos (§3º); quando LCDPR ainda não era exigível, conferir livro-caixa utilizado para DIRPF (§4º). No §5º, receitas, bens, despesas, custos e dívidas organizados segundo legislação/padrão contábil, regime de competência e balanço elaborado por contador habilitado. Cada documento precisa cobrir o período provado; ausência de recibos/contador é pendência, sem presumir regularidade.
5. Norma registral, requisito rural adicional ou entendimento jurisprudencial que não esteja capturado fica 🟡, com indicação da fonte/prova necessária. Não importar automaticamente regras de sujeição rural da RJ do art. 49 §§6º–9º para RE. Encaminhar a classificação a `creditos-sujeitos-e-excluidos-da-re`.

## Saída e limites

Entregar matriz cumulativa de elegibilidade/impedimentos e cronologia com datas documentadas. Não chamar o produtor rural de fora do recorte apenas por ser rural. RE inviável exige explicar o impedimento e orientar avaliação de RJ; RJ rural e renegociação agrária específica são encaminhamentos opcionais, sem inventar comando ou disponibilidade do irmão e sem elaborar inicial de RJ. Sem prova, emitir pendência; impedimento comprovado bloqueia a etapa correspondente, não apaga o histórico.

## Controles e entrega

Em toda chamada, inclusive direta, aplicar `triagem-recuperacao-extrajudicial`: fixar cliente/lado, atividade, etapa, modalidade (162/163), data de corte e objetivo. Lado indefinido limita a coleta; representação dos lados opostos no mesmo caso bloqueia produção. Administrador judicial está fora do recorte. Guardar dados somente em workspace privado por cliente/matéria, nunca no source; nenhum envio externo sem autorização específica.

Ler os anexos literais indicados em `context/`, com `INDICE.md` e `manifesto-captura.json`; registrar dispositivo, linhas, trecho, versão/captura e documento do caso. Captura de 01/10/2026 não prova vigência posterior. Buscas podem normalizar Unicode para NFC em memória, preservando os originais verbatim. Artigo, remissão ou prova ausente = 🟡; contradição ou hipótese vedada = 🔴. Não usar memória ou fonte externa para preencher norma ausente.

Ao encerrar, chamar nesta ordem `anti-alucinacao-recuperacao-extrajudicial`, `validador-recuperacao-extrajudicial` e `suprema-corte-recuperacao-extrajudicial` (R1→R4). Registrar achados e correções: R1 fatos/provas/lado; R2 fundamentos e tensões; R3 tese, objeções e requisitos; R4 completude, sigilo e fronteiras. Falta de controle impede entrega conclusiva; não dizer que uma revisão foi executada sem registro. São instruções ao agente (guidance only), sem enforcement automático comprovado.

Entregar quadro **requisito → fonte → fato → prova/arquivo/trecho → resultado → pendência**, identificando cliente/lado, atividade, operação/modalidade, data de corte, créditos/grupos, valores/origem, garantias, adesões/poderes, cronologia comprovada, fontes e responsável por cada falta. Emitir `PREPARAÇÃO CONDICIONADA À REVISÃO HUMANA`, `PENDENTE DE PROVA`, `BLOQUEADO` ou `FORA DO RECORTE`, com motivo, etapa afetada e próxima providência. Minuta não é protocolo, assinatura, comunicação ou negociação pelo cliente; não afirmar homologação, suspensão ou vinculação sem ato e fundamento comprovados. Suporte: luis@sbroggio.io.
