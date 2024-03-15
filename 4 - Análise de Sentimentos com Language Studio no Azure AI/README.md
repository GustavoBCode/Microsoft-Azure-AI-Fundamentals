# Análise de Sentimentos com Language Studio no Azure AI

Este projeto aborda a implementação de funcionalidades de análise de fala em tempo real, além de análise de sentimentos e opiniões.

Links utilizados no projeto: | [Explore Speech Studio](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/09-speech.html) | [Analyze text with Language Studio](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/06-text-analysis.html) |

# 1 - Conversão de fala em texto em tempo real

1.1 - Acesse o [Speech Studio](https://speech.microsoft.com/portal) e selecione a opção **Conversão de fala em texto**. Clique em **Conversão de fala em texto em tempo real**.

![1](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/dadebdf8-2c9f-4766-a1fd-50884bdcc166)

# 2 - Criando um recurso

2.1 - Na barra lateral, clique em **Criar um recurso**. Escolha a categoria **IA + Machine Learning** e clique no botão **Criar**.

![2](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/db347e84-87b9-431d-a036-7d22159852c6)

2.2 - Clique em **Continue to create your resource**.

2.3 - Se você ainda não tiver um **Grupo de Recursos**, clique em **Criar Novo** e dê o nome de **LABAI-900**. No campo **Nome**, insira **languagestudio-lab**. No campo **Tipo de Preço**, selecione **Free F0**. Marque a caixa de seleção. Agora clique em **Examinar + criar**.

![3](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/5bdba478-ad3e-4420-bf39-98fe70609ba1)

2.4 - Finalize o processo clicando em **Criar**.

![4](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/05c50e91-06e5-4b3d-9423-aa519ef70e73)

# 3 - Análise de sentimentos e opiniões

3.1 - Acesse o [Language Studio](https://language.cognitive.azure.com/home). Nos campos **Azure subscription** e **Resource name**, selecione as seguintes opções: Azure subscript 1 e languagestudio-lab. Em seguida, clique em **Done**.

![5](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/8e039f7f-2d35-4677-b08c-4a07b5ecbded)

3.2 - Selecione **Classify text** e, em seguida,**Analyze sentiment and opinions**.

![6](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/4e1bc165-affc-4720-b789-443314f1565c)

3.3 - Escolha **Portuguese (Brazil)** e cole a [avaliação de hotel](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/blob/main/4%20-%20Análise%20de%20Sentimentos%20com%20Language%20Studio%20no%20Azure%20AI/inputs/Análise%20de%20sentimentos%20e%20opiniões.txt) na caixa de texto. Marque a caixa de seleção e clique em **Run**.

![7](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/ce9e5a3b-81a5-470a-90e5-8eb60570b175)

![8](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/d6659618-c58d-40b1-9908-5788561be896)

3.4 - O resultado será exibido como: 44.00% POSITIVE | 0.00% NEUTRAL | 56.00% NEGATIVE.

![9](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/57026215-4c1a-4080-87c0-f7a111c25e80)

3.5 - Avaliação de palavras-chave do texto original.

![10](https://github.com/GustavoBCode/Microsoft-Azure-AI-Fundamentals/assets/146696103/202089a8-c6b8-4bc7-bcf8-315b5d3278cb)

# Conclusão
As ferramentas de conversão de fala em texto em tempo real e análise de sentimentos têm diversas aplicações práticas, como melhorar o atendimento ao cliente, monitorar mídias sociais e facilitar o registro de consultas médicas. Elas oferecem insights valiosos para análise de mercado e inteligência empresarial, ajudando na tomada de decisões estratégicas. Por meio da transcrição e análise de sentimentos, as empresas podem compreender as necessidades e sentimentos dos clientes, ajustando suas estratégias de acordo. Essas ferramentas são versáteis e têm o potencial de aprimorar a eficiência operacional e a experiência do cliente em diversos setores.




