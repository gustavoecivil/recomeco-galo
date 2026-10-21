# GNV Intelligence Lab — Outubro de 2026

Protótipo interativo de CRM & Analytics, criado como estudo independente de Gustavo Santos para demonstração de capacidade analítica e preparação para entrevista. **Não é um produto oficial do Galo.**

## Abrir e apresentar
- Abra `index.html` em um navegador moderno. Funciona completamente offline.
- Para disponibilizar em Netlify, abra o painel do seu Netlify e crie **um site novo e separado** (não substitua `gustavosantos.net.br`); arraste a pasta `GNV_Intelligence_Lab` ou o ZIP extraído.
- Navegue pelas seis áreas do painel. Ações são simuladas, sem enviar mensagens e sem acessar plataformas de terceiros.
- Na seção CRM, exporte os 2.400 registros **sintéticos** em CSV.
- A seção Laboratório permite mudar hipóteses de campanha e calcular um ROI **hipotético**, não real.

## Separação de dados

### Dados públicos / oficiais
- 11/08/2026: Galo na Veia atingiu 200 mil associados. https://atletico.com.br/galo-na-veia-alcanca-marca-historica-de-200-mil-socios/
- 30/08/2026: ultrapassou 235 mil associados. https://atletico.com.br/galo-na-veia-chega-a-235-mil-socios/
- 15/10/2026: atingiu 300 mil associados. https://atletico.com.br/galo-na-veia-alcanca-marca-historica-de-300-mil-socios/
- 21/09/2026: anúncio do GaloLake (>550 tabelas, aproximadamente 1,8 bilhão de registros). Na partida de 19/09/2026, 11.257 torcedores estrearam na Arena MRV. https://atletico.com.br/galo-utiliza-dados-para-entender-comportamento-do-torcedor/
- 10/06/2024: GNV da Massa lançado como modalidade gratuita. https://atletico.com.br/chegou-o-gnv-da-massa/
- 10/10/2025: clube relata 839 torcedores do GNV da Massa estreantes em uma partida específica. https://atletico.com.br/promocao-na-arena-mrv-impulsiona-o-gnv-da-massa/
- Requisitos da vaga: https://galo.gupy.io/jobs/12731122

### Dados de simulação / hipóteses
- 2.400 perfis totalmente fictícios, sem nomes, e-mails, telefones nem CPFs.
- Distribuição dos planos, opt-in, região, score, frequência e inatividade **inventados para testar o modelo**, não representativos.
- Funil de 10.000 sessões e suas taxas **fictícias**.
- Premissas de custo, conversão, receita, ROI, abandono e aumento de conversão **editáveis** e **hipotéticas**.
- A divisão de 300 mil associados entre planos e receitas não é pública neste estudo; não é estimada.

## Arquitetura
Uma única página `index.html`: HTML, CSS, JavaScript e SVG, sem bibliotecas, CDN, banco de dados ou API. Dados sintéticos gerados com PRNG determinístico a cada abertura. Zero tracking, cookies ou envios. Testes podem ser executados offline.

## Segurança, privacidade e integridade
- Nenhum uso de dados reais da Gupy, GaloID ou GaloLake.
- Não importa login do torcedor nem dados sensíveis.
- Exportação apenas dos registros fictícios gerados no navegador.
- Uso demonstrativo, não validado pelo clube; não sugerir afiliação ou endosso.
- Para um projeto real: validar base legal e preferências de contato, limites de finalidade, governança, retenção, controle A/B e acesso restrito.