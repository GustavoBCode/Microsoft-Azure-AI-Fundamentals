# Azure Cognitive Search: Utilizando AI Search para indexação e consulta de Dados

Neste projeto, mergulhamos na tecnologia do Azure Cognitive Search, uma ferramenta inteligente que revoluciona a forma como buscamos e analisamos dados. Ao longo de algumas etapas simples e práticas, os participantes aprendem desde a configuração inicial até a execução de consultas avançadas. Com isso, eles ganham habilidades valiosas para explorar conjuntos de dados de maneira eficiente e inteligente. No final, estarão prontos para aplicar essas habilidades em uma ampla gama de contextos, desde análises básicas até soluções de pesquisa personalizadas e sofisticadas.

Link utilizado no projeto: [Explore an Azure AI Search index (UI)](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html)

# 1 - Criando um recurso (AI Search)

1.1 - Na Página inicial, navegue até **Mais serviços** e selecione **Pesquisa de IA**.

![1](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/3cefdb5a-1006-4a22-a794-7f0a5496f668)

1.2 - Clique em **Criar serviço pesquisa**.

![2](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/5aa37e14-ab7d-41b4-abb0-c39c25ecc842)

1.3 -  Se você ainda não tiver um **Grupo de Recursos**, crie um *nomeando-o como **LABAI-900**. Defina o **Nome do serviço** como **aisearchia900**, a região como **East US** e a camada de preço como **Básico**. Prossiga clicando em **Revisar + criar**.

![3](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/7e17c3c3-e69e-46a1-8c83-b2491a938a41)

1.4 - Finalize o processo clicando em **Criar**.

![4](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/6f7c1dd0-0e4c-4fc8-8230-c245f4100edd)

# 2 - Criando um recurso (IA services)

2.1 - Na barra lateral, clique em **Criar um recurso**, selecione **IA + Machine Learning** em **Categorias** e clique em **Criar**.

