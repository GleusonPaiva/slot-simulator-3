# 🐉 Dragon's Fortune — Slot Math Simulator 3

Simulador matemático completo de slot machine com **modo bônus**, **Free Spins com multiplicadores progressivos** e **Jackpot de 4 níveis**.

Projeto 3 de 5 do portfólio de **Game Math Design** para o mercado de iGaming.

---

## 📊 Resultados

| Componente | RTP | % do Total |
|---|---|---|
| Jogo Base | 36.73% | 92.3% |
| Bônus (Free Spins) | 0.24% | 0.6% |
| Jackpot Progressivo | 2.82% | 7.1% |
| **RTP Total** | **39.79%** | **100%** |

> **RTP (Return to Player)** = percentual do dinheiro apostado que retorna ao jogador a longo prazo. Ex: RTP de 96% significa que a cada R$100 apostados, R$96 retornam em prêmios.

---

## 🎯 O que este projeto demonstra

- **Wild** — símbolo coringa que substitui qualquer outro na linha de pagamento
- **Scatter** — símbolo especial que aciona o modo bônus independente da posição
- **Free Spins** — rodadas grátis com multiplicadores de 2x a 10x
- **Jackpot Progressivo** — 4 níveis (Mini, Minor, Major, Grand) alimentados por % das apostas
- **RTP Breakdown** — separação do RTP por componente (padrão de certificação GLI/eCOGRA)
- **Simulação Monte Carlo** — validação com 5 milhões de rodadas

---

## 🎰 Glossário de termos

| Termo | Significado |
|---|---|
| **RTP** | Return to Player — % do dinheiro apostado que retorna ao jogador |
| **GGR** | Gross Gaming Revenue — receita bruta do cassino após pagar prêmios |
| **Wild** | Símbolo coringa que substitui qualquer outro símbolo |
| **Scatter** | Símbolo especial que aciona bônus em qualquer posição da grade |
| **Free Spins** | Rodadas grátis concedidas pelo modo bônus |
| **Multiplicador** | Fator que multiplica o prêmio (ex: 5x = prêmio × 5) |
| **Jackpot** | Prêmio máximo do jogo, pode ser fixo ou progressivo |
| **Payline** | Linha de pagamento — padrão de posições que forma combinações vencedoras |
| **Hit Rate** | Frequência de rodadas vencedoras (ex: 10% = 1 em cada 10 rodadas paga algo) |
| **Volatilidade** | Risco do jogo — alta = paga raramente mas muito / baixa = paga sempre mas pouco |

---

## 🏆 Jackpot Progressivo

| Nível | Probabilidade | Valor Inicial | Hits em 5M rodadas |
|---|---|---|---|
| Mini | 0.5000% | 10 créditos | 24.941 |
| Minor | 0.1000% | 50 créditos | 4.924 |
| Major | 0.0200% | 200 créditos | 963 |
| Grand | 0.0050% | 1.000 créditos | 224 |

> 1% de cada aposta é contribuído ao pool de jackpot, dividido entre os 4 níveis.

---

## 🎁 Modo Bônus — Free Spins

```
Ativação: 3 ou mais Scatters em qualquer posição
├─ 3 Scatters = 10 Free Spins
├─ 4 Scatters = 15 Free Spins
└─ 5 Scatters = 25 Free Spins

Durante os Free Spins:
├─ 20% de chance de aumentar o multiplicador a cada spin
├─ Multiplicadores disponíveis: 2x, 3x, 4x, 5x, 6x, 8x, 10x
└─ 5% de chance de reativar o bônus (retrigger)

Frequência de ativação: 0.026% (1 em cada ~3.836 rodadas)
```

---

## 🗂️ Estrutura do projeto

```
slot-simulator-3/
├── slot_simulator_3.py                  # Código principal
├── Dragons_Fortune_Math_Document.xlsx   # Game Math Document completo
├── Dragons_Fortune_Report.pdf           # Relatório técnico de certificação
└── README.md
```

---

## 🚀 Como rodar

```bash
pip install numpy pandas matplotlib openpyxl reportlab
python slot_simulator_3.py
```

---

## 📚 Conceitos aplicados

- **Wild e Scatter** — símbolos especiais padrão da indústria
- **Free Spins com multiplicadores** — feature mais popular dos slots modernos
- **Jackpot Progressivo** — modelo de 4 níveis padrão do mercado
- **RTP Breakdown** — separação por componente exigida na certificação
- **Monte Carlo** — validação estatística com 5 milhões de rodadas

---

## 🛠️ Tecnologias

![Python](https://img.shields.io/badge/Python-3.12-blue)
![NumPy](https://img.shields.io/badge/NumPy-latest-blue)
![Pandas](https://img.shields.io/badge/Pandas-latest-blue)
![Matplotlib](https://img.shields.io/badge/Matplotlib-latest-blue)

---

## 👨‍💻 Autor

**Gleuson Paiva**
Desenvolvedor Python | Automação com IA | Game Math Designer em formação

[![GitHub](https://img.shields.io/badge/GitHub-GleusonPaiva-black)](https://github.com/GleusonPaiva)

---

## 📌 Série de projetos

- [x] Projeto 1 — Slot básico com RTP teórico e Monte Carlo
- [x] Projeto 2 — 10 linhas de pagamento e análise de volatilidade
- [x] Projeto 3 — Modo bônus com Free Spins e Jackpot Progressivo
- [ ] Projeto 4 — Comparador de math models com relatório via IA
- [ ] Projeto 5 — Jogo completo com interface visual
