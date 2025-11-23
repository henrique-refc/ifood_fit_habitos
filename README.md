# ifood_fit_habitos
Algoritmo para auxiliar na aquisição de hábitos fitness, em parceria com o iFood.

🥗 Ifood Fit: Seu Guia Personalizado para Hábitos Alimentares Saudáveis
Visão Geral do Projeto

O Ifood Fit é uma iniciativa inovadora projetada para auxiliar indivíduos na jornada de mudança e manutenção de hábitos alimentares saudáveis. Com foco em gamificação, personalização e motivação contínua, a aplicação cria uma experiência envolvente ao acompanhar metas de bem-estar, oferecer recompensas e proporcionar sugestões de refeições inteligentes.
Este projeto simula uma integração com a plataforma iFood, aproveitando seu alcance e recorrência através de planos de assinatura.

Além disso, o conceito deste algoritmo foi inspirado no livro “O Poder do Hábito”, de Charles Duhigg (2012), que explica a formação de hábitos a partir do loop: gatilho → rotina → recompensa. No Ifood Fit, esse ciclo é aplicado da seguinte forma:

Gatilho: horário aproximado e agendado para o recebimento das refeições diariamente

Rotina: consumo de uma refeição saudável conforme a meta

Recompensa: descontos em itens “não fitness” ao alcançar o objetivo definido

Esse modelo fortalece a consistência e facilita a adoção de hábitos saudáveis de forma prazerosa e sustentável.

Funcionalidades Principais
🎯 Definição e Acompanhamento de Metas de Hábitos Saudáveis

O usuário define metas de dias consecutivos com alimentação saudável (ex.: 3, 6, 12, 20 e 30 dias).
O sistema acompanha o progresso, registra a evolução e celebra cada conquista para reforçar o hábito.

🎁 Sistema de Recompensas Inteligente

Ao concluir uma meta, o usuário recebe ofertas e descontos em alimentos mais indulgentes disponíveis no iFood — um “mimo” controlado que mantém o prazer e reduz a frustração do processo.
As recompensas são geradas dinamicamente para oferecer variedade e atratividade contínuas.

🧠 Sugestões de Refeições Saudáveis com IA (LLM)

Utilizamos um Large Language Model (Google Gemini) para gerar sugestões de refeições equilibradas e compatíveis com o IMC, preferências e necessidades nutricionais de cada usuário.

📊 Cálculo e Classificação do IMC

No cadastro inicial, o aplicativo calcula e classifica o IMC do usuário (ex.: peso normal, sobrepeso, obesidade), garantindo personalização do acompanhamento.

🔄 Recorrência e Escalabilidade por Assinaturas

Planos de 3, 6 e 12 meses garantem:
 
acompanhamento constante da mudança de hábitos

modelo de negócio sustentável com receita recorrente

maior engajamento do usuário no longo prazo

🤖 Modelo de Recomendação de ML

Um Random Forest Classifier aprende com o histórico do usuário e passa a sugerir refeições cada vez mais alinhadas às suas preferências e objetivos.

Como Funciona (Fluxo Básico)

Cadastro Inicial: nome, peso e altura → cálculo do IMC

Escolha do Plano de Assinatura: 3m, 6m ou 12m

Definição da Meta: dias saudáveis consecutivos

Registro Diário: confirmação de refeição saudável

Recompensas: liberadas ao atingir a meta

Sugestões Inteligentes: refeições saudáveis via IA

Tecnologias Utilizadas

Python — linguagem principal

Pandas — manipulação de dados

scikit-learn — Machine Learning (RandomForestClassifier)

Google Generative AI (Gemini) — sugestões personalizadas por IA

Google Colab / Jupyter Notebook — execução e desenvolvimento

Configuração e Execução

1️⃣ Obtenha uma API Key do Google e configure como segredo no Colab:

Nome do segredo: GOOGLE_API_KEY

2️⃣ Instale as dependências necessárias:

pandas

scikit-learn

google-generativeai

3️⃣ Execute o código principal para iniciar a aplicação interativa.
