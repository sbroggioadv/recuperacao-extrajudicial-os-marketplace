---
name: efeitos-e-cumprimento-da-re
description: "Mapeia efeitos do plano e pagamentos comprovados, incluindo limites anteriores à homologação, rejeição e alienação judicial de UPI. Use para verificar alcance e cumprimento da recuperação extrajudicial."
---

# Efeitos e cumprimento da RE

## Entrada, fonte e fronteira

Atue pelo advogado do devedor ou do credor identificado, nunca como administrador judicial. Execute `triagem-recuperacao-extrajudicial` antes de qualquer produção, inclusive invocação direta. Confirme cliente, lado, poderes, empresa/atividade rural ou não, modalidade (162/163), operação, etapa, data do pedido e documentos. Representação de interesses opostos no mesmo caso bloqueia a entrega; lado desconhecido exige esclarecimento, sem preparar as duas peças adversárias. RE rural permanece neste plugin, com cabimento em `cabimento-e-requisitos-da-re`; RJ rural e renegociação específica seguem para a especialização agrária.

Leia somente os textos literais de `context/`; sínteses desta skill não substituem o corpus. Registre diploma/dispositivo, arquivo/linhas/trecho, URL e data da captura do cabeçalho, data do fato/ato e alcance. ✅ significa trecho localizado, não vigência posterior ou procedência; 🟡 significa fonte, prova ou interpretação pendente; 🔴 identifica erro/contradição ou hipótese bloqueada. Remissão não lida continua 🟡. Não citar jurisprudência por memória, nem converter texto tachado em regra vigente. O corpus preserva acentos combinantes da fonte: buscar por dispositivo/linha; eventual NFC serve apenas à localização, sem reescrever a fonte ou alterar citações literais.

Dados reais permanecem na pasta privada escolhida, separados por cliente/matéria, nunca no source do plugin. Não enviar cartas, propostas, petições ou documentos; não protocolar, assinar, negociar nem contatar terceiros pelo cliente. Relato identificado não prova evento processual; ausência de documento é desconhecimento, não prova negativa.

## Entrada específica

Receba cliente/lado, plano e versões, sentença/decisões comprovadas, crédito/grupo/garantias, assinaturas/anuências, cláusulas de efeitos antecipados, cronograma, extratos/recibos, eventos de inadimplemento, acordo antecedente e eventual pedido posterior. Não confundir saldo alegado e pagamento confirmado.

## Âncoras

Leia `context/lei-11101-recuperacao-extrajudicial.md:15–91`, arts. 161–167; `context/lei-11101-disposicoes-comuns.md:33–79,243–247`, arts. 6º, 20-B §3º e 20-C; `context/lei-11101-compilada-integral.md:1783–1837`, art. 142, apenas no alcance da remissão do 166.

## Procedimento e limites

1. Pelo 165 caput, efeitos do plano após homologação judicial. Identifique sentença real, versão homologada, crédito abrangido e condições; pedido distribuído/proposta/adesão não provam homologação. No 163, alcance segue §1º e créditos constituídos até pedido; no 162, signatários comprovados. Não alterar crédito fora do plano contra 163 §2º.
2. 165 §1º permite previsão de efeitos anteriores exclusivamente sobre modificação de valor ou forma de pagamento dos signatários. Exigir cláusula e assinatura válida; 🔴 não antecipar liberação de garantia, efeito a dissidente ou alteração universal. Pelo §2º, rejeição nessa hipótese restitui direito às condições originais, deduzidos valores efetivamente pagos. Mostrar base original, comprovantes, dedução e saldo verificável; sem dados, saldo pendente.
3. 161 §4º versus 163 §8º: não afirmar suspensão universal. Identificar espécie abrangida, pedido, quórum inicial e ratificação judicial condicionada. Garantia real na alienação e afastamento cambial observam anuências expressas de 163 §§4º–5º. Não liberar coobrigado por inferência nem prometer blindagem patrimonial.
4. 20-C exige homologação do acordo pelo juízo competente; p.u.: se RJ ou RE requerida em até 360 dias do acordo pré-processual, reconstituir direitos/garantias originais, deduzir pagamentos e ressalvar atos validamente praticados. Exigir prova do acordo, pedido, datas e atos; não generalizar a qualquer negociação. 20-B §3º também alcança RE: período da suspensão antecedente deduzido da suspensão do art. 6º conforme pressupostos; não tratar 20-B IV/§1º como cautelar automática da RE.
5. 166: alienação judicial de filial/UPI prevista no plano homologado depende de ordem judicial e remete a 142 no que couber. Ler texto vigente, preservando incisos/parágrafos revogados; não importar prazo de 180 dias expressamente falimentar ou condições de RJ para RE por automatismo. 🟡 Alcance de modalidades/rito no caso exige decisão e validação; CPC do leilão não capturado não é completado por memória. Não operar leilão, fixar lance ou declarar ausência universal de sucessão.
6. Compare obrigação, marco, documento, valor previsto, valor efetivamente pago, saldo e divergência; cálculo com origem/prova e parâmetros contratuais, sem contabilidade fictícia. Inadimplemento não causa falência/convolação automática e não transforma esta skill em execução geral, ação falimentar ou AJ. Identifique providências que o advogado deve avaliar no instrumento/decisão e limites da fonte disponível.
7. 167 preserva outros acordos privados, sem homologação ou extensão presumidas. Rejeição pode levar a novo pedido formalmente regular por 164 §8º ou à avaliação de saída; encaminhe a `quando-a-re-nao-serve-e-ponte-para-rj`, sem produzir RJ.

## Entrega específica

Quadro de alcance e efeitos com fonte/cláusula/decisão/prova; relatório de cumprimento por obrigação e memória de dedução, pendências e medidas a avaliar pelo advogado. Não certificar quitação ou desonerar garantias sem documento e base; não assumir fiscalização/relatório de administrador judicial.

## Saída e revisão obrigatória

Entregue cliente/lado, modalidade, empresa/atividade, data de corte, créditos/grupos, valores/origem/documentos, garantias, adesões/poderes, cronologia comprovada, fontes, pendências com responsável, próxima providência e limite da automação. Inclua `requisito → fonte → fato → prova/trecho → resultado → pendência`. Minuta permitida recebe identificação de proposta para revisão humana; lacuna impeditiva limita a entrega a diagnóstico e mapa de provas, sem trecho utilizável baseado em premissa não provada.

Feche com `PREPARAÇÃO CONDICIONADA À REVISÃO HUMANA`, `PENDENTE DE PROVA`, `BLOQUEADO` ou `FORA DO RECORTE`. Não declarar plano homologado, crédito vinculado, prazo suspenso, assinatura válida, pagamento ou decisão sem prova e fundamento. Ao final, chame nesta ordem `anti-alucinacao-recuperacao-extrajudicial`, `validador-recuperacao-extrajudicial` e `suprema-corte-recuperacao-extrajudicial`, R1→R4: fatos/provas; fundamentos/remissões/vigência; tese/objeção pelo lado representado; completude/limites/sigilo. Corrija ou retire trechos reprovados. Dependência ausente ou inexequível gera revisão pendente e impede apresentar a saída como revisada. Controles por instrução (guidance only), sem enforcement por hook. Suporte: luis@sbroggio.io.
