# Projeto de Imersão de IA (Alura e Google) #

## Resumo do Projeto ##
O projeto nesse repositório usa o modelo multimodal do Gemini. Se propõe a identificar palavras chaves relacionadas a Tecnologia da Informação
contidas em arquivos PDF de editais de Concursos Publicos. Obtidas essas palavras chave é verificada se as mesmas estão contidas em sites que ofertam cursos e capacitações nessas tecnologias.    

## Roteiro de Implementação ##

1. Carga do PDF do Edital no Google AI Studio
Carregar o arquivo `Edital_SEPLAG.pdf` pela interface do **GOOGLE AI Studio**.

2. Executar o seguinte prompt:
```
Reporte o conteúdo do Edital relacionado ao Cargo 3 de Tecnologia da Informação. Escreva usando a Língua Portuguesa. 
```
3. Executar o seguinte prompt:
```
Identifique no Edital palavras chave  relacionadas a Tecnologia da Informação. Crie uma lista usando o formato JSON.
```

Resultado:
```
[
  {
    "area": "Legislação",
    "palavras-chave": ["LGPD", "Proteção de Dados"]
  },
  {
    "area": "Análise, Desenho e Automação de Processos",
    "palavras-chave": ["BPM", "Business Process Management", "RPA", "Robotic Process Automation", "Mapeamento de Processos", "Análise de Processos", "Modelagem de Processos", "BPMN"]
  },
  {
    "area": "Arquitetura de Desenvolvimento de Software",
    "palavras-chave": ["Desenvolvimento Web", "JavaScript", "HTML5", "CSS3", "WebSocket", "SPA", "Single Page Application", "AngularJS", "DHTML", "AJAX", "Jasper", "Desenvolvimento Mobile", "Apache CXF", "Java", "C#", "Python", "Usabilidade", "Acessibilidade", "W3C", "e-MAG", "Análise Estática de Código", "Clean Code", "Padrões de Projeto", "GoF", "GRASP", "Internet", "Extranet", "Intranet", "Portal", "XML", "XSLT", "UDDI", "WSDL", "SOAP", "REST", "JSON", "Engenharia de Software", "Requisitos Funcionais", "Requisitos Não Funcionais", "Análise de Sistemas", "Qualidade de Software", "Unified Process", "UP", "UML", "Métrica de Ponto de Função", "Testes de Software", "Teste Unitário", "Teste de Integração", "Teste de Carga", "Teste de Estresse", "SonarQube", "Robot Framework", "JMeter", "Frontend", "Backend", "Hibernate", ".NET Core", "Quarkus", "SpringBoot", "Flask", "Django", "NodeJS", "Express", "NestJS", "JEE", "JPA", "EJB", "JSF", "JMS", "JTA", "JVM"]
  },
  {
    "area": "DevOps",
    "palavras-chave": ["Gestão de Configuração", "DevOps", "Versionamento", "Merge", "Branch", "Pipeline", "CI/CD", "Continuous Integration", "Continuous Delivery", "MASA", "Mesh App and Service Architecture", "Containers", "Docker", "Kubernetes"]
  },
  {
    "area": "Gestão de Produto",
    "palavras-chave": ["Qualidade de Software", "MPSBR", "CMMI"]
  },
  {
    "area": "Big Data & Analytics, Business Intelligence, Inteligência Artificial, Internet das Coisas e Nuvem Computacional",
    "palavras-chave": ["Dado", "Informação", "Conhecimento", "Inteligência", "Dados Estruturados", "Dados Não Estruturados", "Dados Abertos", "Coleta de Dados", "Tratamento de Dados", "Armazenamento de Dados", "Integração de Dados", "Recuperação de Dados", "Banco de Dados Relacional", "Metadados", "Tabelas", "Visões", "Views", "Índices", "Chaves", "Relacionamentos", "Modelagem Dimensional", "Mineração de Dados", "CRISP-DM", "Pré-processamento de Dados", "Classificação", "Regras de Associação", "Agrupamento", "Clusterização", "Detecção de Anomalias", "Modelagem Preditiva", "Aprendizado de Máquina", "Mineração de Texto", "Big Data", "Dados Semiestruturados", "3 Vs", "Ingestão de Dados", "Processamento de Dados", "Disponibilização de Dados", "Pipeline de Dados", "Processamento Distribuído", "Data Lake", "ETL", "ELT", "Soluções de Big Data", "Apache Hadoop", "HBase", "Kudu", "Sqoop", "Nifi", "Hive", "Impala", "Spark", "Spark Streaming", "SOLR", "Oozie", "Yarn", "Kafka", "Flink", "AirFlow", "Arquiteturas de Big Data", "Arquitetura Lambda", "Arquitetura Kappa", "Cloud Computing", "AWS", "Azure", "Visualização de Dados", "Análise Exploratória de Dados", "Planilhas", "SQL", "Business Intelligence", "BI", "Sistemas de Suporte a Decisão", "Gestão de Conteúdo", "Data Warehouse", "Data Mining", "OLAP", "Banco de Dados NoSQL", "Dashboards", "Power BI", "Google Looker", "Pentaho", "Storytelling", "Relatórios Analíticos", "Inteligência Artificial", "Naive Bayes", "Regressão Logística", "Redes Neurais", "Funções de Ativação", "Perceptron", "Árvores de Decisão", "ID3", "C4.5", "Florestas Aleatórias", "Random Forest", "SVM", "Support Vector Machines", "KNN", "K-nearest neighbors", "Comitês de Classificadores", "Métricas de Avaliação", "Matriz de Confusão", "Acurácia", "Precisão", "Revocação", "F1-score", "Curva ROC", "Regressão Linear", "Séries Temporais", "Intervalos de Confiança", "MAE", "MSE", "RMSE", "R2", "Agrupamento por Partição", "Agrupamento por Densidade", "Agrupamento Hierárquico", "Redução de Dimensionalidade", "Seleção de Características", "Feature Selection", "PCA", "Principal Component Analysis", "Descoberta de Conjuntos Frequentes", "Descoberta de Regras de Associação", "Sistemas de Recomendação", "Processamento de Linguagem Natural", "PLN", "Normalização Textual", "Stop Words", "Esteemização", "Lematização", "Análise de Frequência de Termos", "POS-tagging", "Part-of-Speech Tagging", "NER", "Named Entity Recognition", "Rotulação IOB", "N-gramas", "Modelos Vetoriais de Palavras", "CBOW", "Skip-Gram", "GloVe", "Modelos Vetoriais de Documentos", "TF", "TF-IDF", "Paragraph Vector", "Métricas de Similaridade Textual", "Similaridade do Cosseno", "Distância Euclidiana", "Similaridade de Jaccard", "Distância de Manhattan", "Coeficiente de Dice", "Sumarização Automática de Texto", "Modelagem de Tópicos", "Classificação de Texto", "Agrupamento de Texto", "Tradução Automática", "Análise de Sentimentos", "Reconhecimento de Voz", "STT", "Speech to Text", "Internet das Coisas", "IoT", "Internet of Things", "Nuvem Computacional", "Arquitetura em Nuvem", "Desenvolvimento em Nuvem"]
  },
  {
    "area": "Segurança da Informação, Segurança de Datacenter, Segurança de Dispositivos, Disponibilidade", 
    "palavras-chave": ["Confiabilidade", "Integridade", "Disponibilidade", "Criptografia", "Assinatura Digital", "Controle de Acesso", "Certificação Digital", "Infraestrutura de Chaves Públicas", "Ataques a Sistemas de Criptografia", "Gerência de Riscos", "Ameaça", "Vulnerabilidade", "Impacto", "Políticas de Segurança", "NBR ISO/IEC 27002:2005", "NBR ISO/IEC 27001:2013", "NBR ISO/IEC 15408", "Políticas de Senhas", "Autenticação de Dois Fatores", "MFA", "OAuth 2", "JWT", "SSO", "SAML", "OWASP Top 10", "SQL Injection", "XSS", "CSRF", "Ataques de Inclusão de Arquivos"]
  }, 
  {
    "area": "Sistemas Distribuídos", 
    "palavras-chave": ["Arquitetura de Sistemas Distribuídos", "Balanceamento de Carga", "Failover", "Replicação de Estado", "Tuning", "Otimização de Consultas", "Segurança de Banco de Dados", "Middleware", "APS", "Application Platform Suite", "Interoperabilidade de Sistemas", "ePING"]
  }
]
```

## Fontes Acessadas ##
