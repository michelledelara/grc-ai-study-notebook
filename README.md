# 📚 Caderno Temático: GRC, Segurança da Informação e IA

> Projeto de estudo e experimentação sobre **Governança, Riscos e Compliance (GRC)**, utilizando Inteligência Artificial como ferramenta de apoio à análise, síntese e consulta de frameworks e documentos técnicos.

## 🎯 Sobre o Projeto

Este projeto foi desenvolvido com o objetivo de explorar conceitos de **Governança, Gestão de Riscos, Compliance e Segurança da Informação**, combinando referências reconhecidas do mercado com o uso de **Inteligência Artificial generativa**.

A proposta foi utilizar o **NotebookLM** para criar uma base de conhecimento fundamentada em documentos oficiais, testar diferentes estratégias de prompting e avaliar como a qualidade das instruções influencia a precisão, profundidade e utilidade das respostas geradas pela IA.

Além do estudo conceitual, o projeto busca demonstrar uma abordagem prática de utilização responsável da IA em contextos relacionados a **GRC, Cybersecurity e Privacidade de Dados**.

---

## 🧩 Problema

Frameworks de segurança, gestão de riscos e documentos regulatórios costumam ser extensos e possuem linguagem técnica.

O desafio deste projeto foi investigar:

**Como utilizar IA generativa para transformar documentos complexos de GRC e Segurança da Informação em conhecimento estruturado, consultável e útil, sem perder a rastreabilidade das fontes?**

---

## 🎯 Objetivos

* Compreender os fundamentos de **Governança, Riscos e Compliance**.
* Analisar a relação entre GRC, Segurança da Informação e Proteção de Dados.
* Explorar o **NIST Cybersecurity Framework 2.0**, o **COSO ERM** e orientações da **ANPD**.
* Utilizar o NotebookLM como ferramenta de análise de documentos.
* Experimentar técnicas de **engenharia de prompts**.
* Identificar limitações e possíveis alucinações de modelos de IA.
* Criar prompts reutilizáveis para estudos, entrevistas e análises futuras.
* Desenvolver uma base de conhecimento que possa evoluir para projetos de **Cyber GRC e Cloud Security**.

---

## 🛠️ Tecnologias e Conceitos Utilizados

* Inteligência Artificial Generativa
* Google NotebookLM
* Prompt Engineering
* GRC
* Cybersecurity
* Gestão de Riscos
* Compliance
* LGPD
* NIST Cybersecurity Framework 2.0
* COSO Enterprise Risk Management
* Análise e validação de fontes

---

## 📂 Curadoria de Fontes

Para alimentar o NotebookLM, foram selecionadas fontes oficiais e reconhecidas na área de governança, riscos, segurança e privacidade.

### 1. NIST Cybersecurity Framework 2.0

Framework para gerenciamento de riscos de segurança cibernética.

O **NIST CSF 2.0** organiza seus resultados de segurança em seis funções:

`GOVERN → IDENTIFY → PROTECT → DETECT → RESPOND → RECOVER`

A inclusão da função **Govern** na versão 2.0 reforça a relação entre segurança cibernética, estratégia organizacional, responsabilidades e gestão de riscos.

---

### 2. Guia Orientativo de Segurança da Informação da ANPD

Material da Autoridade Nacional de Proteção de Dados direcionado principalmente aos **agentes de tratamento de pequeno porte**.

O documento apresenta orientações sobre medidas administrativas e técnicas de segurança da informação relacionadas à proteção de dados pessoais.

---

### 3. COSO ERM — Enterprise Risk Management

Referência para **gestão de riscos corporativos**, com abordagem integrada à estratégia e ao desempenho organizacional.

O COSO ERM ajuda a compreender como os riscos devem ser considerados não apenas como ameaças isoladas, mas como elementos relacionados aos objetivos, decisões e desempenho da organização.

---

## 🔄 Metodologia

O fluxo utilizado neste projeto foi:

```text
Fontes oficiais
      ↓
Curadoria dos documentos
      ↓
NotebookLM
      ↓
Criação e refinamento de prompts
      ↓
Análise das respostas
      ↓
Verificação nas fontes
      ↓
Ajuste dos prompts
      ↓
Construção da base de conhecimento
```

Um princípio orientou todo o experimento:

> **A IA auxilia na análise, mas a fonte original permanece como referência para validação.**

---

# 🧪 Engenharia de Prompts e Troubleshooting

Um dos principais aprendizados do projeto foi perceber que a qualidade da resposta da IA depende diretamente da qualidade do contexto e das instruções fornecidas.

## Tentativa 1 — Prompt Genérico

### Prompt

