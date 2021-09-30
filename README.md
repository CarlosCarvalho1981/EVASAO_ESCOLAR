# EVASAO ESCOLAR:
Notebooks criados para fazer o perfil de estudantes que se formam em cursos técnicos e também para fazer previsão se os estudantes irão desistir ou concluir o curso.
Os dados originais não podem ser apresentados, mas são dados de todos os cursos de uma escola profissionalizante coletados entre 2015 e 2020, em Santa Catarina.
PERFIL_GERAL: Recebe os dados brutos, faz a seleção e limpeza, salvando em um arquivo csv que será usado na próxima etapa.
PERFIL_TECNICO: Recebe os dados limpos da etapa anterior e gera gráficos para determinar o perfil dos estudantes que se formam nos cursos técnicos. O objetivo é fazer uma campanha de marketing focada no público que tem mais tendência a concluir o curso.
ML_ONE_HOT_ENCODER: Notebook usado para testar diversos algoritmos de ML (Regressão Logística, KNN, Linear SVM, RBF SVM, Gaussian Process, Árvore de Decisão, Floresta Aleatória, Rede Neural, AdaBoost, Naive Bayes e QDA) com o One Hot Encoder.
ML_WEIGHT_EVIDENCE: Testa os mesmos algoritmos acima mas usa o Weight of Evidence Encoder.
ML_MEAN_TARGET: Testa os mesmos algoritmos acima usando o Mean Target Encoder.
ML_JAMES_STEIN: Testa os mesmos algoritmos com o James Stein Encoder.
ML_CATBOOST: Usa o pacote CatBoost para fazer o encoder das variáveis categóricas e usa o algoritmo Random Forest.
Ao final, o modelo que melhor se adaptou aos dados foi o que usa o CatBoost, com acurácia de 88% e foi o escolhido para ser utilizado.
Esse modelo será aplicado em turmas novas para fazer a previsão de qual estudante irá desistir do curso.  O objetivo é que a coordenação do curso tenha uma base para iniciar uma conversa com os estudantes e buscar possíveis motivos de desistência de forma a auxiliar os estudantes a ficarem no curso até o final.

# TRUANCY
These notebooks were made to find the profile of studants that graduate in technical courses and also to predict if the students will finish the course or drop out.
The original data can't be shared but they were collected between 2015 and 2020, at a technical school, in Santa Catarina, Brazil.
PERFIL_GERAL: Gets the raw data, selects the variables and cleans the data, saving it in a csv file that will be used in the next step.
PERFI_TECNICO: Gets the clean data from the previous step and generates bar graphs to find the profile of students that graduate in technical courses.  The goal is to make a marketing campain targeting the audience the probably will finish the course.
ML_ONE_HOT_ENCODER: Notebook used to test various ML algorithms (LogisticRegression, Linear SVM, RBF SVM, Gaussian Process, Decision Tree, Random Forest, Neural Network, AdaBoost, Naive Bayes and QDA) using One Hot Encoder.
ML_WEIGHT_EVIDENCE: Tests the same algorithms above but uses Weight of Evidence Encoder.
ML_MEAN_TARGET: Tests the same algorithms above using Mean Target Encoder.
ML_JAMES_STEIN: Tests the same algorithms above with James Stein Encoder.
ML_CATBOOST: Uses the package CatBoos to encode categorical variables and uses Random Forest algorithm.
At the end, the algorithm that got the best result was the one using CatBoost, reaching an accuracy of 88%.
This model will be apply to new classes to predict which estudent will drop out the course.  The objective here is give the course coordinators a baseline to begin a coversation with the students and find possible reasons for them to drop out, helping them to finish the course.
