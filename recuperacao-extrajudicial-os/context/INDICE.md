# Índice — CRJ · recuperação judicial e extrajudicial

Captura literal em 01/10/2026, exclusivamente de páginas oficiais do Planalto, HTTP 200 em seis fontes. Nenhum agregador ou reescrita do conteúdo legal. Fonte, URL, data, decodificação, SHA-256 do HTML e método constam em cada anexo; `manifesto-captura.json` registra contagens e hashes dos corpos finais.

## Anexos

| Anexo | Artigos distintos / unidade recortada | Caracteres do corpo | Escopo |
| --- | ---: | ---: | --- |
| [lei-11101-compilada-integral.md](lei-11101-compilada-integral.md) | 261 | 237319 | 1–201, com todos os intercalares |
| [lei-11101-disposicoes-comuns.md](lei-11101-disposicoes-comuns.md) | 55 | 57583 | 1–46, com intercalares |
| [lei-11101-recuperacao-judicial.md](lei-11101-recuperacao-judicial.md) | 46 | 52741 | 47–72, com intercalares |
| [lei-11101-convolacao-falencia.md](lei-11101-convolacao-falencia.md) | 12 | 9979 | 73; 74; 75; 76; 77; 78; 79; 80; 81; 82; 82-A; 94 |
| [lei-11101-recuperacao-extrajudicial.md](lei-11101-recuperacao-extrajudicial.md) | 7 | 8077 | 161; 162; 163; 164; 165; 166; 167 |
| [lei-11101-crimes-referencia.md](lei-11101-crimes-referencia.md) | 11 | 5375 | 168; 169; 170; 171; 172; 173; 174; 175; 176; 177; 178 |
| [lei-11101-disposicoes-finais.md](lei-11101-disposicoes-finais.md) | 15 | 8805 | 189; 189-A; 190; 191; 192; 193; 193-A; 194; 195; 196; 197; 198; 199; 200; 201 |
| [lei-14112-transitorias.md](lei-14112-transitorias.md) | 3 | 3025 | 5; 6; 7 |
| [cpc-recuperacao.md](cpc-recuperacao.md) | 5 | 6439 | 139; 300; 305; 313; 1015-pu |
| [ctn-recuperacao.md](ctn-recuperacao.md) | 8 | 3846 | 155-A; 186; 187; 188; 189; 190; 191; 191-A |
| [lei-10522-parcelamento-rj.md](lei-10522-parcelamento-rj.md) | 3 | 21871 | 10-A; 10-B; 10-C |
| [lei-13140-mediacao.md](lei-13140-mediacao.md) | 2 | 659 | 16; 17 |

## Método e limites

Adendo do coordenador recebido em 01/10/2026: acrescentados CPC art. 305 e Lei nº 13.140/2015 arts. 16 e 17, capturados no mesmo padrão literal do briefing.

- `capturar-crj.py` é uma adaptação local do método do playbook `PLAYBOOK/templates/capturar-planalto.py`: o template foi lido, mas não utilizado diretamente porque elimina o conteúdo tachado. O script entregue preserva tachados HTML em `~~texto~~`.
- A fonte principal é `L11101compilado.htm`, já com as alterações da Lei nº 14.112/2020 incorporadas. Não se aplicou manualmente o texto alterador à lei original.
- A cópia `lei-11101-compilada-integral.md` contém o diploma integral, inclusive arts. 83–160, 167-A–167-Y e 179–188, além das assinaturas e da nota do DOU. Ela atende à exigência de integralidade; os seis anexos por bloco mantêm rigorosamente os recortes solicitados e são próprios para consulta dirigida. Não confundir esses recortes com o diploma integral.
- Os intercalares foram preservados: comuns incluem 6-A, 6-B, 6-C, 7-A, 20-A–20-D e 45-A; RJ inclui, entre outros, 69-A–69-L; finais incluem 189-A e 193-A. A cópia integral contém 261 números distintos de artigo, correspondentes a 1–201 e 60 intercalares.
- A página compilada da Lei nº 11.101/2005 não traz texto histórico riscado: traz marcadores literais de revogação. Foram acrescentados tachados aos 26 parágrafos/dispositivos identificados com `(Revogado)`, `(Revogada)` ou `(Revogado pela Lei...)`, sem modificar palavras. Não se tacharam cláusulas de revogação de atos privados ou o art. 200. Redações históricas tachadas na Lei nº 10.522/2002 foram preservadas.
- Entidades HTML decodificadas, espaços e quebras de layout normalizados; remissões e notas legislativas preservadas como texto, inclusive grafias antigas e Unicode decomposto da própria página. Não houve correção editorial nem normalização Unicode.
- O CPC contém integralmente 139, 300, 305 e 313; do art. 1.015, apenas seu parágrafo único, expressamente identificado. O cabeçalho identificador é editorial e não integra o texto da norma.
- As disposições finais incluem 189–201; crimes incluem somente 168–178, como referência, sem análise penal. O anexo da Lei nº 14.112/2020 contém somente 5º–7º. O CTN contém 155-A e 186–191-A. O anexo de parcelamento contém 10-A–10-C integrais, inclusive históricos tachados, sem 10-D.
- Captura de corpus não equivale a auditoria de constitucionalidade, decisões suspensivas, regulamentos fiscais ou de aplicabilidade ao caso concreto. Notas `Vide`, `Vigência` e referências externas foram mantidas; seus destinos não integram esta captura.

