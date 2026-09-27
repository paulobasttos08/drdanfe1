# 🧾 Dr.Danfe

> Plataforma fiscal brasileira — consulta NF-e, CNPJ, geração de DANFE e ferramentas XML.

[![Status](https://img.shields.io/badge/status-em%20desenvolvimento-yellow)](https://drdanfe.com.br)
[![Licença](https://img.shields.io/badge/licen%C3%A7a-MIT-blue)](LICENSE)
[![HTML](https://img.shields.io/badge/frontend-HTML%20%2F%20JS%20puro-orange)](https://drdanfe.com.br)

---

## 🚀 O que é o Dr.Danfe

O **Dr.Danfe** é uma plataforma gratuita de ferramentas fiscais para contadores, empresas e desenvolvedores brasileiros. Todas as funcionalidades rodam **100% no navegador** — nenhum arquivo é enviado para servidores externos.

---

## ✨ Funcionalidades

| Ferramenta | Descrição |
|---|---|
| 🔍 **Consulta CNPJ** | Dados cadastrais da Receita Federal via BrasilAPI — situação, sócios, atividades, filiais e inscrição estadual |
| 📄 **Consulta NF-e** | Consulta por chave de acesso (44 dígitos) ou upload de XML — exibe emitente, destinatário, itens, impostos e status |
| 📦 **Lote NF-e** | Consulta até 50 chaves de uma vez com tabela de resultados exportável em CSV e Excel |
| 🖨️ **Geração de DANFE** | Gera DANFE completo, simplificado, etiqueta 100×60mm e cupom varejo 58mm a partir do XML |
| 📊 **XML → Excel** | Converte lote de XMLs de NF-e em planilha .xlsx com abas "Notas" e "Itens" |
| 🕐 **Histórico** | Salva automaticamente as últimas consultas de CNPJ e NF-e no navegador (localStorage) |
| ✅ **Validador XML** | Valida integridade do XML de NF-e — parsing, campos obrigatórios, assinatura digital e protocolo |
| 📁 **FiscalPDF** | Organiza PDFs de NF-e por destinatário (CNPJ), com suporte a OCR para PDFs digitalizados |

---

## 🛠️ Tecnologias

- **Frontend:** HTML5, CSS3, JavaScript puro (sem frameworks)
- **Processamento de PDF:** [PDF.js](https://mozilla.github.io/pdf.js/), [PDF-lib](https://pdf-lib.js.org/), [Tesseract.js](https://tesseract.projectnaptha.com/) (OCR)
- **Geração de planilhas:** [SheetJS (xlsx)](https://sheetjs.com/)
- **APIs públicas:** [BrasilAPI](https://brasilapi.com.br/) (CNPJ e NF-e), [NFe.io](https://nfe.io/) (NF-e)
- **Monetização:** Google AdSense (plano gratuito com anúncios)

---

## ⚡ Como usar

### Opção 1 — GitHub Pages (mais simples)

1. Faça um fork deste repositório
2. Vá em **Settings → Pages**
3. Selecione a branch `main` e a pasta `/ (root)`
4. Acesse `https://seuusuario.github.io/drdanfe`

### Opção 2 — VPS / Servidor próprio

```bash
# Clonar o repositório
git clone https://github.com/seuusuario/drdanfe.git
cd drdanfe

# Servir com qualquer servidor HTTP
npx serve .
# ou
python3 -m http.server 8080
```

### Opção 3 — Acesso direto

Baixe o arquivo `drdanfe-completo.html` e abra direto no navegador — funciona offline para as ferramentas que não dependem de API.

---

## 📂 Estrutura do projeto

```
drdanfe/
├── drdanfe-completo.html   # Aplicação completa (single file)
├── README.md               # Este arquivo
├── LICENSE                 # Licença MIT
└── .gitignore              # Ignora node_modules, .env, etc.
```

---

## 🔒 Privacidade

- **XMLs de NF-e** são processados 100% localmente no navegador — nenhum dado fiscal é enviado a servidores
- **Consultas de CNPJ e NF-e** usam APIs públicas da Receita Federal / SEFAZ via BrasilAPI
- **Histórico de consultas** é salvo apenas no `localStorage` do navegador do usuário

---

## 📋 Roadmap

- [x] Consulta CNPJ com busca de filiais
- [x] Consulta NF-e por chave de acesso
- [x] Upload XML e geração de DANFE
- [x] Consulta em lote (até 50 chaves)
- [x] Conversor XML → Excel
- [x] Histórico de consultas
- [x] Validador de XML NF-e
- [x] FiscalPDF (organização por destinatário)
- [ ] Consulta CT-e (Conhecimento de Transporte)
- [ ] Cálculo de impostos (ICMS, PIS, COFINS)
- [ ] Alertas por WhatsApp / e-mail
- [ ] Plano Pro (histórico na nuvem, sem anúncios)
- [ ] App Mobile (PWA)

---

## 🤝 Contribuições

Contribuições são bem-vindas! Abra uma [issue](https://github.com/seuusuario/drdanfe/issues) para reportar bugs ou sugerir melhorias.

1. Faça um fork
2. Crie uma branch: `git checkout -b feature/nova-funcionalidade`
3. Commit: `git commit -m 'feat: adiciona nova funcionalidade'`
4. Push: `git push origin feature/nova-funcionalidade`
5. Abra um Pull Request

---

## 📄 Licença

Distribuído sob a licença MIT. Veja [`LICENSE`](LICENSE) para mais informações.

---

## 📬 Contato

Site: [drdanfe.com.br](https://drdanfe.com.br)

---

<div align="center">
  <sub>Feito com ❤️ para contadores e empresas brasileiras</sub>
</div>
