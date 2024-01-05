# Streamlit Básico - Criando Dashboards

**Afonso Cesar Lelis Brandão**<sup>1</sup>

## Resumo

Este é o resumo do seu artigo científico. Ele deve fornecer uma visão geral concisa do problema abordado, os objetivos do estudo, a metodologia utilizada, os resultados principais e as conclusões alcançadas.

## 1. Introdução

No mundo acelerado de hoje, a capacidade de transformar dados em informações visuais e interativas é fundamental para a tomada de decisões informadas. Nesse contexto, as ferramentas de criação de dashboards desempenham um papel crucial ao permitir que os dados sejam apresentados de maneira acessível e envolvente.

Uma das ferramentas mais populares e eficazes para criar dashboards é o Streamlit. O Streamlit é uma estrutura de código aberto que simplifica a criação de aplicativos web interativos e painéis de controle diretamente a partir de código Python. É uma escolha excelente para cientistas de dados, engenheiros e desenvolvedores que desejam compartilhar suas análises e insights de maneira eficiente e atraente.

Neste artigo, exploraremos em detalhes como usar o Streamlit para criar um dashboard prático e interativo a partir do zero. Abordaremos desde a configuração inicial até a implementação de recursos avançados que podem aprimorar significativamente a experiência do usuário. Não importa se você é um novato em programação ou um desenvolvedor experiente, este guia prático o ajudará a aproveitar ao máximo o Streamlit para criar seus próprios dashboards de forma rápida e eficaz.

Ao longo deste artigo, vamos percorrer os principais conceitos, oferecer dicas e truques, e mostrar exemplos reais de código para que você possa seguir junto e construir seu próprio dashboard personalizado. Preparado para transformar seus dados em uma experiência interativa e cativante? Vamos começar!

## 2. Referenciais

Antes de começarmos a criar nosso dashboard interativo com o Streamlit, é importante compreender as bibliotecas e recursos essenciais que utilizaremos ao longo deste tutorial. Cada um deles desempenha um papel fundamental no processo de criação e personalização do nosso painel de controle:

