---
name: recuperacao-extrajudicial-master
description: "Coordena pedidos de recuperação extrajudicial pelo advogado do devedor ou do credor, inclusive rural, com triagem, roteamento local e revisão R1→R4."
---

# Coordenação da RE pelo advogado do devedor ou do credor

## Entrada e sequência obrigatória

Receber pedido, configuração privada e documentos. Reconfirmar cliente e lado **por caso**, empresa/atividade (inclusive rural), objetivo, fase, modalidade pretendida, processos, passivo, garantias, datas e prova dos atos. Sem lado/documentos, coletar o mínimo e produzir apenas matriz de pendências. Administrador judicial é fora do recorte; representação oposta no mesmo caso bloqueia.

Executar `triagem-recuperacao-extrajudicial`, `anti-alucinacao-recuperacao-extrajudicial` e `validador-recuperacao-extrajudicial` antes das produtoras. Triagem interna retorna ao master; controles não se chamam recursivamente. Selecionar o destino pelo objetivo/lado/provas e verificar `<nome>` antes de executar. Destino ausente gera dependência explícita, nunca conteúdo improvisado. Após cada resultado, repetir guard/validador e fechar com `suprema-corte-recuperacao-extrajudicial` R1→R4, inclusive saída bloqueada e comandos diretos. Registrar rodadas reais, sem simular revisores independentes. Guidance only: instruções ao agente; nenhum hook certifica cumprimento.

## Rol exato de 24 destinos

| Destino | Quando usar |
|---|---|
| `recuperacao-extrajudicial-install` | Configurar ambiente privado e primeiro uso |
| `recuperacao-extrajudicial-master` | Coordenar jornada por lado e modalidade |
| `triagem-recuperacao-extrajudicial` | Fixar cliente, lado, atividade, etapa e objetivo |
| `anti-alucinacao-recuperacao-extrajudicial` | Verificar existência e rastreabilidade de fatos/citações |
| `validador-recuperacao-extrajudicial` | Conferir subsunção, denominador, requisitos e efeitos |
| `suprema-corte-recuperacao-extrajudicial` | Revisão R1→R4 de toda produção |
| `cabimento-e-requisitos-da-re` | Testar elegibilidade e impedimentos |
| `creditos-sujeitos-e-excluidos-da-re` | Classificar crédito e grupo |
| `garantias-e-anuencias-na-re` | Testar alcance sobre garantias |
| `dossie-documental-da-re` | Preparar prova e instrução |
| `mediacao-e-conciliacao-antecedentes` | Mapear negociação antecedente e vedações |
| `negociacao-do-devedor-na-re` | Preparar posição negocial do devedor |
| `negociacao-do-credor-na-re` | Preparar posição do credor |
| `plano-consensual-da-re` | Estruturar plano pela modalidade consensual |
| `plano-de-extensao-da-re` | Estruturar grupos e proposta de extensão |
| `adesoes-e-poderes-na-re` | Conferir prova de adesão e representação |
| `quorum-e-trilha-de-um-terco` | Demonstrar denominadores, limiares e complementação |
| `pedido-de-homologacao-da-re` | Montar pedido e instrução do devedor |
| `analise-do-plano-pelo-credor` | Avaliar inclusão, tratamento e riscos |
| `impugnacao-do-credor-na-re` | Estruturar impugnação do art. 164 |
| `resposta-do-devedor-a-impugnacao` | Responder motivos e evidências do credor |
| `publicidade-prazos-e-decisao-da-re` | Organizar comunicação, marcos e decisão |
| `efeitos-e-cumprimento-da-re` | Mapear efeitos e monitorar obrigações |
| `quando-a-re-nao-serve-e-ponte-para-rj` | Identificar limite da RE e organizar encaminhamento |

## Contratos de passagem e filtros

