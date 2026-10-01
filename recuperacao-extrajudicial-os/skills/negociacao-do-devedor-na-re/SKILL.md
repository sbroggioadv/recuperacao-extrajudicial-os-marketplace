---
name: negociacao-do-devedor-na-re
description: "Prepara agenda e proposta não vinculante do devedor na recuperação extrajudicial com passivo, caixa e garantias documentados."
---

# Negociação do devedor na RE

## Entradas e fontes

Confirmar advogado do devedor; receber mapa de passivo validado, fluxo de caixa e premissas identificadas, condições de contratos, garantias, adesões/poderes e objetivos. Ler `context/lei-11101-recuperacao-extrajudicial.md:17–57,83–91` (161 §§1º–5º, 162–163, 165–167); para antecedente, `context/lei-11101-disposicoes-comuns.md:227–249` (20-A–20-D).

## Execução

1. Consumir as matrizes de `cabimento-e-requisitos-da-re`, `creditos-sujeitos-e-excluidos-da-re`, `garantias-e-anuencias-na-re` e `dossie-documental-da-re`. Sem cabimento/passivo comprovados, limitar proposta a cenário condicionado; nunca apresentar como devedor elegível fato ainda pendente.
2. Separar acordo privado do 167, plano consensual do 162 e extensão do 163. Mapear condições e público alcançado, interesses, prioridades e alternativas. Não chamar acordo bilateral de plano vinculante a dissidentes; não chamar extensão de cram down da RJ.
3. Preparar deságio, parcelas, vencimentos e cenários somente sobre valores fornecidos. Explicitar premissas, fontes, incertezas, desembolso e limite de caixa; sem dados, não estimar viabilidade, fluxo ou retorno. Não prometer adesão, crédito novo ou recebimento.
4. Pelo 161 §2º, recusar pagamento antecipado de dívidas e tratamento desfavorável a não sujeitos. Exclusões e não incluídos não entram no denominador nem têm condições alteradas pelo plano; não oferecer renúncia de terceiro. Trabalhista exige negociação coletiva comprovada e enquadramento validado para extensão, com tensão 161 §1º × 163 §1º expressa.
5. Supressão/substituição de garantia real na alienação e afastamento de variação cambial exigem anuências expressas próprias (163 §§4º–5º). Proposta não cria aprovação. Efeito antecipado do 165 §1º limita-se a valor/forma de pagamento de signatários; rejeição restaura condições com dedução do pago (§2º).
6. Preparar agenda, argumentos e minuta não vinculante, com reservas e itens negociáveis/não negociáveis. Se houver antecedente, chamar `mediacao-e-conciliacao-antecedentes`; não prometer suspensão de 60 dias à RE. Natureza/classificação e critérios de voto não são moeda de acordo.
7. Enviar condições documentadas às skills de plano da modalidade escolhida. Assinaturas/poderes vão a `adesoes-e-poderes-na-re`; quórum só recebe o registro admitido por essa skill. Não contar intenção verbal de adesão nem retirar signatário após distribuição sem anuência expressa dos demais (161 §5º).

## Saída

Agenda e proposta não vinculante: crédito/grupo, cláusula, premissa financeira, prova, garantia/anuência, risco, contraponto provável, responsável e próximo passo. Não negociar pelo cliente, enviar oferta, assinar, protocolar ou converter em RJ. RE inviável gera encaminhamento fundamentado, sem elaboração de RJ.

## Controles e entrega

Em toda chamada, inclusive direta, aplicar `triagem-recuperacao-extrajudicial`: fixar cliente/lado, atividade, etapa, modalidade (162/163), data de corte e objetivo. Lado indefinido limita a coleta; representação dos lados opostos no mesmo caso bloqueia produção. Administrador judicial está fora do recorte. Guardar dados somente em workspace privado por cliente/matéria, nunca no source; nenhum envio externo sem autorização específica.

Ler os anexos literais indicados em `context/`, com `INDICE.md` e `manifesto-captura.json`; registrar dispositivo, linhas, trecho, versão/captura e documento do caso. Captura de 01/10/2026 não prova vigência posterior. Buscas podem normalizar Unicode para NFC em memória, preservando os originais verbatim. Artigo, remissão ou prova ausente = 🟡; contradição ou hipótese vedada = 🔴. Não usar memória ou fonte externa para preencher norma ausente.

Ao encerrar, chamar nesta ordem `anti-alucinacao-recuperacao-extrajudicial`, `validador-recuperacao-extrajudicial` e `suprema-corte-recuperacao-extrajudicial` (R1→R4). Registrar achados e correções: R1 fatos/provas/lado; R2 fundamentos e tensões; R3 tese, objeções e requisitos; R4 completude, sigilo e fronteiras. Falta de controle impede entrega conclusiva; não dizer que uma revisão foi executada sem registro. São instruções ao agente (guidance only), sem enforcement automático comprovado.

Entregar quadro **requisito → fonte → fato → prova/arquivo/trecho → resultado → pendência**, identificando cliente/lado, atividade, operação/modalidade, data de corte, créditos/grupos, valores/origem, garantias, adesões/poderes, cronologia comprovada, fontes e responsável por cada falta. Emitir `PREPARAÇÃO CONDICIONADA À REVISÃO HUMANA`, `PENDENTE DE PROVA`, `BLOQUEADO` ou `FORA DO RECORTE`, com motivo, etapa afetada e próxima providência. Minuta não é protocolo, assinatura, comunicação ou negociação pelo cliente; não afirmar homologação, suspensão ou vinculação sem ato e fundamento comprovados. Suporte: luis@sbroggio.io.
