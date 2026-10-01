---
description: "Conduzir a jornada de RE pelo advogado do devedor ou do credor."
argument-hint: "[pedido e documentos pertinentes]"
---

# /recuperacao-extrajudicial-master

Ler e executar `recuperacao-extrajudicial-master`; reconfirmar cliente/lado, aplicar triagem, guard e validador antes de produtoras, verificar destino real, repetir controles sobre o resultado e fechar com Suprema Corte R1→R4. Falta de destino não permite improviso.

Entrada: $ARGUMENTS

Cliente/lado definidos antes da análise. Usar exclusivamente texto literal local em `context/`, sem memória para artigos/fatos nem consulta a Jusbrasil/Escavador. Saída: `PREPARAÇÃO CONDICIONADA À REVISÃO HUMANA`, `PENDENTE DE PROVA`, `BLOQUEADO` ou `FORA DO RECORTE`, com provas, fontes, pendências e responsável. Não presumir suspensão, homologação ou assinatura; não enviar, assinar, aderir, protocolar ou atuar como administrador judicial. Dados exclusivamente na matéria privada. Controles por instrução (Guidance only), sem alegação de enforcement por hook.

Controles locais exatos: `anti-alucinacao-recuperacao-extrajudicial` → `validador-recuperacao-extrajudicial` → `suprema-corte-recuperacao-extrajudicial` R1→R4.