![1](https://github.com/GustavoBCode/Reconhecimento-Facial-e-transformacao-de-imagens-em-Dados-no-Azure-ML/assets/146696103/be1d3df1-d966-464a-8bfb-88bbc9b8ccb9)

2.2 - Em **Grupo de Recursos**, selecione **LABAI-900**. No campo Nome, insira **buscascognitivasai900**. Selecione **Standard S0** como o **Tipo de Preço** e marque a caixa de seleção. Clique em **Examinar + criar**.

![5](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/0a743ca8-aa5d-45f0-bb13-0ebe88883b44)

2.3 - Finalize o processo clicando em **Criar**.

![6](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/50d0482b-8a96-4f83-8e02-aa46ff07a09e)

# 3 - Criando um recurso (Contas de armazenamento)

3.1 - Na Página inicial, clique em **Contas de armazenamento**.

![7](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/9972c034-57fb-409c-819c-84b124da962c)

3.2 - Clique em **Criar**.

![8](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/32a7646d-e402-4f92-9fe0-135171002510)

3.3 - Em **Grupo de Recursos**, selecione **LABAI-900**. No campo **Nome da conta de armazenamento**, insira **buscascognitivasai900**. Selecione **LRS (armazenamento com redundância local)**. Clique em **Revisar + criar**.

![9](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/eed69ee8-67d0-44ea-867e-d14a6affb41e)

3.4 - Finalize o processo clicando em **Criar**.

![10](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/90e6bd9c-faea-4b25-a982-c0f8c05e4631)

# 4 - Configurando e Carregando arquivos (Contas de armazenamento)

4.1 - Clique em **Ir para recurso**.

![11](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/270de3bc-b910-45cf-b291-3262a9bc5a24)

4.2 - Na barra lateral, encontre a categoria **Configurações** e clique em **Configuração**. Habilite o acesso anônimo ao Blob clicando em **Habilitado**. Clique em **Salvar**.

![12](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/4d754f98-92ea-4d9f-b953-1ddddf299d2b)

4.3 -  Na barra lateral, vá para **Armazenamento de dados** e clique em **Contêineres**. Adicione um novo **contêiner** com o nome **coffeereviews** e configure o Nível de acesso anônimo** como **Contêiner**. Clique em **Criar**.

![13](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/cd9cb840-bdab-4412-b5f5-2c2780f95284)

4.4 - Clique em **coffeereviews**.

![14](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/2b8775c9-03e6-491d-9520-e762d0c8f99e)

4.5 - Baixe o arquivo [reviews](https://raw.githubusercontent.com/MicrosoftLearning/mslearn-ai-fundamentals/main/data/knowledge/reviews.zip) e  extraia-o. Em seguida, clique em **Carregar**. Clique em **Procurar arquivos**, selecione todos os arquivos na pasta reviews e clique em **Carregar**.

![15](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/bdc83464-53e1-4bb9-a349-3ccb9b713c4e)

# 5 - Importando dados (Pesquisa de IA)

5.1 - Na Página inicial, clique em **Pesquisa de IA**.

![16](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/b8fef804-8d2d-4f30-bb18-a6fa16b6d569)

5.2 - Clique em **aisearchai900**.

![17](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/6d9292a7-4256-4b01-afd2-6865ceb2c2ca)

5.3 - Clique em **Importar dados**.

![18](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/f7191ea3-5c8a-440d-86bd-7dd1d9a74954)

5.4 - Selecione **Fonte de dados existente** e escolha **Armazenamento de Blob do Azure**.

![19](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/fc0aae2f-99ef-4df6-a6fd-32eef49927b4)

5.5 - Nomeie a fonte de dados como **coffeereviews** e selecione a conexão existente **buscascognitivasai900**, seguido de **coffeereviews**. Clique em **Selecionar**.

![20](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/991dc8c1-859a-4f13-8e85-027bba2f6c0e)

![21](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/fe25aa97-1edc-4e25-897d-19e906a8aa3f)

5.6 - Siga as instruções do [Explorar um índice de Pesquisa de IA (UI) do Azure](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html) nas etapas 4 a 15, no tópico **indexar os documentos**.

![22](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/ea7a50d9-bfea-4cd9-b29f-7f5138a62bd0)

# 6 - Gerenciador de pesquisa

6.1 - Acesse o **Gerenciador de pesquisa**.

![23](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/d1792b72-1e4d-4e28-94d0-d6a5a71d0108)

6.2 - Para testar a consulta, insira o código **search=*&$count=true** e clique em **Pesquisar**.

![24](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/78a6b29e-bfce-4d45-a22a-83318e8c533f)

6.3 - Para buscar avaliações em Chicago, utilize o código **search=locations:'Chicago'** e clique em **Pesquisar**.

![25](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/1c7a65ad-9df9-4b90-ba1f-badda037235d)

6.4 - Para encontrar avaliações negativas, use o código **search=sentiment:'negative'** e clique em **Pesquisar**.

![26](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/50bc29c5-2d78-42a6-a531-a0112d2a1caf)


# Conclusão 

A capacidade de utilizar ferramentas como o Azure Cognitive Search no mundo real é uma oportunidade empolgante e transformadora. Com essa tecnologia, podemos aprimorar a eficiência e a precisão de pesquisas de informações em uma ampla gama de setores e aplicações. Desde a análise de grandes conjuntos de dados para tomada de decisões estratégicas até a criação de sistemas de pesquisa avançados para clientes e usuários finais, o potencial é vasto. Além disso, a capacidade de personalizar e adaptar essas soluções de acordo com as necessidades específicas de cada projeto ou organização permite uma flexibilidade e escalabilidade sem precedentes. Em resumo, o uso dessas ferramentas no mundo real não apenas melhora a eficiência e a precisão, mas também impulsiona a inovação e abre novas oportunidades para criar valor e impacto positivo em diversos campos e setores.
