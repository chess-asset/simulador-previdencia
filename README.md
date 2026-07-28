# Simulador do Colaborador — Plano de Previdência

Página estática de página única (sem dependências, sem build) publicada via GitHub Pages.
Mostra, para um colaborador, quanto o plano de previdência instituído pela empregadora
pode acumular até a aposentadoria, e compara com o mesmo valor aplicado num fundo comum
sujeito ao come-cotas.

**Valores ilustrativos. Não é oferta de plano de previdência.**

## Manutenção

A fonte de verdade é `simulador/simulador_colaborador.html` no repositório interno do caso
`prev_corp_btg`. O motor de cálculo em JavaScript é uma porta 1:1 do motor em Python
(`comparativo_ir.py` e `engine.py`), com paridade verificada ao centavo por
`verificar_paridade.js` / `verificar_paridade.py`.

Para atualizar: copiar o HTML sobre `index.html`, commitar e dar push. A URL não muda —
o QR Code impresso continua válido.

O botão "Quero aderir" está desativado enquanto a constante `FORM_URL`, no topo do bloco
`<script>`, estiver vazia. Basta preenchê-la com a URL do formulário.
