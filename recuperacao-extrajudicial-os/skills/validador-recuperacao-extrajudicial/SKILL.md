---
name: validador-recuperacao-extrajudicial
description: "Valida aplicação normativa, cabimento, créditos, quórum, adesões, prazos e efeitos da RE contra o corpus literal e as provas do caso."
---

# Validador de aplicação normativa, quórum e efeitos

Receber dossiê/rascunho, guard, datas/modalidade, créditos/grupos, registro admitido de adesões e cálculo. Sem entradas, suspender conclusão dependente. Guidance only: instrução ao agente, sem enforcement por hook. Existência da citação não prova pertinência, vigência integral ou cabimento.

## Matriz normativa e corpus

Para cada fundamento registrar arquivo/dispositivo/trecho, URL oficial do cabeçalho, versão/data/captura, hash do corpo quando conferido, fato/data do caso, remissões, alterações/revogações, destinatário/modalidade, selo e alcance. Ler `context/INDICE.md` e `context/manifesto-captura.json`: confrontar todos os arquivos do índice citados nesta cadeia e a presença de seus dispositivos, não apenas nome da lei. Hash do HTML não se compara aos bytes Markdown. Atualização posterior não demonstrada é 🟡. Não alterar corpus nem pesquisar direito externo.

| Controle | Âncora literal em `context/` e condição |
|---|---|
| Cabimento, competência e rural | `lei-11101-disposicoes-comuns.md` 1º–3º; `lei-11101-recuperacao-judicial.md` 48; `lei-11101-recuperacao-extrajudicial.md` 161 caput/§3º: atividade regular há mais de 2 anos, requisitos cumulativos, janelas de 5 anos do 48 II/III e de 2 anos do 161 §3º; RJ pendente impede. Rural: 48 §§2º–5º com documentação e tempestividade próprias, sem rito RJ transplantado |
| Créditos e extensão | RE 161 §1º/163 §§1º–3º; RJ 49 §3º; `lei-11101-compilada-integral.md` 83/86 II: excluir tributário/exclusões legais; distinguir 162/163. 🔴 Espécie trabalhista/acidente não compõe denominador de extensão sem negociação coletiva comprovada **e** enquadramento validado; multas e 83 IX não são abrangidos por presunção. 83 IV/V revogados não voltam a vigorar |
| Adesão e documentos | RE 162/163 §6º/164 §6º: exposição patrimonial, último exercício e demonstrações especiais (RJ 51 II por remissão), poderes para novar/transigir, relação completa e registros. Não exigir automaticamente três exercícios da RJ. Simulação/vício impede; desistência após distribuição só com anuência expressa dos demais signatários (161 §5º) |
| Quórum | RE 163 caput/§§1º–3º/7º: só registro admitido; por espécie/grupo juridicamente validado, T positivo, centavos exatos, `2*A > T`, `3*A >= T`. Fora do plano/art. 43 não computam; deduplicar; câmbio da véspera da assinatura documentado. 1/3 exige compromisso de complemento em 90 dias improrrogáveis desde o pedido; conversão só a pedido do devedor, sem produzir RJ |
| Garantias | RE 163 §§4º–5º: aprovação expressa do titular para supressão/substituição de garantia real na alienação e afastamento cambial; condições distintas, sem liberação presumida de coobrigados |
| Suspensão | RE 161 §4º × 163 §8º; comuns 6º: sem stay universal; espécies abrangidas, ratificação pelo juiz com prova do quórum inicial. Negociação não supre pedido/ratificação |
| Mediação | Comuns 20-A–20-D: não mediar natureza/classificação ou critérios de voto; IV/§1º de 20-B antecede RJ, §3º deduz suspensão também na RE; 20-C p.u.: reconstituição de direitos/garantias originais **se requerida RJ ou RE em até 360 dias contados do acordo pré-processual**, com acordo/pedido comprovados, dedução de valores pagos e ressalva dos atos validamente praticados; não prazo para reconstituir. `cpc-recuperacao.md` 305 e `lei-13140-mediacao.md` 16–17 capturados; 306–310 🟡, sem rito completo |
| Contraditório e prazos | RE 164: edital eletrônico, cartas, 30 dias do edital com prova do crédito; fundamentos taxativos do §3º (não cumulativos), 5 dias ao devedor (§4º), 5 ao juiz (§5º), marcos comprovados. `lei-11101-disposicoes-finais.md` 189 §1º I–II: dias corridos, 189 §1º II: “as decisões proferidas nos processos a que se refere esta Lei serão passíveis de agravo de instrumento, exceto nas hipóteses em que esta Lei previr de forma diversa”; a apelação da sentença do 164 §7º é hipótese diversa; apelação sem efeito suspensivo (164 §7º), sem redigir recurso |
| Tensão na impugnação | `lei-11101-convolacao-falencia.md` 94 III e integral 130/131: ressalva do 94 menciona plano judicial, 131 judicial ou extrajudicial. 🟡 Alcance na RE depende de análise jurídica; não equiparar automaticamente; registrar também na resposta do devedor |
| Efeitos e alienação | RE 165–167; integral 142: efeitos após homologação, antecipados só valor/forma dos signatários, rejeição restaura com dedução; alienação do 166 condicionada ao plano/decisão e 142, sem operar leilão ou declarar ausência universal de sucessão |

