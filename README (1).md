# Despesas Eletricidade e Água — Casa

Aplicação web (ficheiro único HTML) para dividir as despesas de eletricidade e água entre duas frações de uma casa com contador único, a partir das leituras individuais de cada fração.

## Como usar

1. Abre o `index.html` num browser, ou instala a app no telemóvel (ver secção abaixo).
2. No separador **Inquilinos**, confirma os nomes das frações (por defeito "T2" e "T3 Casal dos Cortezes nº51") e adiciona o nome e contacto (WhatsApp) de cada inquilino.
3. No separador **Calculadora**:
   - Introduz o mês da leitura e o mês a que a fatura se refere (a água tem, por norma, um atraso de faturação em relação à eletricidade).
   - Introduz as leituras atuais do contador de cada fração e o preço da fatura.
   - A percentagem de consumo de cada fração é calculada automaticamente a partir da diferença entre a leitura atual e a leitura do mês anterior.
4. Guarda o registo do mês — fica no **Histórico**, consultável e editável a qualquer momento.
5. Usa os botões de WhatsApp para enviar a cada inquilino o valor a pagar, ou copia o resumo para colar num Google Docs.

## Dados

Todos os dados (inquilinos, leituras, histórico) ficam guardados localmente no browser/dispositivo onde a app for usada — não há servidor nem base de dados externa. Se instalares em mais do que um telemóvel, cada um tem os seus próprios dados.

## Ficheiros

- `index.html` — a aplicação
- `manifest.json` — permite instalar a app como ícone no telemóvel
- `service-worker.js` — permite abrir a app mesmo sem internet
- `icon-192.png` / `icon-512.png` — ícone da app

## Instalar no telemóvel

Isto **só funciona depois de a pasta estar publicada num link real** (ex: GitHub Pages) — não funciona a abrir o ficheiro diretamente do telemóvel.

**Android (Chrome):**
1. Abre o link do GitHub Pages.
2. Toca no menu (⋮) > "Adicionar ao ecrã principal" ou "Instalar app".

**iPhone (Safari):**
1. Abre o link do GitHub Pages.
2. Toca no botão Partilhar (□↑) > "Adicionar ao Ecrã Principal".

Depois de instalada, a app abre em ecrã inteiro com o seu próprio ícone, como uma app normal, e continua a funcionar mesmo sem ligação à internet.