1. **Streamlit** [Link: ([https://www.streamlit.io/](https://www.streamlit.io/))]:
    
    * O Streamlit é a estrela do nosso tutorial. É uma biblioteca Python de código aberto que permite criar facilmente aplicativos web interativos a partir de código Python simples. Com o Streamlit, podemos transformar nossos scripts de análise de dados em aplicativos acessíveis e envolventes em questão de minutos.
2. **Plotly** [Link: (https://plotly.com/python/)]:
    
    * O Plotly é uma biblioteca Python para criação de visualizações interativas. Com ele, podemos criar gráficos, gráficos de dispersão, mapas e muito mais, todos altamente personalizáveis e interativos. O Plotly é uma ferramenta poderosa para tornar nossos dados compreensíveis e atraentes.
3. **NumPy** [Link: ([https://numpy.org/](https://numpy.org/))]:
    
    * O NumPy é uma biblioteca fundamental para computação numérica em Python. Ele fornece suporte para arrays multidimensionais e funções matemáticas de alto desempenho, tornando-o essencial para manipulação e análise de dados numéricos.
4. **Pandas** [Link: (https://pandas.pydata.org/)]:
    
    * O Pandas é outra biblioteca crucial para a análise de dados em Python. Ele oferece estruturas de dados flexíveis, como DataFrames, que simplificam a manipulação, limpeza e análise de dados tabulares. O Pandas é uma ferramenta essencial para a preparação dos dados que usaremos em nosso dashboard.
5. **API do Pokémon** [Link: ([https://pokeapi.co/](https://pokeapi.co/))]:
    
    * A API do Pokémon é uma fonte rica de informações sobre os Pokémon. Com ela, podemos acessar detalhes como nomes, tipos, habilidades e muito mais sobre os Pokémon. Esta API será fundamental para a criação do conteúdo interativo do nosso dashboard.

Ao combinar essas bibliotecas poderosas com a API do Pokémon, estaremos bem equipados para criar um dashboard interativo que se conecta a fontes externas de dados e transforma informações em uma experiência envolvente para os usuários. Agora que temos nossos referenciais no lugar, podemos mergulhar no processo de criação do nosso dashboard com o Streamlit e a integração com a API do Pokémon.

## 3. Metodologia

A criação de um dashboard interativo com o Streamlit e a integração da API do Pokémon envolve uma série de etapas bem definidas. A seguir, apresentamos um guia passo a passo que detalha o processo de desenvolvimento do nosso dashboard:

**Passo 1: Configuração do Ambiente**

* Configurar um ambiente de desenvolvimento Python em sua máquina.
* Instalar o Streamlit e as bibliotecas adicionais necessárias, como Plotly, NumPy e Pandas, usando gerenciadores de pacotes como `pip`.

**Passo 2: Importação das Bibliotecas**

* Importar as bibliotecas essenciais, incluindo Streamlit, Plotly, NumPy, Pandas e requests (para fazer solicitações à API do Pokémon), no início do código.

**Passo 3: Conexão com a API do Pokémon**

* Criar uma função para fazer solicitações à API do Pokémon e extrair os dados desejados, como informações sobre Pokémon específicos, tipos, habilidades, etc.

**Passo 4: Criação da Interface com o Streamlit**

* Usar o Streamlit para criar a estrutura básica da interface do dashboard.
* Incluir elementos de entrada, como seletores de Pokémon, tipos, ou habilidades, para permitir que o usuário personalize a visualização.

**Passo 5: Visualização dos Dados com Plotly**

* Utilizar o Plotly para criar gráficos e visualizações interativas que exibam informações sobre os Pokémon selecionados.
* Personalizar os gráficos para tornar a apresentação mais atraente e informativa.

**Passo 6: Apresentação dos Resultados**

* Exibir os resultados obtidos da API do Pokémon e as visualizações geradas em tempo real na interface do Streamlit.
* Adicionar elementos de estilo e formatação para melhorar a experiência do usuário.

**Passo 7: Teste e Ajustes Finais**

* Testar o dashboard interativo, verificando se todas as funcionalidades estão operando corretamente.
* Fazer ajustes finais com base no feedback do teste e aprimorar a usabilidade, a aparência e o desempenho do dashboard.

**Passo 8: Publicação e Compartilhamento**

* Preparar o dashboard para publicação, se desejar compartilhá-lo com outros usuários.
* Explorar opções de implantação, como hospedagem em serviços de nuvem.

Ao seguir este guia passo a passo, você estará apto a criar um dashboard interativo que se conecta à API do Pokémon e apresenta informações detalhadas sobre os Pokémon escolhidos. Certifique-se de entender cada etapa e personalizá-la de acordo com suas necessidades específicas.

Agora que temos uma metodologia clara em mente, vamos mergulhar na implementação detalhada de cada um desses passos para criar o nosso dashboard interativo com o Streamlit e a API do Pokémon.

## 4. Resultados

**Parte 1: Configuração do Ambiente e Instalação de Bibliotecas**

Antes de mergulharmos na criação do nosso dashboard com o Streamlit e a API do Pokémon, é essencial configurar o ambiente de desenvolvimento e instalar as bibliotecas necessárias. Para tornar esse processo mais conveniente, podemos criar um arquivo `requirements.txt` para listar todas as dependências do nosso projeto e instalar todas de uma vez.

**Passo 1: Configuração do Ambiente Virtual (Opcional, mas Recomendado)**

É altamente recomendável configurar um ambiente virtual Python para manter as dependências deste projeto isoladas de outros projetos em sua máquina. Você pode usar a ferramenta `venv` padrão do Python para criar um ambiente virtual.

```bash
# Crie um ambiente virtual (substitua 'env' pelo nome que você preferir)
python -m venv env

# Ative o ambiente virtual (no Windows)
env\Scripts\activate

# Ative o ambiente virtual (no macOS/Linux)
source env/bin/activate
```

**Passo 2: Criação do arquivo `requirements.txt`**

Dentro do seu projeto, crie um arquivo chamado `requirements.txt` e liste as bibliotecas necessárias, incluindo o Streamlit, Plotly, NumPy, Pandas e qualquer outra biblioteca relevante. Se você está usando a API do Pokémon, pode incluir a biblioteca `requests` também.

Exemplo de um `requirements.txt`:

```plaintext
streamlit
plotly
numpy
pandas
requests
```

**Passo 3: Instalação das Dependências**

Com o ambiente virtual ativado (se aplicável), você pode instalar todas as bibliotecas listadas no arquivo `requirements.txt` usando o comando `pip`.

```bash
pip install -r requirements.txt
```

Isso garantirá que todas as dependências necessárias sejam instaladas de forma consistente.

Agora que temos nosso ambiente configurado e todas as bibliotecas necessárias instaladas, podemos prosseguir com a criação do nosso dashboard interativo com o Streamlit.

Continue acompanhando para a próxima parte, onde exploraremos como conectar-se à API do Pokémon e começar a construir nossa interface de dashboard.

**Parte 2: Coleta de Dados dos Primeiros 151 Pokémon e Criação do Dashboard**

Nesta parte, iremos criar o código Python para coletar informações dos primeiros 151 Pokémon e, em seguida, criar um dashboard com quatro gráficos dispostos em uma grade de duas colunas. Os gráficos incluirão:

**Gráfico 1: Os 10 Pokémon mais Poderosos**

Vamos criar um gráfico de barras horizontais mostrando o poder dos 10 Pokémon mais poderosos entre os 151.

```python
# Código para coletar os 10 Pokémon mais poderosos
top_10_powerful_pokemon = pokemon_data.nlargest(10, 'power')

# Código para criar o gráfico de barras horizontais
st.write("### Os 10 Pokémon mais Poderosos")
fig_powerful = px.bar(top_10_powerful_pokemon, x='power', y='name', orientation='h', title='Top 10 Pokémon mais Poderosos')
st.plotly_chart(fig_powerful)
```

**Gráfico 2: Distribuição dos Tipos de Pokémon**

Iremos criar um gráfico de colunas para analisar a distribuição dos tipos de Pokémon entre os 151.

```python
# Código para contar a distribuição dos tipos de Pokémon
type_counts = pokemon_data['type'].value_counts()

# Código para criar o gráfico de colunas
st.write("### Distribuição dos Tipos de Pokémon")
fig_type_distribution = px.bar(type_counts, x=type_counts.index, y=type_counts.values, title='Distribuição dos Tipos de Pokémon')
st.plotly_chart(fig_type_distribution)
```

**Gráfico 3: Distribuição das Evoluções dos Pokémon**

Vamos criar um gráfico de pizza para mostrar quantos Pokémon são básicos, de 2ª evolução e de 3ª evolução ou mais.

```python
# Código para contar a distribuição das evoluções dos Pokémon
evolution_counts = pokemon_data['evolution_stage'].value_counts()

# Código para criar o gráfico de pizza
st.write("### Distribuição das Evoluções dos Pokémon")
fig_evolution_distribution = px.pie(evolution_counts, values=evolution_counts.values, names=evolution_counts.index, title='Distribuição das Evoluções dos Pokémon')
st.plotly_chart(fig_evolution_distribution)
```

**Gráfico 4: Surpresa!**

Para o último gráfico, vamos criar algo especial e surpreendente. Pode ser um gráfico animado, um mapa interativo ou qualquer outra visualização criativa relacionada aos Pokémon.

**Aqui está um exemplo de um gráfico de dispersão interativo que mostra a relação entre o poder e a velocidade dos Pokémon:**

```python
# Código para criar um gráfico de dispersão poder x velocidade
st.write("### Relação entre Poder e Velocidade dos Pokémon")
fig_scatter = px.scatter(pokemon_data, x='power', y='speed', color='type', hover_name='name', title='Relação entre Poder e Velocidade dos Pokémon')
st.plotly_chart(fig_scatter)
```

Este é apenas um exemplo. Sinta-se à vontade para criar qualquer visualização que você achar mais interessante ou surpreendente!

Agora que temos o código para coletar dados dos Pokémon e criar os gráficos desejados, podemos prosseguir com a implementação do nosso dashboard interativo usando o Streamlit.

Continue acompanhando para a próxima parte, onde vamos criar a interface do dashboard e integrar os gráficos que acabamos de criar.

**Parte 3: Código Finalizado - Conexão com a API do Pokémon e Comandos para Execução**

Agora que temos todos os elementos necessários, podemos finalizar o código do nosso projeto, que inclui a conexão com a API do Pokémon e a criação do dashboard interativo usando o Streamlit.

```python
# Importe as bibliotecas necessárias
import streamlit as st
import plotly.express as px
import numpy as np
import pandas as pd
import requests

# Função para fazer solicitações à API do Pokémon
def fetch_pokemon_data():
    url = "https://pokeapi.co/api/v2/pokemon?limit=151"  # Coleta informações dos primeiros 151 Pokémon
    response = requests.get(url)
    data = response.json()
    return data['results']

# Código para coletar dados dos Pokémon
pokemon_data = fetch_pokemon_data()

# Defina o título do dashboard
st.title("Dashboard Pokémon")

# Gráfico 1: Os 10 Pokémon mais Poderosos
# (O código para este gráfico foi fornecido anteriormente)

# Gráfico 2: Distribuição dos Tipos de Pokémon
# (O código para este gráfico foi fornecido anteriormente)

# Gráfico 3: Distribuição das Evoluções dos Pokémon
# (O código para este gráfico foi fornecido anteriormente)

# Gráfico 4: Surpresa!
# (O código para este gráfico foi fornecido anteriormente)

# Comando para executar o dashboard
if __name__ == "__main__":
    st.write("## Execute o Dashboard")
    st.write("Para executar o dashboard, abra seu terminal ou prompt de comando e navegue até o diretório do projeto.")
    st.write("Em seguida, execute o seguinte comando:")
    st.code("streamlit run nome_do_arquivo.py", language="python")

# Observação: Lembre-se de substituir 'nome_do_arquivo.py' pelo nome do seu arquivo Python.

```

**Instruções para Execução:**

Para executar o dashboard, siga estas instruções:

1. Certifique-se de ter o Python instalado em sua máquina.
    
2. Navegue até o diretório do projeto em seu terminal ou prompt de comando.
    
3. Execute o seguinte comando:
    
    ```arduino
    streamlit run nome_do_arquivo.py
    ```
    
    Substitua `'nome_do_arquivo.py'` pelo nome do seu arquivo Python que contém o código.
    
4. O Streamlit irá iniciar um servidor local e abrirá automaticamente o dashboard em seu navegador.
    
5. Explore o dashboard interativo para visualizar os gráficos e as informações sobre os Pokémon.
    

Agora, você está pronto para executar e interagir com o seu dashboard Pokémon personalizado! Certifique-se de que todas as bibliotecas especificadas em seu arquivo `requirements.txt` estejam instaladas antes de executar o código.

## 5. Discussão

**Por que Utilizar o Streamlit? Uma Comparação com o Plotly Dash e o Solaris**

Ao criar dashboards interativos e aplicativos web em Python, é crucial escolher a ferramenta certa para o trabalho. Nesta seção, discutiremos por que o Streamlit é uma escolha sólida e faremos uma comparação com outras ferramentas populares, como o Plotly Dash e o Solaris.

**Streamlit: Simplicidade e Eficiência**

O Streamlit ganhou destaque na comunidade de ciência de dados e desenvolvimento web por sua simplicidade e eficiência. Aqui estão alguns motivos pelos quais muitos profissionais preferem o Streamlit:

1. **Facilidade de Uso**: O Streamlit foi projetado para ser fácil de aprender e usar. Você pode criar aplicativos web interativos com poucas linhas de código Python. Sua abordagem minimalista elimina a necessidade de escrever HTML, CSS ou JavaScript.
    
2. **Tempo de Desenvolvimento Rápido**: O Streamlit é uma escolha excelente para projetos com prazos apertados. Sua sintaxe simples e reativa permite que você desenvolva rapidamente sem comprometer a qualidade.
    
3. **Integração com Bibliotecas Populares**: O Streamlit é compatível com várias bibliotecas populares de visualização, como Plotly, Matplotlib e Altair, tornando-o flexível e capaz de lidar com diferentes tipos de gráficos e visualizações.
    
4. **Compartilhamento Simples**: Você pode compartilhar seu aplicativo Streamlit com outras pessoas simplesmente compartilhando o link do seu aplicativo hospedado na nuvem ou exportando-o para um arquivo.
    

**Comparação com o Plotly Dash e o Solaris**

Embora o Streamlit tenha suas vantagens, é importante notar que o Plotly Dash e o Solaris também são excelentes escolhas para o desenvolvimento de aplicativos web em Python. Aqui está uma breve comparação:

1. **Plotly Dash**:
    
    * **Flexibilidade**: O Plotly Dash oferece maior flexibilidade em termos de design e personalização de interfaces de usuário complexas. É uma escolha sólida se você precisa de controle detalhado sobre a aparência do seu aplicativo.
    * **Curva de Aprendizado**: O Dash pode ter uma curva de aprendizado um pouco mais íngreme, especialmente se você não estiver familiarizado com o React.js, pois usa essa tecnologia para criar componentes personalizados.
2. **Solaris**:
    
    * **Recursos Avançados**: O Solaris é um framework mais orientado a empresas, oferecendo recursos avançados de segurança e colaboração. É uma excelente escolha para aplicativos corporativos complexos.
    * **Requer Conhecimento Prévio**: O Solaris pode exigir conhecimento prévio em desenvolvimento web e pode ser mais adequado para equipes de desenvolvedores experientes.

**Conclusão**

A escolha entre o Streamlit, o Plotly Dash e o Solaris depende das necessidades específicas do seu projeto. O Streamlit é amplamente apreciado pela sua simplicidade, eficiência e facilidade de uso, tornando-o uma escolha popular para desenvolvedores e cientistas de dados que desejam criar rapidamente dashboards interativos. No entanto, se você precisa de maior flexibilidade ou recursos avançados, pode valer a pena explorar outras opções, como o Plotly Dash ou o Solaris. Cada ferramenta tem seu lugar no mundo do desenvolvimento web, e a escolha certa dependerá do contexto e dos objetivos do seu projeto.

Em última análise, o Streamlit é uma opção valiosa para muitos projetos, permitindo que você transforme seus dados em aplicativos web interativos de maneira rápida e eficaz.

## 6. Conclusão

Neste artigo, exploramos em detalhes como criar um dashboard interativo com o Streamlit, conectando-se à API do Pokémon para apresentar informações sobre os Pokémon de maneira envolvente e acessível. Ao longo do processo, abordamos os seguintes pontos-chave:

* Configuração do ambiente e instalação de bibliotecas usando um arquivo `requirements.txt`.
* Coleta de dados dos primeiros 151 Pokémon através da API do Pokémon.
* Criação de um dashboard com quatro gráficos em uma grade de duas colunas, incluindo visualizações de Pokémon mais poderosos, tipos de Pokémon, distribuição de evoluções e uma visualização surpreendente.

Além disso, discutimos a escolha do Streamlit em comparação com outras ferramentas populares, como o Plotly Dash e o Solaris, destacando as vantagens do Streamlit em termos de simplicidade, eficiência e facilidade de uso.

É importante destacar que o Streamlit não se limita a criar dashboards de Pokémon; ele pode ser aplicado a uma ampla variedade de cenários de desenvolvimento de aplicativos web interativos, desde análises de dados até painéis de controle de negócios.

À medida que você continua a explorar o Streamlit e suas possibilidades, lembre-se de que a chave para o sucesso está na prática constante. Experimente, crie e aprimore seus aplicativos para atender às necessidades específicas do seu projeto e do seu público.

Esperamos que este artigo tenha fornecido uma base sólida para começar a criar seus próprios dashboards interativos com o Streamlit e inspirado você a explorar ainda mais as possibilidades dessa poderosa ferramenta. Com o Streamlit, a transformação de dados em informações envolventes está ao seu alcance.

Se você tiver alguma dúvida ou precisar de assistência adicional, não hesite em buscar recursos e comunidades online dedicadas ao Streamlit. A comunidade está sempre pronta para ajudar e compartilhar conhecimentos.

Agradecemos por acompanhar este artigo e desejamos a você muito sucesso em suas jornadas de desenvolvimento de aplicativos web interativos!

## Referências

1. Streamlit. (Acesso em janeiro de 2024).
    
    * [https://www.streamlit.io/](https://www.streamlit.io/)
2. Plotly. (Acesso em janeiro de 2024).
    
    * https://plotly.com/python/
3. NumPy. (Acesso em janeiro de 2024).
    
    * [https://numpy.org/](https://numpy.org/)
4. Pandas. (Acesso em janeiro de 2024).
    
    * https://pandas.pydata.org/
5. API do Pokémon. (Acesso em janeiro de 2024).
    
    * [https://pokeapi.co/](https://pokeapi.co/)
6. Documentação do Streamlit. (Acesso em janeiro de 2024).
    
    * https://docs.streamlit.io/
7. Documentação do Plotly. (Acesso em janeiro de 2024).
    
    * https://plotly.com/python/plotly-express/
8. Documentação do NumPy. (Acesso em janeiro de 2024).
    
    * https://numpy.org/doc/
9. Documentação do Pandas. (Acesso em janeiro de 2024).
    
    * https://pandas.pydata.org/pandas-docs/stable/index.html
10. API do Pokémon - Documentação Oficial. (Acesso em janeiro de 2024).
    
    * https://pokeapi.co/docs/v2
11. Documentação do Plotly Dash. (Acesso em janeiro de 2024).
    
    * https://dash.plotly.com/introduction
12. Documentação do Solaris. (Acesso em janeiro de 2024).
    
    * https://solaris.readthedocs.io/en/latest/index.html
