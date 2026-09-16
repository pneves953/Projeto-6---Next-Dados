# Projeto 6 — Next Carreira em dados

**Como usar:** copie este arquivo para `docs/canvas-projeto.md` no repositório da equipe e preencha durante o E2 (qua 16/09). O canvas é validado pelo mentor ao fim do E2: aprovado, aprovado com ajustes, ou devolvido com pendências claras (pendências resolvidas até o E3). O canvas aprovado fica versionado no repositório — ele é a referência dos checkpoints: as perguntas daqui são as que o CP1 verifica (critério 1.4) e as que a análise e o dashboard precisam responder (critérios 2.1 e 2.2).

Lembre da regra do E2: **não existe viabilidade sem amostra baixada e aberta.**

---

## Identificação

| | |
|---|---|
| **Nome da equipe** | Equipe 6 |
| **Integrantes** | |
| **Mentor** | |
| **Tema** | |
| **Repositório GitHub** | |

---

## 1. Problema de negócio

A Neoenergia Pernambuco realiza a avaliação manualmente de laudos de aferição do medidor de energia apresentando indícios de irregulariedade.

Hoje os laudos de aferição são analisados manualmente. O volume é alto, existe rotatividade na equipe e a classificação pode ser inconsistente. Isso gera atrasos, dificulta a análise de todos os laudos do mês e pode resultar em cobranças equivocadas.

Logo , uma solução de triagem de laudos que automatiza a classificação de indícios e prioriza os casos por impacto, permitindo que os analistas concentrem o esforço nos laudos mais relevantes financeiramente.

---

## 2. Público / decisor

Distribuidora de Energia - Neoenergia

Área: Gestão de perdas

Tomador de decisão: Analista de Perdas


---

## 3. Perguntas analíticas

No mínimo 3, respondíveis com os dados escolhidos. Uma pergunta respondível tem recorte claro (onde, quando, o quê) e o dado necessário existe na fonte. O CP1 verifica que ao menos 3 continuam respondíveis com os dados **reais**.

| # | Pergunta | Que decisão ela informa? | Respondível com os dados? (verificado na amostra) |
|---|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |
| 4 (opcional) | | | |
| 5 (opcional) | | | |

---

## 4. Fontes de dados

Uma linha por fonte. A amostra precisa ter sido **baixada e aberta hoje** — coluna a coluna. Lembrete: se a fonte tiver API, a coleta usa API (requisito do M3). Troca de fonte é livre até o E3 (21/09); depois, só com a coordenação.

| Fonte | Link | Formato | Volume estimado | Licença/acesso | Amostra baixada e aberta? (sim/não) | Colunas-chave confirmadas na amostra |
|---|---|---|---|---|---|---|
|Excel de laudos da prestadora |Não aplicável — fonte fornecida pela |XLSX/Excel |12 meses |Acesso interno |Não — aguardando amostra |A confirmar |
|Base existente da demandante |Não aplicável — fonte fornecida pela |SQL/banco |12 meses |Acesso interno |Não — aguardando amostra|A confirmar |

---

## 5. Escopo e entregáveis — a regra do fatiável

Defina primeiro a fatia mínima: o menor recorte que ainda exercita o ciclo completo (banco → pipeline → análise → dashboard). Ela é o compromisso da equipe. As extensões só entram se a fatia mínima estiver pronta — e nada entra após o congelamento de escopo (05/10).

**Fatia mínima (compromisso):**

```
Triagem de laudos de medidores dos últimos 12 meses, utilizando os campos estruturados disponíveis no Excel, com ingestão e validação dos dados, aplicação de regra de classificação de indício de fraude/defeito e geração de fila priorizada por impacto, com visualização dos principais indicadores do processo.
```

**Extensões desejáveis (apenas se sobrar tempo):**

```
Ampliar a análise para períodos além da amostra inicial de 12 meses.
Evoluir a priorização incorporando outros critérios operacionais definidos pela demandante.
```

**Fora de escopo (o que decidimos NÃO fazer):**

```
Leitura automática do PDF dos laudos.
```

---

## 6. Riscos e mitigação

Ao menos 3 riscos do **seu** projeto (não genéricos). Consulte a tabela de riscos comuns no [`guia-do-projeto.md`](guia-do-projeto.md).

| Risco | Sinal precoce | Mitigação | Responsável por monitorar | Plano B |
|---|---|---|---|---|
|Amostra de 12 meses não ser disponibilizada no prazo | SQL existente não ser disponibilizado ou não representar claramente as regras atuais | Cobrança tempestiva via e-mail para o Victor | Toda a Equipe | Criação de uma população fictícia para criação da ferramenta| 
| Dados pessoais aparecerem na base| Colunas com títulos sujeitivos de informações pessoais| Troca da informação pessoal por um ID ou número de identificação e revisão antes de carregar os dados| Toda a Equipe | - |
| Perfeccionismo no dashboard|Informações demais e não objetivas no dasboard. | Checklist para criação do dashboard| Todo a equipe | - |

---

## 7. Divisão de papéis

Todos codificam — papéis distribuem responsabilidade de acompanhamento, não exclusividade de execução. Cada papel tem uma pessoa sombra (backup). Em equipes de 4, coordenação acumula com outro papel; em equipes de 5–6, dados/pipeline e análise podem ser duplicados.

| Papel | Titular | Sombra |
|---|---|---|
| Coordenação de projeto | | |
| Dados / pipeline | | |
| Análise | | |
| Visualização / pitch | | |

**Canal de comunicação da equipe (fora do horário de aula):**

```
(ex.: grupo no WhatsApp + board no GitHub Projects)
```

---

## Validação do mentor (preenchida pelo mentor no E2)

| | |
|---|---|
| **Status** | ( ) Aprovado ( ) Aprovado com ajustes ( ) Devolvido com pendências |
| **Data** | |
| **Amostra baixada e aberta verificada?** | ( ) Sim ( ) Não |
| **Pendências (com prazo até o E3 — seg 21/09)** | |