> "O que é GRC segundo os documentos?"

### Resultado

A resposta apresentou definições corretas, porém excessivamente genéricas e teóricas.

Não houve conexão suficiente entre:

* governança;
* gestão de riscos;
* segurança da informação;
* compliance;
* proteção de dados.

### Aprendizado

Perguntas muito amplas aplicadas a documentos técnicos tendem a produzir respostas igualmente amplas.

**Prompt genérico → resposta genérica.**

---

## Tentativa 2 — Papel + Fontes + Objetivo + Formato

### Prompt

> "Aja como um Diretor de Segurança da Informação (CISO). Com base exclusivamente no NIST CSF 2.0 e no Guia Orientativo de Segurança da Informação da ANPD, crie uma tabela relacionando ações de Governança com requisitos e práticas de Compliance e proteção de dados. Explique como a gestão de riscos conecta esses elementos."

### Resultado

A resposta se tornou:

* mais estruturada;
* mais contextualizada;
* orientada à prática;
* mais adequada ao cenário de Segurança da Informação.

### Estrutura identificada

Um prompt técnico de melhor qualidade pode combinar:

```text
PAPEL
+
CONTEXTO
+
FONTES
+
TAREFA
+
RESTRIÇÕES
+
FORMATO DA RESPOSTA
```

---

## ⚠️ Problema Encontrado — Informação Além das Fontes

Durante alguns testes, o modelo começou a apresentar exemplos que não estavam diretamente fundamentados nos documentos utilizados.

Para reduzir esse comportamento, foi adicionada uma restrição explícita:

> "Baseie sua resposta estritamente nos documentos fornecidos. Quando uma informação não puder ser confirmada pelas fontes, informe que não há evidência suficiente em vez de completar a resposta por inferência."

### Aprendizado

Em aplicações relacionadas a **GRC, Compliance, Segurança e Privacidade**, fluência não significa necessariamente precisão.

Por isso, respostas geradas por IA devem passar por:

* validação;
* verificação da fonte;
* revisão humana;
* análise do contexto.

---

# 📖 Miniguia de GRC

## 🏛️ Governança — A Direção

Governança estabelece **como a organização é dirigida, supervisionada e responsabilizada**.

Envolve elementos como:

* estratégia;
* políticas;
* papéis e responsabilidades;
* tomada de decisão;
* supervisão;
* accountability;
* alinhamento entre tecnologia e objetivos de negócio.

**Analogia:** é o volante que determina para onde a organização pretende ir.

---

## 📡 Riscos — O Radar

Gestão de riscos busca identificar eventos ou condições que possam afetar os objetivos da organização.

O processo normalmente envolve:

1. identificação;
2. análise;
3. avaliação;
4. tratamento;
5. monitoramento.

Exemplos no contexto de segurança:

* vazamento de dados;
* comprometimento de credenciais;
* indisponibilidade de sistemas;
* configuração inadequada de recursos;
* acesso não autorizado.

**Analogia:** é o radar que ajuda a identificar obstáculos antes que eles comprometam o caminho.

---

## ⚖️ Compliance — As Regras

Compliance está relacionado à conformidade da organização com:

* leis;
* regulamentações;
* normas;
* contratos;
* políticas;
* procedimentos internos.

No contexto de proteção de dados no Brasil, a **LGPD** é uma das principais referências regulatórias.

**Analogia:** são as regras que determinam quais limites precisam ser respeitados durante o percurso.

---

# 🔗 Como os três pilares se conectam?

```text
                 GOVERNANÇA
             define direção e
              responsabilidades
                     │
                     ▼
                GESTÃO DE
                  RISCOS
              identifica e
             prioriza ameaças
                     │
                     ▼
                CONTROLES
                     │
                     ▼
                COMPLIANCE
             verifica aderência
          às obrigações aplicáveis
```

Na prática, os três elementos trabalham de forma integrada.

A **Governança** estabelece objetivos e responsabilidades.

A **Gestão de Riscos** identifica o que pode impedir esses objetivos.

Os **controles** são implementados para tratar os riscos.

O **Compliance** auxilia na verificação de que leis, normas, políticas e requisitos aplicáveis estão sendo observados.

---

# 🧠 Glossário

### Risco Inerente

Nível de risco existente **antes da aplicação dos controles** destinados a reduzi-lo.

### Risco Residual

Nível de risco que permanece **após a implementação e consideração da efetividade dos controles**.

### Controle

Medida utilizada para modificar um risco.

Pode envolver processos, políticas, tecnologias ou procedimentos.

### Framework

Estrutura organizada de princípios, práticas ou resultados que auxilia uma organização na implementação e gestão de determinada área.

