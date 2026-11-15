---
name: recuperacao-extrajudicial-install
description: "Configura a pasta privada, identidade profissional e preferências para iniciar o recuperacao-extrajudicial-os, sem receber autos nem decidir cabimento."
---

# Instalação e primeiro uso

Configurar o escritório, sem analisar cliente nem pedir autos. Orientar **Passo 0 — Prepare a sua fábrica jurídica**: escolher pasta privada CoWork OS (Windows `C:\CoWork OS`; Mac, pasta CoWork OS na pasta do usuário pelo Finder) e selecioná-la no Cowork, concedendo acesso. Não varrer pastas nem mover documentos. Verificar caminho e acesso concedido antes de gravar: caminho dentro do plugin/repositório compartilhado impede gravação.

Usar **AskUserQuestion**, até quatro opções por pergunta, para escolhas fechadas; dividir listas maiores. Se indisponível, explicar e usar escolhas numeradas, sem fingir botões. Nome/OAB, cidade/e-mail e caminho são texto livre; não inventar dados profissionais.

1. Colher pasta privada em texto livre e conferir acesso e isolamento.
2. Colher identidade profissional opcional (nome/OAB/cidade/e-mail), sem inventar habilitação.
3. Lado habitual: **Devedor**, **Credor**, **Ambos em casos distintos**, **Ainda não definido**. Preferência nunca substitui a identificação por caso; oposição no mesmo caso é bloqueada.
4. Tom: **Objetivo**, **Didático**, **Técnico**. Travas e R1→R4 permanecem ligadas.
5. Mostrar resumo e pedir confirmação da configuração antes de persistir exclusivamente na pasta privada autorizada. Sem caminho/acesso ou confirmação, fornecer resumo sem gravação; nunca declarar configuração salva sem conferir arquivo real.

Explicar portas reais `/recuperacao-extrajudicial-install`, `/recuperacao-extrajudicial-master`, `/recuperacao-extrajudicial-triagem` e `/recuperacao-extrajudicial-revisar`. Exemplo sintético: “Represento o credor; analise o plano e as garantias nos documentos fornecidos, liste provas faltantes e revise em R1→R4”. Não anexar dados reais ao source. RE de produtor rural permanece aqui; RJ rural/renegociação específica são encaminhadas ao agrário. Administrador judicial está fora. Irmãos são opcionais, nunca pré-requisito comercial.

Saída: resumo da configuração, caminho efetivamente usado/pendências, como pedir e limites. Instalação não emite parecer jurídico. Em pedido jurídico subsequente, chamar `recuperacao-extrajudicial-master`; não improvisar análise dentro do install. Guidance only: orientação ao agente, sem enforcement por hook.

## Fontes, sigilo e estado de entrega

Usar exclusivamente texto literal de `context/`, documentos do caso e relatos atribuídos. Índice, URL, memória e resumo não suprem artigo ausente. Não consultar Jusbrasil/Escavador nem completar o corpus pela internet nesta execução. Registrar arquivo, dispositivo, linhas/trecho, versão, data de captura e alcance. ✅ significa texto conferido no recorte; 🟡 significa fonte, prova, atualização ou interpretação pendente; 🔴 significa contradição ou hipótese bloqueada. Captura não certifica atualização posterior nem fato do caso. Buscas podem comparar Unicode em NFC apenas em memória: preservar os originais verbatim, tachados e remissões; cabeçalho editorial não é norma. Hash do HTML identifica snapshot, não prova texto atual.

Dados ficam em workspace privado, separados por cliente e matéria, fora do source e de repositórios compartilhados. Não enviar documentos a conectores/serviços sem autorização específica; não inventar integração disponível. Norma ética/LGPD não capturada recebe 🟡 sem número de artigo inventado. Não representar lados opostos no mesmo caso. Minuta é proposta: envio, assinatura, negociação, protocolo e decisões exigem atuação humana autorizada. Suporte: suporte@iapx.pro.

Entregar cliente/lado, empresa/atividade, objetivo/modalidade, data de corte, créditos/grupos, valores e origem, garantias, adesões/poderes, cronologia comprovada e matriz **requisito → fonte → fato → prova/trecho → resultado → pendência/responsável**. Fechar com `PREPARAÇÃO CONDICIONADA À REVISÃO HUMANA`, `PENDENTE DE PROVA`, `BLOQUEADO` ou `FORA DO RECORTE`, indicando próxima providência e limite da automação. Não afirmar homologação, suspensão, vinculação ou assinatura válida sem prova e fundamento.