## Reprodução e verificação

```sh
python3 context/capturar-crj.py --destino /tmp/crj-recaptura
rg -P '[\x00-\x08\x0B\x0C\x0E-\x1F\x80-\x9F]' context
python3 - <<'PYCODE'
from pathlib import Path
for f in Path('context').iterdir():
    if f.is_file():
        assert '\ufffd' not in f.read_text(encoding='utf-8'), f
print('PASS: UTF-8 estrito e ausência de U+FFFD')
PYCODE
```

A busca `rg` acima deve retornar vazia (exit code 1 significa ausência de correspondências). O script verifica extração independente por remoção de tags/decodificação de entidades contra `HTMLParser` nas seis páginas completas, compara o texto dos corpos antes/depois de inserir tachados e valida os números 1–201 da compilada. Nesta execução, extração independente PASS para as seis fontes e reprodução do mesmo snapshot PASS byte a byte para os 12 anexos. Hashes dos corpos validados contra o manifesto. Fonte pode mudar em nova captura; hashes referem-se ao snapshot de 01/10/2026.

`DONE` é marcador vazio de conclusão da captura desta lane. Não é aprovação jurídica dos plugins.

## Busca no corpus

O original verbatim preserva caracteres NFD da fonte oficial. Para buscas com acentuação, normalize consulta e texto para NFC em memória, sem modificar os anexos nem os hashes do manifesto. Exemplo: `unicodedata.normalize("NFC", texto)`. Apenas os caminhos operacionais deste índice foram adaptados ao diretório local do plugin.


## Conferência de proveniência da cópia local — FRE, 01/10/2026

A hipótese de normalização NFC prévia da cópia local **não se confirmou**: os 12 corpos dos anexos são idênticos byte a byte aos hashes `sha256_corpo` do `manifesto-captura.json`; sete corpos ainda mudam sob NFC (compilada integral, disposições comuns, recuperação judicial, recuperação extrajudicial, crimes, disposições finais e parcelamento). Os outros cinco já estão em NFC. Nenhuma normalização foi aplicada aos anexos nesta correção: preservar o original permite reproduzir os hashes existentes. A equivalência “texto idêntico ao original após NFC” é critério para eventual cópia normalizada, não alegação de transformação histórica comprovada. Se houver essa cópia, registrar separadamente hash original e hash NFC, sem substituir o original ou atribuir seu hash à cópia transformada.

Reprodução local, sem recaptura ou serviço externo:

```sh
python3 - <<'PYCODE'
from pathlib import Path
import hashlib, json, unicodedata
p = Path('context')
m = json.loads((p / 'manifesto-captura.json').read_text())
nao_nfc = []
for anexo in m['anexos']:
    corpo = (p / anexo['arquivo']).read_text().split('\n---\n\n', 1)[1]
    assert hashlib.sha256(corpo.encode()).hexdigest() == anexo['sha256_corpo']
    if corpo != unicodedata.normalize('NFC', corpo):
        nao_nfc.append(anexo['arquivo'])
assert len(nao_nfc) == 7
print('PASS: 12 hashes originais; 7 corpos ainda não NFC', nao_nfc)
PYCODE
```
