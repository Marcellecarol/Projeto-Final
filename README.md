# Projeto-Final
Sistema de Informações Ambulatoriais (SIA)


Descrição
Este projeto utiliza dados do Sistema de Informações Ambulatoriais (SIA) para analisar atendimentos e procedimentos realizados em estabelecimentos de saúde no Brasil, com foco em eficiência, distribuição demográfica e evolução ao longo do tempo.

Motivação
A análise dos atendimentos ambulatoriais é fundamental para aprimorar a gestão de recursos na saúde pública e otimizar os serviços prestados à população.

Pré-requisitos
Python 3.8+
Pandas
BigQuery
Google Cloud SDK
Instalação
Passos para Configuração:
# Clone o repositório
git clone https://github.com/Marcellecarol/Projeto-Final.git

# Acesse o diretório do projeto
cd Projeto-Final

# Instale as dependências
pip install -r requirements.txt

Uso
Como Rodar o Projeto: Para executar os scripts e análises, use os seguintes comandos:
Consulta SQL no BigQuery:
# Executar coleta de dados
python coleta_dados.py

# Processar dados
python processamento_dados.py

# Escrever os resultados em um arquivo
python escrita_dados.py

sql
Copiar código
SELECT estado, COUNT(*) AS total_atendimentos
FROM `sistema_informacoes_ambulatoriais.atendimentos`
GROUP BY estado;
Rodar análise em Python:

bash
Copiar código
python analise_atendimentos.py --ano 2024
Estrutura do Projeto
plaintext
Copiar código
├── data                   # Dados ambulatoriais
├── scripts                # Scripts de análise
├── notebooks              # Notebooks Jupyter
└── README.md              # Documentação
Contribuição
Contribuições são bem-vindas!.

Licença
Este projeto está licenciado sob a MIT License - veja o arquivo LICENSE para mais detalhes.

Contato
Para dúvidas ou sugestões, entre em contato: marcellecarolina15@gmail.com.