Remissões históricas: CPC/1973 584 III no 161 §6º sem correspondência atual inventada; 163 §3º II conserva anomalia “art. 43 deste artigo”, a conferir com comuns 43. Critérios externos do ACC (Lei 4.728 art. 75 e normas específicas), rito recursal CPC e leilão não capturados permanecem 🟡. Não generalizar lacuna para bloquear trabalho independente dela.

Saída: **fundamento → trecho/versão → fato/prova → selo → alcance → divergência/etapa impedida/responsável**, memória de cálculo conferida e versão efetiva. Resultado desconhecido não vira zero. Retornar ao chamador em cadeia; chamada direta fecha com Suprema Corte, sem chamada recursiva. Selos não certificam assinatura/autenticidade, viabilidade financeira, decisão nem sucesso jurídico.

## Fontes, sigilo e estado de entrega

Usar exclusivamente texto literal de `context/`, documentos do caso e relatos atribuídos. Índice, URL, memória e resumo não suprem artigo ausente. Não consultar Jusbrasil/Escavador nem completar o corpus pela internet nesta execução. Registrar arquivo, dispositivo, linhas/trecho, versão, data de captura e alcance. ✅ significa texto conferido no recorte; 🟡 significa fonte, prova, atualização ou interpretação pendente; 🔴 significa contradição ou hipótese bloqueada. Captura não certifica atualização posterior nem fato do caso. Buscas podem comparar Unicode em NFC apenas em memória: preservar os originais verbatim, tachados e remissões; cabeçalho editorial não é norma. Hash do HTML identifica snapshot, não prova texto atual.

Dados ficam em workspace privado, separados por cliente e matéria, fora do source e de repositórios compartilhados. Não enviar documentos a conectores/serviços sem autorização específica; não inventar integração disponível. Norma ética/LGPD não capturada recebe 🟡 sem número de artigo inventado. Não representar lados opostos no mesmo caso. Minuta é proposta: envio, assinatura, negociação, protocolo e decisões exigem atuação humana autorizada. Suporte: luis@sbroggio.io.

Entregar cliente/lado, empresa/atividade, objetivo/modalidade, data de corte, créditos/grupos, valores e origem, garantias, adesões/poderes, cronologia comprovada e matriz **requisito → fonte → fato → prova/trecho → resultado → pendência/responsável**. Fechar com `PREPARAÇÃO CONDICIONADA À REVISÃO HUMANA`, `PENDENTE DE PROVA`, `BLOQUEADO` ou `FORA DO RECORTE`, indicando próxima providência e limite da automação. Não afirmar homologação, suspensão, vinculação ou assinatura válida sem prova e fundamento.
