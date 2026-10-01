---
name: resposta-do-devedor-a-impugnacao
description: "Prepara manifestação do devedor sobre impugnação ao plano de RE, verificando fatos, quórum, representação e marco do prazo de cinco dias. Use quando o advogado do devedor receber impugnação do art. 164."
---

# Resposta do devedor à impugnação

## Entrada, fonte e fronteira

Atue pelo advogado do devedor ou do credor identificado, nunca como administrador judicial. Execute `triagem-recuperacao-extrajudicial` antes de qualquer produção, inclusive invocação direta. Confirme cliente, lado, poderes, empresa/atividade rural ou não, modalidade (162/163), operação, etapa, data do pedido e documentos. Representação de interesses opostos no mesmo caso bloqueia a entrega; lado desconhecido exige esclarecimento, sem preparar as duas peças adversárias. RE rural permanece neste plugin, com cabimento em `cabimento-e-requisitos-da-re`; RJ rural e renegociação específica seguem para a especialização agrária.

Leia somente os textos literais de `context/`; sínteses desta skill não substituem o corpus. Registre diploma/dispositivo, arquivo/linhas/trecho, URL e data da captura do cabeçalho, data do fato/ato e alcance. ✅ significa trecho localizado, não vigência posterior ou procedência; 🟡 significa fonte, prova ou interpretação pendente; 🔴 identifica erro/contradição ou hipótese bloqueada. Remissão não lida continua 🟡. Não citar jurisprudência por memória, nem converter texto tachado em regra vigente. O corpus preserva acentos combinantes da fonte: buscar por dispositivo/linha; eventual NFC serve apenas à localização, sem reescrever a fonte ou alterar citações literais.

Dados reais permanecem na pasta privada escolhida, separados por cliente/matéria, nunca no source do plugin. Não enviar cartas, propostas, petições ou documentos; não protocolar, assinar, negociar nem contatar terceiros pelo cliente. Relato identificado não prova evento processual; ausência de documento é desconhecimento, não prova negativa.

## Entrada específica

Receba impugnação integral/anexos, ato dos autos que abre a manifestação, prova da comunicação, pedido/plano/versões, documentos contábeis e de crédito, registro das adesões/poderes, cálculos e decisões. Confirme atuação pelo devedor; não produzir simultaneamente ataque pelo credor.

## Âncoras

Leia `context/lei-11101-recuperacao-extrajudicial.md:31–81`, arts. 163–164, especialmente 164 §§3º–6º; `context/lei-11101-convolacao-falencia.md:79–109`, art. 94 III; `context/lei-11101-compilada-integral.md:1691–1711`, arts. 129–131; `context/lei-11101-disposicoes-finais.md:15–23`, art. 189 §1º.

## Procedimento e limites

1. 164 §4º abre 5 dias para manifestação quando apresentada impugnação. O prazo do devedor não começa automaticamente no edital ou na data escrita pelo credor. Obtenha marco nos autos e encaminhe a `publicidade-prazos-e-decisao-da-re`; dias corridos pela LREF. Regra complementar de início/contagem não capturada fica 🟡, sem prazo final ou tempestividade fabricados.
2. Decomponha cada alegação do credor, fundamento no 164 §3º, fatos, prova e pedido; indique resposta, documento que a sustenta e lacuna. Não tratar I–III como cumulativos nem rejeitar toda impugnação por faltar um deles. Exigência externa só pode ser enfrentada afirmativamente após texto capturado.
3. Conteste quórum com registro de `adesoes-e-poderes-na-re` e memória de `quorum-e-trilha-de-um-terco`, por grupo validado. Não contar excluído, duplicado ou poderes pendentes; distinguir estágio do ingresso de 1/3 e obrigação de complemento em 90 dias de quórum final estritamente superior à metade. Não somar grupos nem ressuscitar classes revogadas de 83 IV/V.
4. Para ato do 94 III, enfrentar alínea, conduta e prova; para 130, separar intenção de prejudicar, conluio fraudulento e efetivo prejuízo. Negação genérica não substitui documento. 🟡 A ressalva de 94 III diz plano judicial; 131 também menciona RE, mas restrita aos atos de 129 I/II/III/VI previstos e realizados na forma do plano. Registrar tese/objeção e alcance interpretativo pendente; nunca usar 131 como imunidade universal a fraude/130.
5. Pelo 164 §6º, prova de simulação de créditos ou vício de representação dos signatários exige indeferimento: não minimizar como irregularidade automaticamente sanável. Identifique o que é provado, controverso, faltante ou corrigível por ato real e validado. Não inventar nova assinatura, retificação, adesão, convalidação ou deferimento; mudança de documento/plano exige cronologia e nova análise dos efeitos.
6. 164 §5º exige apreciação judicial e ausência de atos do 130/outras irregularidades; cumprir o prazo da defesa não prova homologação. Registre pontos não refutados e documentos urgentes para o advogado, sem omitir evidência desfavorável. Recurso e resposta recursal completa ficam fora do recorte.

## Entrega específica

Minuta de manifestação do devedor, quando permitida, com marco provado, síntese de cada impugnação, respostas individualizadas, documentos/cálculos e requerimentos sustentados. Quadro `alegação → fundamento → prova do credor → contraponto/prova do devedor → sanável/impeditivo/controverso → pendência`. Sem suporte essencial, entregar mapa de resposta e documentos, sem peça que certifique regularidade fictícia.

## Saída e revisão obrigatória

Entregue cliente/lado, modalidade, empresa/atividade, data de corte, créditos/grupos, valores/origem/documentos, garantias, adesões/poderes, cronologia comprovada, fontes, pendências com responsável, próxima providência e limite da automação. Inclua `requisito → fonte → fato → prova/trecho → resultado → pendência`. Minuta permitida recebe identificação de proposta para revisão humana; lacuna impeditiva limita a entrega a diagnóstico e mapa de provas, sem trecho utilizável baseado em premissa não provada.

Feche com `PREPARAÇÃO CONDICIONADA À REVISÃO HUMANA`, `PENDENTE DE PROVA`, `BLOQUEADO` ou `FORA DO RECORTE`. Não declarar plano homologado, crédito vinculado, prazo suspenso, assinatura válida, pagamento ou decisão sem prova e fundamento. Ao final, chame nesta ordem `anti-alucinacao-recuperacao-extrajudicial`, `validador-recuperacao-extrajudicial` e `suprema-corte-recuperacao-extrajudicial`, R1→R4: fatos/provas; fundamentos/remissões/vigência; tese/objeção pelo lado representado; completude/limites/sigilo. Corrija ou retire trechos reprovados. Dependência ausente ou inexequível gera revisão pendente e impede apresentar a saída como revisada. Controles por instrução (guidance only), sem enforcement por hook. Suporte: luis@sbroggio.io.
