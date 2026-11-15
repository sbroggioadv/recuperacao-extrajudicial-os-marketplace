---
name: analise-do-plano-pelo-credor
description: "Avalia inclusão, tratamento, garantias e riscos do crédito no plano de RE e entrega parecer para a negociação do credor. Use quando o advogado do credor receber proposta, plano ou edital de recuperação extrajudicial."
---

# Análise do plano pelo credor

## Entrada, fonte e fronteira

Atue pelo advogado do devedor ou do credor identificado, nunca como administrador judicial. Execute `triagem-recuperacao-extrajudicial` antes de qualquer produção, inclusive invocação direta. Confirme cliente, lado, poderes, empresa/atividade rural ou não, modalidade (162/163), operação, etapa, data do pedido e documentos. Representação de interesses opostos no mesmo caso bloqueia a entrega; lado desconhecido exige esclarecimento, sem preparar as duas peças adversárias. RE rural permanece neste plugin, com cabimento em `cabimento-e-requisitos-da-re`; RJ rural e renegociação específica seguem para a especialização agrária.

Leia somente os textos literais de `context/`; sínteses desta skill não substituem o corpus. Registre diploma/dispositivo, arquivo/linhas/trecho, URL e data da captura do cabeçalho, data do fato/ato e alcance. ✅ significa trecho localizado, não vigência posterior ou procedência; 🟡 significa fonte, prova ou interpretação pendente; 🔴 identifica erro/contradição ou hipótese bloqueada. Remissão não lida continua 🟡. Não citar jurisprudência por memória, nem converter texto tachado em regra vigente. O corpus preserva acentos combinantes da fonte: buscar por dispositivo/linha; eventual NFC serve apenas à localização, sem reescrever a fonte ou alterar citações literais.

Dados reais permanecem na pasta privada escolhida, separados por cliente/matéria, nunca no source do plugin. Não enviar cartas, propostas, petições ou documentos; não protocolar, assinar, negociar nem contatar terceiros pelo cliente. Relato identificado não prova evento processual; ausência de documento é desconhecimento, não prova negativa.

## Entrada específica

Receba plano completo e anexos, título e prova do crédito, origem/data de constituição, saldo documentado, vencimentos, garantias/coobrigados, vínculos com devedor, assinaturas, poderes, pedido, edital, decisões e objetivo do credor. Fixe versão do plano e data de corte; proposta sem autos não equivale a pedido distribuído.

## Âncoras

Leia `context/lei-11101-recuperacao-extrajudicial.md:15–87`, arts. 161–165; `context/lei-11101-recuperacao-judicial.md:45`, art. 49, §3º; `context/lei-11101-compilada-integral.md:1209–1263,1303`, arts. 83 e 86, II; `context/lei-11101-disposicoes-comuns.md:545–547`, art. 43. São localizadores, não prova automática de enquadramento.

## Procedimento e limites

1. Encaminhe cabimento e classificação a `cabimento-e-requisitos-da-re` e `creditos-sujeitos-e-excluidos-da-re`. Distinga crédito excluído, incluído, condicionado e controverso. Tributário, 49 §3º e 86 II não entram por conveniência negocial. Trabalhista/acidente exige negociação coletiva; 🔴 na extensão, bloquear denominador sem negociação coletiva comprovada e enquadramento validado diante de 161 §1º × 163 §1º. Multas não são abrangidas por presunção; 83 IV/V revogados não são classes atuais.
2. No art. 162, confronte termos e signatários comprovados. No 163, ausência de assinatura do cliente não significa exclusão: extensão homologada pode atingir os abrangidos nos limites do §1º. Não anunciar vinculação atual sem sentença e prova do crédito/grupo; crédito fora do plano conserva valor/condições originais (§2º).
3. Pelo lado credor fixado na triagem, use o modo auditoria, sem produzir adesão nem plano. Encaminhe adesões a `adesoes-e-poderes-na-re` e memória a `quorum-e-trilha-de-um-terco`. Mais da metade é estrito por espécie/grupo, não contagem de cabeças, soma indiscriminada ou antigo 3/5. Um terço é ingresso condicionado com compromisso de complemento em 90 dias improrrogáveis, não aprovação definitiva. Registre relacionados do art. 43 e a remissão literal defeituosa de 163 §3º II; exija câmbio da véspera da assinatura provado.
4. Compare deságio, prazo, parcelas, juros/atualização, moeda e garantias com contrato e plano; calcule somente com valores comprovados e exponha método. Não estimar recebimento, caixa ou viabilidade sem dados. Por 163 §§4º–5º, supressão/substituição de garantia real na alienação e afastamento de variação cambial exigem aprovações expressas próprias. Não liberar coobrigado ou garantia por mera adesão.
5. Pelo 161 §2º, examine pagamento antecipado de dívidas e tratamento desfavorável a não sujeitos. Confronte 161 §4º com 163 §8º: sem stay universal; suspensão restrita e ratificação dependem dos pressupostos/provas. Pelo 165, efeitos anteriores limitam-se a valor/forma de pagamento dos signatários e exigem previsão; rejeição restaura condições originais, deduzindo pagos.
6. Organize prazo/prova para eventual impugnação em `publicidade-prazos-e-decisao-da-re` e `impugnacao-do-credor-na-re`. Registre regra de desistência de adesão após distribuição (161 §5º), sem autorizar retirada unilateral. A decisão de aderir/negociar/opor-se é do cliente assistido.

## Entrega específica e passagem

Parecer por crédito: inclusão/grupo, tratamento original × proposto, garantia/anuência, alcance condicionado, riscos, opções e provas faltantes. Entregue este parecer a `negociacao-do-credor-na-re`, que o consome para preparar contraproposta e reservas; esta skill não negocia, não envia oferta e não assina adesão. Risco de prazo vai ao acompanhamento, sem ocultá-lo no parecer.

## Saída e revisão obrigatória

Entregue cliente/lado, modalidade, empresa/atividade, data de corte, créditos/grupos, valores/origem/documentos, garantias, adesões/poderes, cronologia comprovada, fontes, pendências com responsável, próxima providência e limite da automação. Inclua `requisito → fonte → fato → prova/trecho → resultado → pendência`. Minuta permitida recebe identificação de proposta para revisão humana; lacuna impeditiva limita a entrega a diagnóstico e mapa de provas, sem trecho utilizável baseado em premissa não provada.

Feche com `PREPARAÇÃO CONDICIONADA À REVISÃO HUMANA`, `PENDENTE DE PROVA`, `BLOQUEADO` ou `FORA DO RECORTE`. Não declarar plano homologado, crédito vinculado, prazo suspenso, assinatura válida, pagamento ou decisão sem prova e fundamento. Ao final, chame nesta ordem `anti-alucinacao-recuperacao-extrajudicial`, `validador-recuperacao-extrajudicial` e `suprema-corte-recuperacao-extrajudicial`, R1→R4: fatos/provas; fundamentos/remissões/vigência; tese/objeção pelo lado representado; completude/limites/sigilo. Corrija ou retire trechos reprovados. Dependência ausente ou inexequível gera revisão pendente e impede apresentar a saída como revisada. Controles por instrução (guidance only), sem enforcement por hook. Suporte: suporte@iapx.pro.
