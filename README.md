# Barbearia Alvorada — Site Institucional

Página inicial responsiva da **Barbearia Alvorada**, em arquivo único (`index.html`), sem build e sem dependências além das fontes do Google e das fotos externas.

- **Site no ar:** https://ddesites.github.io/barbearia-alvorada/
- **Repositório:** https://github.com/DDESites/barbearia-alvorada
- **Arquivo publicado:** `index.html` (raiz do repositório)

---

## 1. Status atual

| Item | Situação |
|---|---|
| Publicação no GitHub Pages | ✅ Ativa (branch `main`, raiz) |
| Layout responsivo (360 → 1440 px) | ✅ Sem overflow horizontal |
| Lighthouse — Acessibilidade | ✅ 100 |
| Lighthouse — Boas práticas | ✅ 100 |
| Lighthouse — SEO | ✅ 100 |
| WhatsApp com mensagem de agendamento | ✅ Link pronto, **falta o número** |
| Endereço, horários, telefone | ⏳ Placeholders — aguardando confirmação |
| Preços dos serviços | ⏳ Não exibidos — aguardando confirmação |
| Nomes/cargos da equipe | ⏳ Rótulos provisórios — aguardando confirmação |
| Fotos do acervo | ⏳ Ilustrativas (Unsplash) — trocar por fotos reais |

---

## 2. Seções da página

1. **Início (hero)** — headline, CTA de agendamento e selo "desde 2020".
2. **Faixa de confiança** — mensagens de marca em dourado.
3. **Serviços** — Corte · Barba · Corte + barba · Acabamento.
4. **A barbearia** — história, foto de apoio e números da marca.
5. **Equipe** — 3 cards com retrato (nomes provisórios).
6. **Galeria** — 4 fotos do ambiente e dos cortes.
7. **Citação de marca** — faixa dourada com o slogan.
8. **Contato** — endereço/horários (placeholders) + cartão do WhatsApp.
9. **CTA fixo no celular** — barra inferior com botão de agendamento.

---

## 3. Direção visual

| Elemento | Valor |
|---|---|
| Grafite (base escura) | `#23262d` / `#30333c` |
| Dourado (marca) | `#d9a52e` |
| Creme (fundo claro) | `#f4f1ea` / `#e8e4da` |
| Tipografia títulos | Barlow Condensed (500–800) |
| Tipografia textos | DM Sans (400–700) |

**Breakpoints:** `1440+` (4 colunas de serviço) · `≤850 px` (hero em pilha, serviços em 2 colunas, nav reduzida) · `≤600 px` (equipe 2×1, galeria 2×2, CTA fixo no rodapé).

---

## 4. Pendências — dados a confirmar

Antes de considerar o site finalizado, preencher:

- [ ] **WhatsApp:** número completo com DDI + DDD. Hoje o link é `wa.me/?text=...` **sem destinatário** (abre o app, mas não seleciona o contato).
- [ ] **Endereço** completo (rua, número, bairro, cidade/UF, CEP) + link do Google Maps.
- [ ] **Horários de funcionamento** (dias e intervalos, inclusive sábado).
- [ ] **Telefone fixo**, se houver.
- [ ] **Preços** de cada serviço — ou confirmar a redação "consulte valores".
- [ ] **Nomes e cargos** da equipe (3 profissionais) e fotos reais.
- [ ] Confirmar o ano **"Desde 2020"** usado em textos e selo.
- [ ] Fotos reais da barbearia no lugar das imagens ilustrativas.

### Onde estão os placeholders (busca no `index.html`)

| Conteúdo | Trecho a buscar |
|---|---|
| Endereço | `Consulte nosso endereço` |
| Horários | `Consulte nossos horários` |
| Telefone | `Telefone e endereço podem ser adicionados aqui.` |
| WhatsApp | `https://wa.me/?text=` (inserir `55DDDNUMERO?text=`) |
| Equipe | `Nosso time` · `Atendimento próximo` · `Qualidade em cada corte` |
| Serviços | `<article class="service">` (inserir preço em cada um) |

---

## 5. Como atualizar e publicar

```powershell
# 1. edite o index.html
# 2. suba as mudanças
git add index.html
git commit -m "Atualiza horários e preços"
git push
```

O GitHub Pages reconstrói sozinho em ~1 minuto. A URL não muda.

> A edição local fica em:
> `C:\Users\Bruno\Documents\Codex\2026-10-09\es\outputs\index.html`

---

## 6. Próximos passos (sugestão)

1. Confirmar os dados da seção 4 e publicar em um único push.
2. Trocar as fotos do Unsplash por imagens locais (`/img/`), otimizadas em WebP.
3. Adicionar **JSON-LD `BarberShop`** com endereço, telefone, horários e preço — melhora o SEO local (aparece no Google Maps/busca).
4. Apontar **domínio próprio** (ex.: `barbeariaalvorada.com.br`) nas configurações do Pages.
5. Publicar o link no Instagram/Google Meu Negócio com UTM para rastrear cliques.

---

*Documento de roteiro do projeto — atualize este README conforme os dados forem confirmados.*
