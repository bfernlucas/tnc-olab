# Dashboard MEL — TNC · Agricultura Familiar no Pará

Protótipo de painel de monitoramento. Publicar via **GitHub Pages** em Settings → Pages → Branch: main → /(root).

## Conectar à planilha real

Altere `DATA_URL` no script do `index.html`:

**Google Sheets (CSV publicado)**
```
Arquivo > Compartilhar > Publicar na web > Formato: CSV > Copiar URL
```

**SharePoint / OneDrive**
Use a URL de exportação CSV da lista ou planilha.

## Estrutura de dados esperada (JSON ou CSV)

```
con, mel, tra, ater, car, prada, cred, uds, atualizado, quinzena, periodo
```

Exemplo mínimo (JSON):
```json
{
  "atualizado": "15/04/2026",
  "quinzena": "13",
  "periodo": "Abr/2025 – Set/2026",
  "con": 312,
  "mel": 189,
  "tra": 41,
  "ater": 87,
  "car": 23,
  "prada": 19,
  "cred": 18,
  "uds": 6
}
```

## Abas do dashboard

| Aba | Indicadores |
|---|---|
| Visão Geral | KPIs P1 + P2, evolução por quinzena, progresso por eixo |
| Indivíduos · P1 | Funil 1.1→1.3, qualitativo ATER (2.1), por parceiro, regularização |
| Desenv. Territorial · P2 | Crédito (1.7/2.4), UDs (1.8), maturidade (1.9/2.5), governança (1.10/2.6), mercados |
| Resultados CP / MP | KSIs ToC TNC (2.1–2.9), Métricas TNC 2030 (3.1–3.5), Impacto LP (4.1–4.2) |
| Qualidade dos Dados | Registros, validação, lacunas, status de entrega por parceiro, amostragem Olab |
