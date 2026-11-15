---
name: publicidade-prazos-e-decisao-da-re
description: "Organiza edital, cartas, manifestação, complemento, decisão e orientação recursal na RE, condicionando marcos à prova dos autos. Use para acompanhar publicidade e prazos do procedimento de homologação."
---

# Publicidade, prazos e decisão da RE

## Entrada, fonte e fronteira

Atue pelo advogado do devedor ou do credor identificado, nunca como administrador judicial. Execute `triagem-recuperacao-extrajudicial` antes de qualquer produção, inclusive invocação direta. Confirme cliente, lado, poderes, empresa/atividade rural ou não, modalidade (162/163), operação, etapa, data do pedido e documentos. Representação de interesses opostos no mesmo caso bloqueia a entrega; lado desconhecido exige esclarecimento, sem preparar as duas peças adversárias. RE rural permanece neste plugin, com cabimento em `cabimento-e-requisitos-da-re`; RJ rural e renegociação específica seguem para a especialização agrária.

Leia somente os textos literais de `context/`; sínteses desta skill não substituem o corpus. Registre diploma/dispositivo, arquivo/linhas/trecho, URL e data da captura do cabeçalho, data do fato/ato e alcance. ✅ significa trecho localizado, não vigência posterior ou procedência; 🟡 significa fonte, prova ou interpretação pendente; 🔴 identifica erro/contradição ou hipótese bloqueada. Remissão não lida continua 🟡. Não citar jurisprudência por memória, nem converter texto tachado em regra vigente. O corpus preserva acentos combinantes da fonte: buscar por dispositivo/linha; eventual NFC serve apenas à localização, sem reescrever a fonte ou alterar citações literais.

Dados reais permanecem na pasta privada escolhida, separados por cliente/matéria, nunca no source do plugin. Não enviar cartas, propostas, petições ou documentos; não protocolar, assinar, negociar nem contatar terceiros pelo cliente. Relato identificado não prova evento processual; ausência de documento é desconhecimento, não prova negativa.

## Entrada específica

Receba cliente/lado, número/juízo comprovados, modalidade, recibo de distribuição, edital eletrônico e prova da publicação, destinatários e comprovantes das cartas, impugnações, atos de abertura de prazo/intimações, conclusões, sentença e versões do plano. Documento sem data verificável permanece pendência.

## Âncoras

Leia `context/lei-11101-recuperacao-extrajudicial.md:55–81`, arts. 163 §§7º–8º e 164; `context/lei-11101-disposicoes-finais.md:15–23`, art. 189 §1º I–II. Não substituir remissão ao CPC por prazo conhecido de memória.

## Procedimento e limites

1. 164 caput: o juiz ordena edital eletrônico ao receber pedido de 162/163. Registrar ordem, publicação e prova de acesso nos autos separadamente. Não inventar edital a partir da distribuição ou considerar carta individual equivalente à publicação.
2. 164 §1º: no prazo do edital o devedor comprova envio de carta a todos os credores sujeitos domiciliados/sediados no país, com distribuição, condições do plano e prazo de impugnação. Compare relação nominal a comprovantes individualizados. Preparar checklist/minuta de comunicação para envio humano, sem dizer entregue/enviada na falta da prova nem estender automaticamente a exigência textual a destinatários no exterior.
3. 164 §2º: 30 dias ao credor contados da publicação do edital, com prova do crédito. 164 §4º: 5 dias de manifestação do devedor mediante abertura do prazo nos autos após impugnação. Separar esses marcos; comunicação sem suporte é 🟡. Encaminhar imediatamente às skills de impugnação/resposta conforme lado, sem aguardar um vencimento calculado sem prova.
4. 164 §5º: decorrido o prazo do §4º, autos conclusos imediatamente e decisão do juiz em 5 dias. Registrar conclusão, período previsto e decisão real. Decurso não produz homologação, rejeição ou deferimento tácito. Ausência de ato nos documentos recebidos não prova inércia judicial.
5. 163 §7º: quando aplicável, registrar data do pedido, ingresso de pelo menos 1/3 por espécie e compromisso de atingir mais da metade em 90 dias improrrogáveis. Remeter registro/cálculo aos donos de adesões e quórum. Não fabricar prorrogação ou conversão automática. 163 §8º não é suspensão geral: exigir espécies abrangidas, prova do quórum inicial e ato de ratificação para afirmar seu estado.
6. 189 §1º I determina dias corridos para prazos da LREF. Tabela separa evento, documento, data provada, duração/fonte, marco, vencimento confirmado pelo advogado e ato realizado. Sem regra complementar/marco seguro, não inventar primeiro/último dia, feriado, calendário ou tempestividade. Não transferir dias corridos a prazo externo não capturado.
7. Da sentença, 164 §7º: apelação sem efeito suspensivo. 189 §1º II: “as decisões proferidas nos processos a que se refere esta Lei serão passíveis de agravo de instrumento, exceto nas hipóteses em que esta Lei previr de forma diversa”; a apelação da sentença do 164 §7º é hipótese diversa. Prazo/rito recursal completo do CPC não está capturado: 🟡, obter fonte/provas e encaminhar ao advogado, sem recurso pronto ou número de dias de memória. 164 §8º permite novo pedido após não homologação cumpridas formalidades, sem cura automática.

## Entrega específica

Cronologia comprovada, matriz de cartas/destinatários, pendências de autos e quadro de alcance/dispositivo da decisão. Registrar recurso/evento apenas se provado. Encaminhar sentença/plano/pagamentos a `efeitos-e-cumprimento-da-re`; não converter acompanhamento em fiscalização de AJ ou promessa de decisão.

## Saída e revisão obrigatória

Entregue cliente/lado, modalidade, empresa/atividade, data de corte, créditos/grupos, valores/origem/documentos, garantias, adesões/poderes, cronologia comprovada, fontes, pendências com responsável, próxima providência e limite da automação. Inclua `requisito → fonte → fato → prova/trecho → resultado → pendência`. Minuta permitida recebe identificação de proposta para revisão humana; lacuna impeditiva limita a entrega a diagnóstico e mapa de provas, sem trecho utilizável baseado em premissa não provada.

Feche com `PREPARAÇÃO CONDICIONADA À REVISÃO HUMANA`, `PENDENTE DE PROVA`, `BLOQUEADO` ou `FORA DO RECORTE`. Não declarar plano homologado, crédito vinculado, prazo suspenso, assinatura válida, pagamento ou decisão sem prova e fundamento. Ao final, chame nesta ordem `anti-alucinacao-recuperacao-extrajudicial`, `validador-recuperacao-extrajudicial` e `suprema-corte-recuperacao-extrajudicial`, R1→R4: fatos/provas; fundamentos/remissões/vigência; tese/objeção pelo lado representado; completude/limites/sigilo. Corrija ou retire trechos reprovados. Dependência ausente ou inexequível gera revisão pendente e impede apresentar a saída como revisada. Controles por instrução (guidance only), sem enforcement por hook. Suporte: suporte@iapx.pro.