- `cabimento-e-requisitos-da-re` é dona do cabimento rural: art. 161 caput → 48 §§2º–5º; RE rural não é encaminhada integralmente ao agrário. RJ rural e renegociação específica vão ao agrário; RJ empresarial fica em `recuperacao-judicial-os`, sem produzir RJ aqui. Verificar disponibilidade do irmão, sem inventar slash command nem exigir aquisição.
- `analise-do-plano-pelo-credor` entrega parecer → `negociacao-do-credor-na-re` consome; `adesoes-e-poderes-na-re` entrega registro admitido → `quorum-e-trilha-de-um-terco` calcula somente sobre ele. Lado credor não recebe tese do devedor por padrão.
- Cabimento exige análise cumulativa de art. 48: atividade regular há mais de 2 anos; impedimento de RJ anterior há menos de 5 anos (II/III), cumulando com art. 161 §3º (RJ pendente e RJ/RE há menos de 2 anos). Para RJ anterior, 5 anos é mais restritivo. Fatos desconhecidos não equivalem a ausência de impedimento.
- Distinguir arts. 162/163; tensão 161 §1º × 163 §1º: não computar espécie trabalhista/acidente na extensão sem negociação coletiva comprovada **e** enquadramento validado; multas não têm sujeição presumida. Tributário/49 §3º/86 II ficam fora, observadas remissões e provas.
- Quórum por espécie/grupo validado: centavos exatos; `2*A > T` e, para ingresso do §7º, `3*A >= T`, total positivo. 1/3 não basta para extensão final: compromisso de complemento em 90 dias improrrogáveis da data do pedido, conversão só a pedido do devedor. Não calcular por cabeça, arredondar metade, somar grupos insuficientes, contar duplicado/relacionado do art. 43/crédito excluído ou poderes pendentes. Câmbio da véspera da assinatura precisa de fonte/data/taxa.
- Confrontar 161 §4º e 163 §8º: pedido não gera stay universal; alcance restrito às espécies abrangidas e ratificação condicionada ao quórum inicial comprovado. Negociação/mediação não suspende por si todos os prazos; 20-B IV/§1º antecede RJ, §3º desconta suspensão também na RE; 20-C p.u. alcança RE.
- Sem anuência própria, não suprimir/substituir garantia real na alienação (163 §4º), afastar variação cambial (§5º) nem liberar coobrigado por inferência. Pedido não equivale à homologação (165); efeitos antecipados só valor/forma de pagamento dos signatários, com restauração e dedução se rejeitado.
- Publicidade/prazos: edital e cartas comprovados; 30 dias para impugnar com prova do crédito; 5 ao devedor e 5 ao juiz, com marcos provados; dias corridos pelo 189 §1º I. 189 §1º II: “as decisões proferidas nos processos a que se refere esta Lei serão passíveis de agravo de instrumento, exceto nas hipóteses em que esta Lei previr de forma diversa”; a apelação da sentença do 164 §7º é hipótese diversa; apelação sem efeito suspensivo e agravo são orientação, sem recurso completo ou prazo CPC fabricado.

## Âncoras locais e lacunas

Ler `context/lei-11101-recuperacao-extrajudicial.md` (161–167), `context/lei-11101-disposicoes-comuns.md` (1º–3º/6º/20-A–20-D/43), `context/lei-11101-recuperacao-judicial.md` (48/49 §3º/51 II), `context/lei-11101-disposicoes-finais.md` (189 §1º), `context/lei-11101-compilada-integral.md` (83/86 II/130/131/142), `context/lei-11101-convolacao-falencia.md` (94 III), `context/cpc-recuperacao.md` (305) e `context/lei-13140-mediacao.md` (16–17), conforme etapa. CPC 305 e mediação 16–17 estão capturados; CPC 306–310 seguem 🟡. Registrar 🟡 94 III (ressalva de plano judicial) × 131 (judicial/extrajudicial); não resolver por equiparação automática. Incisos 83 IV/V revogados e CPC/1973 584 III são remissões históricas, nunca vigência reconstruída. Preservar anomalia literal “art. 43 deste artigo” no 163 §3º II. Rito recursal completo, leilão e critérios externos do ACC não capturados bloqueiam suas entregas dependentes.

## Fontes, sigilo e estado de entrega

Usar exclusivamente texto literal de `context/`, documentos do caso e relatos atribuídos. Índice, URL, memória e resumo não suprem artigo ausente. Não consultar Jusbrasil/Escavador nem completar o corpus pela internet nesta execução. Registrar arquivo, dispositivo, linhas/trecho, versão, data de captura e alcance. ✅ significa texto conferido no recorte; 🟡 significa fonte, prova, atualização ou interpretação pendente; 🔴 significa contradição ou hipótese bloqueada. Captura não certifica atualização posterior nem fato do caso. Buscas podem comparar Unicode em NFC apenas em memória: preservar os originais verbatim, tachados e remissões; cabeçalho editorial não é norma. Hash do HTML identifica snapshot, não prova texto atual.

Dados ficam em workspace privado, separados por cliente e matéria, fora do source e de repositórios compartilhados. Não enviar documentos a conectores/serviços sem autorização específica; não inventar integração disponível. Norma ética/LGPD não capturada recebe 🟡 sem número de artigo inventado. Não representar lados opostos no mesmo caso. Minuta é proposta: envio, assinatura, negociação, protocolo e decisões exigem atuação humana autorizada. Suporte: suporte@iapx.pro.

Entregar cliente/lado, empresa/atividade, objetivo/modalidade, data de corte, créditos/grupos, valores e origem, garantias, adesões/poderes, cronologia comprovada e matriz **requisito → fonte → fato → prova/trecho → resultado → pendência/responsável**. Fechar com `PREPARAÇÃO CONDICIONADA À REVISÃO HUMANA`, `PENDENTE DE PROVA`, `BLOQUEADO` ou `FORA DO RECORTE`, indicando próxima providência e limite da automação. Não afirmar homologação, suspensão, vinculação ou assinatura válida sem prova e fundamento.
