
---

### **Descrição do Repositório (Português)**  
Repositório contendo capturas de tela compactadas (`tar.gz`) com registros de atividades acadêmicas, profissionais e de pesquisa realizadas nos últimos 5 anos. Inclui:  
- Convites para comentar artigos de Data Science no LinkedIn.  
- Histórico de pesquisas no Google sobre TI e programação.  
- Comprovação de conclusão de quizzes e rankings no **Mimo** e **Aprovado APP**.  
- Estudos interdisciplinares aplicando Data Science em biomedicina, fitoterapia (ervas como vassourinha, quebra-pedra, boldo, babosa etc.) e medicina tradicional.  

Dados organizados para análise de evolução técnica e científica.

---

### **Repository Description (English)**  
Repository containing compressed screenshots (`tar.gz`) documenting academic, professional, and research activities over the last 5 years. Includes:  
- Invitations to comment on Data Science articles on LinkedIn.  
- Google search history related to IT and programming.  
- Proof of completion for quizzes and leaderboards on **Mimo** and **Aprovado APP**.  
- Interdisciplinary studies applying Data Science to biomedicine, herbalism (e.g., verbena, mint, insulin plant, ginger), and traditional medicine.  

Organized for tracking technical and scientific progress.

---

### **README.md (English/Português)**  

```markdown
# Activity Mapping & Research Archive (2019–2024)

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

## Contents
- **`screenshots/`**: Compressed (`tar.gz`) screenshots of:
  - LinkedIn engagements (Data Science articles).
  - Google search history (IT/programming topics).
  - Course completions (Mimo, Aprovado APP quizzes/podiums).
- **`biological_studies/`**: Research notes on herbal medicine (e.g., quebra-pedra, boldo, babosa) and Data Science applications in health.
- **`stats/`**: Course performance metrics.

## Usage
```bash
tar -xzvf screenshots.tar.gz  # Extract screenshots
```

## Research Focus
- **Data Science in Traditional Medicine**: Analysis of herbs (e.g., *Plectranthus barbatus*, *Baccharis trimera*) for biomedical applications.
- **Skill Tracking**: Evolution in programming/IT via quantified learning history.

---

# Mapeamento de Atividades & Arquivo de Pesquisa (2019–2024)

[![Licença: MIT](https://img.shields.io/badge/Licença-MIT-blue.svg)](LICENSE)

## Conteúdo
- **`capturas/`**: Compactadas (`tar.gz`) com:
  - Interações no LinkedIn (artigos de Data Science).
  - Histórico de pesquisas no Google (TI/programação).
  - Completude de cursos (quizzes/pódios no Mimo e Aprovado APP).
- **`estudos_biologicos/`**: Notas de pesquisa em fitoterapia (ex.: quebra-pedra, boldo, babosa) e ciência de dados aplicada à saúde.
- **`estatisticas/`**: Métricas de desempenho em cursos.

## Uso
```bash
tar -xzvf capturas.tar.gz  # Extrair arquivos
```

## Foco da Pesquisa
- **Ciência de Dados na Medicina Tradicional**: Análise de ervas (ex.: *insulina vegetal*, *capim-limão*) para aplicações biomédicas.
- **Evolução Técnica**: Rastreamento de habilidades em programação/TI via histórico de aprendizado.
```

---

### **Notas Adicionais**  

Aqui estão as **notas adicionais** sobre como esse repositório pode ser usado para **mapeamento de atividades**, **registro de pesquisas** e **análise de produtividade**, além de sugestões para otimizar o processo:

---

### **Notas Adicionais: Aplicações e Métodos**  

#### **1. Mapeamento de Atividades**  
- **Linha do Tempo Visual**:  
  - Use scripts (ex.: Python + `matplotlib`) para gerar gráficos de atividades por ano/mês a partir dos metadados das capturas (datas de arquivos).  
  - Exemplo:  
    ```python
    import os
    from datetime import datetime
    import matplotlib.pyplot as plt

    files = os.listdir("screenshots/")
    dates = [datetime.fromtimestamp(os.path.getctime(f)) for f in files]
    plt.hist(dates, bins=12)  # Atividades por mês
    ```
- **Categorização**:  
  - Tags em arquivos (ex.: `#linkedin`, `#curso`, `#pesquisa_google`) para filtrar por tipo de atividade.  

#### **2. Registro do Cotidiano de Pesquisas**  
- **Análise de Tópicos Dominantes**:  
  - Extraia termos frequentes do histórico do Google (ex.: com `grep` ou NLP simples) para identificar fases de estudo (ex.: "Python OOP" em 2021, "Vitamina K" em 2023).  
- **Correlação com Eventos**:  
  - Relacione picos de pesquisas com marcos profissionais (ex.: aumento em "SQL" antes de uma entrevista).  

#### **3. Estudos Interdisciplinares (Saúde/Data Science)**  
- **Banco de Dados de Ervas**:  
  - Estruture notas em Markdown ou CSV com campos:  
    ```markdown
    | Nome       | Efeito Medicinal       | Estudo Associado          |
    |------------|------------------------|---------------------------|
    | Quebra-Pedra | Diurético             | [https://bit.ly/4hO5qZG] |        |
    ```
  - Use scripts para cruzar dados com artigos salvos (ex.: `pandas` para análise de frequência de termos).  

#### **4. Acompanhamento de Cursos**  
- **Dashboard de Progresso**:  
  - Crie um `progress.md` com:  
    ```markdown
    ## Mimo (2023)  
    - ✅ Python Basics (100%)  
    - 🟡 SQL (70%)  
    ```  
  - Automatize atualizações via API do Mimo (se disponível).  

#### **5. Privacidade e Eficiência**  
- **Ofuscação**:  
  - Use `sed` ou ferramentas como `gimp` para borrar e-mails/nomes em capturas:  
    ```bash
    gimp -i -b '(batch-blur "screenshot.png")'  # Exemplo simplificado
    ```  
- **Compressão Automatizada**:  
  - Script para compactar mensalmente:  
    ```bash
    tar -czvf pesquisas_$(date +%m-%Y).tar.gz /pasta_capturas/
    ```  

---

### **Como Isso Ajuda?**  
- **Autoconhecimento**:  
  - Padrões de estudo (ex.: "quanto tempo levo para dominar um tópico?").  
- **Portfólio Dinâmico**:  
  - Evidências concretas de evolução técnica e científica.  
- **Tomada de Decisão**:  
  - Identifique gaps (ex.: "foco em Python em 2022, mas falta de Cloud").  

---

### **Exemplo de Estrutura de Diretórios Que Pode Ser Utilizada**  
```plaintext
/repo  
├── /screenshots  
│   ├── linkedin_2022.tar.gz  
│   ├── google_searches_2023.tar.gz  
├── /biological_studies  
│   ├── herbal_effects.csv  
│   ├── vitamin_k_research.md  
├── /scripts  
│   ├── plot_activity.py  
│   ├── compress_monthly.sh  
└── README.md  
```

--- 

### **Ferramentas Recomendadas**  
- **Automação**: `cron` (agendamento), `jq` (processar JSON de APIs).  
- **Visualização**: `Obsidian` (para notas interligadas), `Gephi` (redes de tópicos).  

Essas práticas transformam o repositório em um **"diário técnico-científico"** com utilidade prática além do armazenamento.
