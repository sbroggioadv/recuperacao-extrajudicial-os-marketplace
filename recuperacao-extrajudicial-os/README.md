# Recuperação Extrajudicial OS

Versão 0.1.1 — estrutura inicial em desenvolvimento. Rol aprovado pelo Doc 01/10: 24 skills e 12 comandos; skills e commands ainda vazios nesta entrega de estrutura. Esta versão não está publicada e não constitui capacidade jurídica operacional.

Público: advogado do devedor ou do credor, com lado definido por caso; administrador judicial fora. Preço decidido: R$ 398. Suporte: suporte@iapx.pro.

## Recorte e fronteiras

Recuperação extrajudicial dos arts. 161–167 da Lei 11.101/2005, inclusive RE do produtor rural; mediação/conciliação dos arts. 20-A–20-D no alcance do corpus. A futura skill `cabimento-e-requisitos-da-re` será dona do cabimento rural por 161 caput → 48 §§2º–5º. RJ rural e renegociação agrária específica permanecem no agrário. RJ completa, falência completa, administração judicial, contabilidade e atuação externa automática ficam fora.

As portas previstas são `/recuperacao-extrajudicial-install` e `/recuperacao-extrajudicial-master`; ainda não estão disponíveis nesta estrutura. Não há comandos operacionais nesta lane.

## Corpus e revisão

`context/INDICE.md` e `context/manifesto-captura.json` descrevem o snapshot oficial de 01/10/2026, remissões e hashes. Os anexos normativos são cópias verbatim. Unicode NFD da fonte foi preservado; normalize para NFC em memória ao buscar texto acentuado. Captura não certifica atualização posterior nem aplicabilidade ao caso.

✅ CPC 305 e Lei 13.140 arts. 16–17 presentes; 🟡 CPC 306–310, remissões processuais e interpretação pendentes. 🔴 Tensão 161 §1º × 163 §1º: não computar espécie trabalhista no denominador de extensão sem negociação coletiva comprovada e enquadramento validado. Incisos revogados não voltam a ser vigentes por remissão.

Toda futura skill de mérito deverá encerrar com `anti-alucinacao-recuperacao-extrajudicial`, `validador-recuperacao-extrajudicial` e `suprema-corte-recuperacao-extrajudicial`, com revisão R1→R4. Esta exigência é orientação para o build (guidance only), ainda sem enforcement operacional.

## Sigilo e estado

Dados profissionais e casos devem permanecer em workspace privado por matéria, fora do source e do corpus. Minutas exigem revisão humana; nenhum envio, assinatura, negociação ou protocolo externo é realizado automaticamente. A licença está em `LICENCA`. Este repositório é local e não possui remote.
