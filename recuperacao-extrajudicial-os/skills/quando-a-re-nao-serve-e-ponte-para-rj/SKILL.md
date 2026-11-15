---
name: quando-a-re-nao-serve-e-ponte-para-rj
description: "Identifica insuficiência ou impedimentos da RE e prepara pacote de transição para avaliação humana, sem construir recuperação judicial. Use quando cabimento, adesões, passivo ou decisão indicarem limites da RE."
---

# Quando a RE não serve e ponte para RJ

## Entrada, fonte e fronteira

Atue pelo advogado do devedor ou do credor identificado, nunca como administrador judicial. Execute `triagem-recuperacao-extrajudicial` antes de qualquer produção, inclusive invocação direta. Confirme cliente, lado, poderes, empresa/atividade rural ou não, modalidade (162/163), operação, etapa, data do pedido e documentos. Representação de interesses opostos no mesmo caso bloqueia a entrega; lado desconhecido exige esclarecimento, sem preparar as duas peças adversárias. RE rural permanece neste plugin, com cabimento em `cabimento-e-requisitos-da-re`; RJ rural e renegociação específica seguem para a especialização agrária.

Leia somente os textos literais de `context/`; sínteses desta skill não substituem o corpus. Registre diploma/dispositivo, arquivo/linhas/trecho, URL e data da captura do cabeçalho, data do fato/ato e alcance. ✅ significa trecho localizado, não vigência posterior ou procedência; 🟡 significa fonte, prova ou interpretação pendente; 🔴 identifica erro/contradição ou hipótese bloqueada. Remissão não lida continua 🟡. Não citar jurisprudência por memória, nem converter texto tachado em regra vigente. O corpus preserva acentos combinantes da fonte: buscar por dispositivo/linha; eventual NFC serve apenas à localização, sem reescrever a fonte ou alterar citações literais.

Dados reais permanecem na pasta privada escolhida, separados por cliente/matéria, nunca no source do plugin. Não enviar cartas, propostas, petições ou documentos; não protocolar, assinar, negociar nem contatar terceiros pelo cliente. Relato identificado não prova evento processual; ausência de documento é desconhecimento, não prova negativa.

## Entrada específica

Receba lado representado, atividade rural ou não, diagnóstico de cabimento/créditos/garantias, plano/adesões válidas, memória por grupo, cronologia dos pedidos/decisões, passivo e caixa documentados e decisão do advogado. Falta de prova não é impossibilidade definitiva da via.

## Âncoras

Leia `context/lei-11101-recuperacao-extrajudicial.md:15–91`, arts. 161–167, especialmente 161 §§1º/3º/4º, 163 §7º, 164 §8º e 167; `context/lei-11101-recuperacao-judicial.md:17–35`, art. 48, apenas pela remissão de 161 para cabimento; `context/lei-11101-disposicoes-comuns.md:15–31`, arts. 1º–3º.

## Procedimento e limites

1. Consuma a matriz de `cabimento-e-requisitos-da-re`, sem recriar cabimento da RJ. Verificar cumulativos do 48, inclusive atividade regular superior a 2 anos e impedimentos de RJ anterior de 5 anos de II/III, cumulados com pedido de RJ pendente ou RJ/RE anterior em menos de 2 anos do 161 §3º; janela de 5 anos é mais restritiva para RJ anterior. Não sugerir RJ como solução automática de impedimento que também a afete.
2. Separe impedimento jurídico provado, exclusão de crédito essencial à proposta, insuficiência de prova, quórum não alcançado e inadequação econômica relatada. Consuma `creditos-sujeitos-e-excluidos-da-re`, registro de adesões e memória do quórum; não declarar fracasso financeiro ou viabilidade sem dados/perícia humana. Créditos excluídos não passam a sujeitos para tornar a RE conveniente.
3. No 163 §7º, 1/3 autoriza ingresso condicionado, não quórum final; complemento exige mais da metade por espécie em 90 dias improrrogáveis. Conversão para RJ é facultada a pedido do devedor. 🔴 Não automatizar conversão, apresentar vontade do credor como pedido do devedor ou redigir inicial/plano de RJ aqui. Pedido do devedor e ato processual são eventos distintos a comprovar.
4. Não homologação permite novo pedido com formalidades pelo 164 §8º, sem repetição automaticamente válida nem falência obrigatória. 167 mantém outras modalidades de acordo privado. Apresente alternativas de avaliação e limites legais, sem impor migração para produto irmão ou inventar resultado judicial.
5. RE do produtor rural permanece neste plugin: requisitos rurais de 48 §§2º–5º são do cabimento local. Quando o pedido for RJ rural/renegociação agrária específica, encaminhar à especialização agrária, sem copiar suas peças. Para RJ empresarial, destino indicado é `recuperacao-judicial-os`: confirmar disponibilidade antes de invocar qualquer capacidade; ausência do irmão não impede entregar pacote de transição autossuficiente.
6. Se lado credor, produzir nota sobre impacto/limites e providências a avaliar, nunca decisão de ajuizar/converter em nome do devedor. Administrador judicial, falência completa, cobrança/execução geral e reorganização societária ficam fora do recorte. Não transferir dados a outro plugin/serviço sem ação humana autorizada; preservar a pasta privada por matéria.

## Entrega específica

Nota de insuficiência/limite da via: causa e prova, desconhecidos separados, alternativas condicionadas, riscos e decisão que cabe ao advogado/cliente. Pacote de transição com índice de documentos, histórico de RE, créditos/garantias, adesões, cálculos, decisões e lacunas, sem petição/plano de RJ ou comando inventado. A saída para avaliação de RJ recebe `FORA DO RECORTE`; etapas locais pendentes mantêm estado próprio, sem tratar encaminhamento como aprovação da RJ.

## Saída e revisão obrigatória

Entregue cliente/lado, modalidade, empresa/atividade, data de corte, créditos/grupos, valores/origem/documentos, garantias, adesões/poderes, cronologia comprovada, fontes, pendências com responsável, próxima providência e limite da automação. Inclua `requisito → fonte → fato → prova/trecho → resultado → pendência`. Minuta permitida recebe identificação de proposta para revisão humana; lacuna impeditiva limita a entrega a diagnóstico e mapa de provas, sem trecho utilizável baseado em premissa não provada.

Feche com `PREPARAÇÃO CONDICIONADA À REVISÃO HUMANA`, `PENDENTE DE PROVA`, `BLOQUEADO` ou `FORA DO RECORTE`. Não declarar plano homologado, crédito vinculado, prazo suspenso, assinatura válida, pagamento ou decisão sem prova e fundamento. Ao final, chame nesta ordem `anti-alucinacao-recuperacao-extrajudicial`, `validador-recuperacao-extrajudicial` e `suprema-corte-recuperacao-extrajudicial`, R1→R4: fatos/provas; fundamentos/remissões/vigência; tese/objeção pelo lado representado; completude/limites/sigilo. Corrija ou retire trechos reprovados. Dependência ausente ou inexequível gera revisão pendente e impede apresentar a saída como revisada. Controles por instrução (guidance only), sem enforcement por hook. Suporte: suporte@iapx.pro.