Exemplos:

* NIST CSF
* COSO ERM
* ISO/IEC 27001

### Mitigação

Estratégia utilizada para reduzir a probabilidade e/ou o impacto associado a determinado risco.

### Auditoria

Processo sistemático de avaliação de evidências para verificar se critérios, requisitos ou controles estão sendo atendidos.

---

# ♻️ Prompts Reutilizáveis

## 🎤 Preparação para entrevistas

> "Atue como entrevistador para uma vaga de Analista de GRC. Utilizando exclusivamente os documentos disponibilizados, faça cinco perguntas técnicas progressivamente mais difíceis. Aguarde minha resposta antes de apresentar a próxima pergunta. Após cada resposta, avalie precisão técnica, clareza e pontos de melhoria."

---

## 🛡️ Aplicação do NIST CSF 2.0

> "Utilizando o NIST Cybersecurity Framework 2.0 como referência, crie um checklist com dez ações para começar a implementar a função IDENTIFY em uma pequena empresa. Para cada ação, indique o objetivo e o risco que ela ajuda a compreender ou gerenciar."

---

## ⚖️ Análise de Compliance

> "Compare os controles ou práticas de segurança identificados nos documentos com as orientações da ANPD. Para cada correspondência, indique a fonte utilizada e sinalize explicitamente quando não houver evidência suficiente para estabelecer uma relação."

---

## 📊 Análise de Riscos

> "A partir do cenário apresentado, identifique os riscos, diferencie risco inerente e risco residual e indique possíveis controles. Não presuma informações que não estejam disponíveis. Liste separadamente as premissas utilizadas."

---

## 🎓 Explicação de conceitos

> "Explique a diferença entre risco inerente e risco residual em três níveis: primeiro para uma pessoa sem conhecimento técnico, depois para um Analista de GRC e, por último, como eu explicaria o conceito em uma entrevista de emprego."

---

# 💡 Principais Aprendizados

Este projeto permitiu observar que o uso de IA em GRC exige mais do que simplesmente fazer perguntas a um modelo.

Os principais aprendizados foram:

* selecionar fontes confiáveis antes de utilizar IA;
* fornecer contexto suficiente ao modelo;
* delimitar claramente a tarefa;
* estabelecer restrições;
* solicitar formatos específicos de resposta;
* separar informações provenientes da fonte de inferências;
* validar conteúdos técnicos;
* documentar erros e ajustes realizados;
* manter revisão humana em decisões relacionadas a risco e compliance.

---

# 🧭 IA Aplicada a GRC

Um possível fluxo de utilização responsável de IA em GRC seria:

```text
Finding / Evidência
        ↓
Identificação do Risco
        ↓
Consulta à Base de Conhecimento
        ↓
Correlação com Frameworks
        ↓
Sugestão da IA
        ↓
Validação Humana
        ↓
Decisão / Tratamento
        ↓
Registro para Auditoria
```

A IA pode apoiar atividades como:

* classificação inicial de riscos;
* correlação entre controles e frameworks;
* síntese de documentos;
* preparação de checklists;
* identificação preliminar de requisitos;
* apoio à documentação;
* preparação para auditorias;
* consulta a bases de conhecimento.

Porém, **decisões de risco e compliance não devem depender exclusivamente da saída de um modelo de IA**.

---

# 🚀 Próximos Passos

Este projeto pode evoluir para aplicações mais práticas de Cyber GRC, incluindo:

* [ ] Criar uma matriz de riscos.
* [ ] Mapear controles entre NIST CSF e LGPD.
* [ ] Criar um exemplo de Risk Register.
* [ ] Adicionar cenários de incidentes de segurança.
* [ ] Relacionar findings técnicos a requisitos de compliance.
* [ ] Criar uma versão estruturada dos findings em JSON.
* [ ] Explorar automação de análise de riscos com IA.
* [ ] Integrar conceitos de Cloud Security e AWS.
* [ ] Criar um protótipo de assistente de GRC baseado em fontes confiáveis.

---

# 🏁 Conclusão

O experimento mostrou que a Inteligência Artificial pode ser uma ferramenta poderosa para apoiar atividades de **Governança, Riscos, Compliance e Segurança da Informação**, especialmente na organização e análise de grandes volumes de documentação.

Ao mesmo tempo, o projeto reforçou um princípio essencial:

> **Em GRC, a IA deve apoiar a decisão — não substituir a análise crítica, a evidência e a validação humana.**

A combinação entre **fontes confiáveis + engenharia de prompts + validação humana + rastreabilidade** é fundamental para utilizar IA de forma responsável em contextos de risco, segurança e compliance.
