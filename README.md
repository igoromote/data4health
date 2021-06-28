# Projeto `Perfil dos estabelecimentos passíveis de Licença Sanitária em Manaus a partir da adesão à Rede Nacional para a Simplificação do Registro e da Legalização de Empresas e Negócios (REDESIM).`
# Project `Profile of establishments subject to Sanitary License in Manaus after joining the National Network for the Simplification of Registration and Legalization of Companies and Businesses (REDESIM).`

# Apresentação

O presente projeto foi originado no contexto das atividades da disciplina de pós-graduação [*Ciência e Visualização de Dados em Saúde*](https://github.com/datasci4health/home), oferecida no primeiro semestre de 2021, na Unicamp.

|Nome  | RA | Especialização|
|--|--|--|
| Igor Mateus Omote  | 169819  | Computação|
| Larissa Maria Lago Quintela  | 160343  | Elétrica|
| Marcos Vinicius Soares Silva  | 224692  | Saúde|
| Nádia Maria Soares Bezerra  | 187940  | Saúde|

# Introdução e Referenciais de Teóricos
A Lei Federal Nº 8.080, de 19 de setembro de 1990, também conhecida como Lei Orgânica do SUS1, representa um marco para as condições de promoção, proteção e recuperação da saúde no Brasil. Entre outras providências, a Lei define o Sistema Único de Saúde - SUS e a organização dos serviços correspondentes, entre eles a Vigilância Sanitária (Visa), entendida como um conjunto de ações capaz de eliminar, diminuir ou prevenir riscos à saúde, abrangendo o controle de bens de consumo e da prestação de serviços que se relacionam, direta ou indiretamente, com a saúde. Atualmente, estas ações são executadas pelo Sistema Nacional de Vigilância Sanitária, composto pelos órgãos de Visa local (Visas municipais e estaduais) e pelo órgão federal, a Agência Nacional de Vigilância Sanitária - Anvisa, coordenadora do sistema, conforme definido na Lei Nº9.782, de 26 de janeiro de 19992.

Neste sentido, uma das ações empreendidas pelos órgãos de Visa municipal ou estadual - conforme pactuação bipartite - é a emissão de documentos, denominados Licença ou Alvará Sanitário, que habilitam a operação de atividades específicas que estão sujeitas ao controle sanitário, tais como a fabricação e o comércio de medicamentos, cosméticos, alimentos e a prestação de serviços saúde hospitalares e ambulatoriais. Desta forma, o licenciamento sanitário constitui uma das atribuições do SUS e representa uma importante ação de proteção à saúde da população.

Ao mesmo tempo que visa garantir o cumprimento de requisitos para o funcionamento de estabelecimentos de forma segura e com menor risco sanitário possível, o licenciamento representa um processo burocrático e complexo para ambos os lados: setor regulado e órgãos reguladores. Isso porque não há, no Brasil de modo geral, procedimentos claros e padronizados para a emissão de licenças sanitárias, entre outros fatores.

Com o objetivo de sanar parte desse problema, alguns esforços estão sendo realizados nos últimos anos em nível federal, como a criação da Rede Nacional para a Simplificação do Registro e da Legalização de Empresas e Negócios (Redesim)3 e a publicação da Lei da Liberdade Econômica4, além de uma série de normativas correlatas. A Redesim é um sistema integrado que permite a abertura, fechamento, alteração e legalização de empresas em todas as Juntas Comerciais do Brasil, simplificando procedimentos e reduzindo a burocracia ao mínimo necessário. Já a Lei da Liberdade Econômica definiu normas que protegem a livre iniciativa de atividades econômicas e diminui a participação do Estado como agente de intermediação e regularização. Tais iniciativas permitem que, atualmente, empresas de baixo risco, que são em maior quantidade no Brasil, obtenham licenças e alvará de forma automática, ou seja, os pequenos negócios e estabelecimentos classificados como de baixo risco sanitário podem ter a Licença Sanitária emitida na mesma hora que fizerem a solicitação pela internet.

As iniciativas de simplificação e organização do processo de licenciamento além de beneficiar o setor regulado e o ambiente de negócio, também,  demonstraram-se favoráveis para os órgãos reguladores, que podem dispor, a partir de então, de acesso imediato a informações de todas as empresas formalizadas nas juntas comerciais da sua jurisdição, o que, favorece o gerenciamento de risco no território, permitindo o tratamento prioritário de atividades de alto risco. Dessa forma, utilizando-se a nova tecnologia evidenciaria os casos que demandam maior urgência, dessa forma busca-se evitar casos como a emblemática tragédia da Boate Kiss5,6. No caso da Vigilância Sanitária, onde comumente as inspeções são realizadas a partir de demandas externas (denúncias ou solicitações de licenciamento), a integração à Redesim proporciona melhores condições para o gerenciamento proativo do órgão que, de posse das informações sobre localização e atividades das empresas, não precisa aguardar provocações externas para atuar. 

Responsável por coordenar e dar suporte para todas as Vigilâncias Sanitárias do Brasil, a Anvisa publicou a RDC Nº153, de 26 de abril de 2017, que estabeleceu diretrizes nacionais para simplificação  e  integração  dos  procedimentos  de  licenciamento  sanitário  no  âmbito  da Redesim7, e a Instrução Normativa Nº 16/2017, que dispõe sobre a lista de Classificação Nacional de Atividades Econômicas - CNAE classificadas por grau de risco para fins de licenciamento sanitário8. Apesar das iniciativas nacionais para simplificação do licenciamento sanitário no país, levantamento recente realizado pela Agência indica que apenas 6,0% dos municípios realizam o licenciamento de forma integrada à Redesim na internet e apenas 15,4% adotam procedimentos simplificados para concessão da   licença sanitária para atividades econômicas de baixo risco9.

Em Manaus, o licenciamento sanitário é realizado pelo Departamento de Vigilância Sanitária (Visa Manaus), órgão vinculado à Secretaria Municipal de Saúde de Manaus, e o município está integrado à Redesim desde 2015, quando também publicou uma classificação de risco para as atividades econômicas sujeitas à vigilância sanitária10, proporcionando ao município melhores condições para modernização dos órgãos licenciadores.

Entre as principais mudanças evidenciadas nos últimos anos quanto ao  processo de licenciamento sanitário da Visa Manaus estão: adesão a sistema de licenciamento informatizado, emissão de licenças sanitárias digitais, integração  aos demais órgãos de licenciamento (ambiental e urbanístico), digitalização do processo, simplificação e automatização de licenças para estabelecimentos de baixo risco. Tais melhorias foram viabilizadas por meio da implantação do Sistema de Licenciamento Integrado Municipal - SLIM. O sistema foi implantado na Visa Manaus em 2018 e oficialmente instituído na prefeitura pelo Decreto Municipal Nº 4.648, em 12 de novembro de 201911, mas a automatização para emissão de licenças de baixo risco só foi efetivada em 03 de fevereiro de 202012.

O Decreto Municipal Nº 4.648/2019 também atualizou a classificação de risco adotada pela Visa Manaus. A partir de então, a classificação das atividades econômicas passíveis de licenciamento sanitário em Manaus ficaram assim definidas: “alto risco”, “baixo risco” e “risco condicionado”11. Cabe destacar que a classificação como “risco condicionado” é uma classificação intermediária, usada quando a descrição da atividade econômica pela CNAE não é capaz de definir o grau de risco ao qual o estabelecimento está realmente sujeito. Nestes casos, a análise e classificação final do risco da atividade em alto ou baixo é feita por um servidor do órgão e o sistema SLIM não fornece esta informação final, sugerindo uma oportunidade de melhoria no processo.

De qualquer forma, a implantação de um sistema informatizado para a gestão do licenciamento e emissão de licenças sanitárias em Manaus possibilitou aparente melhoria ao processo, além de uma maior geração e disponibilização de dados, o que anteriormente era dificultado pela abertura e tramitação de processos físicos, com procedimentos basicamente manuais, além da precariedade das ferramentas de gestão utilizadas pelo órgão. 

Apesar da adesão ao SLIM possibilitar geração de dados mais robustos, as informações sobre licenciamento sanitário em Manaus continuam indisponíveis ou com acesso restrito, estando limitada tanto para a população quanto para os próprio órgão licenciador, que atualmente dispõe apenas de indicadores quantitativos para a gestão do processo, como a  quantidade de licenças solicitadas versus licenças emitidas, conforme relatório interno da Visa Manaus referente aos dados de gestão 2017 a 202013. Após busca na literatura e em sites de outras Vigilâncias Sanitárias do país, percebeu-se que também não há dados abertos nem indicadores sobre o perfil dos estabelecimentos licenciados nas cidades brasileiras. 

Entendendo que a falta de informações acerca de um processo, qualquer que seja, pode comprometer significativamente a sua gestão e otimização, e com o objetivo de produzir mais informações sobre o licenciamento sanitário em Manaus, subsidiar a gestão do processo pelo órgão de Vigilância Sanitária e dar conhecimento ao setor regulado e à população em geral quanto ao cenário a que estão expostos, este levantamento se propõe a caracterizar o perfil dos estabelecimentos passíveis de licenciamento existentes na cidade e encontrar atributos que interferem na probabilidade de uma empresa ser licenciada ou funcionar de forma irregular (sem licença sanitária).

# Descrição Resumida do Projeto
A cidade de Manaus aderiu à Rede Nacional para a Simplificação do Registro e da Legalização de Empresas e Negócios (REDESIM) em 2015, disponibilizando aos órgãos licenciados acesso ao Sistema de Licenciamento Integrado Municipal - SLIM, uma nova plataforma para emissão de licenças e alvarás no município. A Vigilância Sanitária de Manaus, responsável pela emissão de licenças sanitárias, implementou o SLIM a partir de fevereiro de 2018, quando as licenças sanitárias passaram a ser emitidas em formato digital. O órgão não dispõe de dados anteriores a fevereiro de 2018, quando não havia sistemas informatizados e estatísticas detalhadas acerca do licenciamento sanitário no município. O presente projeto tem a proposta de analisar o perfil dos estabelecimentos sujeitos à Vigilância Sanitária existentes em Manaus e das licenças emitidas por meio do sistema atualmente utilizado, o qual está parametrizado com os requisitos da Lei de Liberdade Econômica e integrado à REDESIM, bem como encontrar parâmetros associados à regularização das empresas que exercem atividades de saúde ou de interesse à saúde no território de Manaus, além de fornecer subsídios e recomendações para o órgão regulador otimizar sua atuação voltada para segurança sanitária da prestação de serviços e da produção e circulação de bens. 

> [Link para vídeo da Proposta](https://drive.google.com/file/d/1cgtKYQ0HazdL1GH1zUqj3C_ZMvQsadIi/view)

> [Link para vídeo da Apresentação Final]()

> [Slides da Proposta](https://drive.google.com/drive/u/1/folders/1BStruK_Xw899V4RjTQcJ_tggbBP1onUl)

> [Slides da Apresentação Final]()



# Perguntas de Pesquisa
* Qual o perfil dos estabelecimentos licenciados e não licenciados quanto ao risco sanitário, localização geográfica e atividade desenvolvida?
* O maior percentual de estabelecimentos licenciados e não licenciados tem relação com o risco sanitário, atividade da empresa e IDH da região?
* É possível predizer se empresas enquadradas em determinados grupos (região, segmento de atividade, etc) irão ou não solicitar o licenciamento antes de começarem a funcionar?

# Bases de Dados
## Refazer 
# Metodologia
O pipeline seguido por este estudo será o KDD presente na figura abaixo. A partir do entendimento do problema macro, é possível traçar os objetivos da pesquisa. Assim, com as perguntas científicas formuladas, e a seleção dos bancos de dados promissores realizada, inicia-se a etapa de **data cleaning** e tratamento de dados faltantes. A transformação dos dados presentes será feita visando facilitar a validação de algumas hipóteses estabelecidas no início, neste ponto tem-se como opções a redução de dimensionalidade e a normalização por exemplo. A fase de **Data Mining** consiste tanto na aplicação de algoritmos utilizando conceitos de aprendizado de máquina como regressão, classificação e clustering quanto de análises estatísticas, como correlações e estatísticas descritivas. Finalmente, em **Interpretation / Evaluation** será possível gerar insights a partir das análises já realizadas. 

É válido ressaltar que este método é iterativo, desta forma, caso os bancos de dados coletados se mostrem insuficientes, novos serão coletados a fim de gerar insights mais expressivos.

![Metodologia Adotada](./reports/figures/metodologia.png)

# Ferramentas
O projeto será feito em [Python 3](https://www.python.org/), junto do [Jupyter Notebook](https://jupyter.org/). Para o tratamento de dados, utilizar-se-á de dataframes suportados pela biblioteca [Pandas](https://pandas.pydata.org/) ou em arrays suportados pela biblioteca [NumPy](https://numpy.org/). Os modelos serão treinados na biblioteca [Scikit-Learn](https://scikit-learn.org/stable/) ou pelo [TensorFlow](https://www.tensorflow.org/).

# Bases de Dados e Evolução
## Refazer isso

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>

Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io
