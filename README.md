# Mapa de Fretes Brasil

Mapa interativo que exibe os multiplicadores de custo de frete por estado brasileiro para **grandes cargas** (colchões e cama box), com origem em **São Paulo**.

## Sobre o projeto

A ferramenta permite visualizar rapidamente quanto custa transportar uma carga grande para cada estado do Brasil em relação ao custo base de São Paulo (referência = 1,0×). Ao passar o mouse ou clicar em um estado, são exibidos os detalhes do multiplicador e uma estimativa de custo.

### Fonte dos dados

- **ANTT Portaria SROC nº 3/2026** — CCD R$ 6,585/km
- ILOS, GuiadoTRC e pesquisa de mercado 2025–2026
- Âncora de calibração: Uruguaiana (RS) ≈ R$ 500 | São Paulo ≈ R$ 100

## Funcionalidades

- Mapa coroplético colorido por faixa de custo (gradiente de verde a vermelho)
- Painel lateral com detalhes do estado selecionado
- Rankings de estados mais caros e mais baratos
- Indicação de regiões adversas (custo anômalo ou acesso difícil)
- **Mobile**: bottom sheet deslizante — toque em um estado para abrir os detalhes automaticamente

## Tecnologias

- [Leaflet.js](https://leafletjs.com/) — renderização do mapa interativo
- GeoJSON dos estados brasileiros (simplificado)
- HTML, CSS e JavaScript puros — sem dependências de build

## Como usar

Basta abrir o arquivo `index.html` no navegador. Nenhuma instalação ou servidor é necessário.

```bash
# Clone o repositório
git clone https://github.com/B3g4/mapa-fretes.git

# Abra no navegador
cd mapa-fretes
start index.html   # Windows
# ou
open index.html    # macOS
```

## Deploy

O projeto está disponível em produção na Vercel:
**https://mapa-fretes.vercel.app**

Configurado via `vercel.json` para deploy automático.

## Aviso

> Os valores são estimativas calibradas para grandes cargas e podem variar conforme transportadora, volume negociado e sazonalidade. Consulte sempre a transportadora para cotações precisas.

## Licença

MIT
