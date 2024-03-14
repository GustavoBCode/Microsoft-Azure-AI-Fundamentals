# Reconhecimento Facial e transformação de imagens em Dados no Azure ML

Este projeto tem como objetivo mostrar passo a passo de como utilizar uma plataforma baseada em inteligência artificial (IA) para análise e processamento avançado de imagens. A plataforma [**Vision Studio**](https://portal.vision.cognitive.azure.com/gallery/featured) é projetada para oferecer uma série de recursos, desde a detecção de objetos e faces até a extração de texto de imagens e adição de legendas. É uma solução versátil que pode ser aplicada em uma variedade de contextos, desde reconhecimento facial para segurança até reconhecimento óptico de caracteres para digitalização de documentos.

Links utilizados no projeto: | [Detect faces in Vision Studio](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/04-face.html) | [Read text in Vision Studio](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/05-ocr.html) | [Analyze images in Vision Studio](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/03-image-analysis.html) |


# 1 - Criando um recurso 

1.1 - Na barra lateral, clique em **Criar um recurso**. Em **Categorias**, selecione **IA + Machine Learning** e, em seguida, clique no botão **Criar**.

![1](https://github.com/GustavoBCode/Reconhecimento-Facial-e-transformacao-de-imagens-em-Dados-no-Azure-ML/assets/146696103/be1d3df1-d966-464a-8bfb-88bbc9b8ccb9)


1.2 - Se você ainda não tiver um **Grupo de Recursos**, clique em **Criar Novo** e dê o nome de **LABAI-900**. No campo **Nome**, insira **visualstudioai900**. No campo **Tipo de Preço**, selecione **Standard S0**. Marque a caixa de seleção. Agora clique em **Examinar + criar**.

![2](https://github.com/GustavoBCode/Reconhecimento-Facial-e-transformacao-de-imagens-em-Dados-no-Azure-ML/assets/146696103/2c47b426-5e46-4805-a89e-4e572322f54f)

1.3 - Para finalizar esse processo, clique em **Criar**.

![3](https://github.com/GustavoBCode/Reconhecimento-Facial-e-transformacao-de-imagens-em-Dados-no-Azure-ML/assets/146696103/ca56845d-001d-4eaa-8c30-9553c6d8ebc0)

# 2 - Selecionando recurso

2.1 - Abra o [Vision Studio](https://portal.vision.cognitive.azure.com/gallery/featured). Na tela inicial, clique em **View all resources**.

![4](https://github.com/GustavoBCode/Reconhecimento-Facial-e-transformacao-de-imagens-em-Dados-no-Azure-ML/assets/146696103/38a337fb-7e2d-435b-a839-edeff0ca1698)

2.2 - Selecione o **visualstudioai900**. Clique em **Select as default resource**. Em seguida, clique no **X** para fechar.

![5](https://github.com/GustavoBCode/Reconhecimento-Facial-e-transformacao-de-imagens-em-Dados-no-Azure-ML/assets/146696103/e73cb837-eab1-4131-ad2f-e01bd0dd88a8)

# 3 - Detectar faces em imagens

3.1 - Clique em **Face**, e então clique em **Detect faces an image**.

![6](https://github.com/GustavoBCode/Reconhecimento-Facial-e-transformacao-de-imagens-em-Dados-no-Azure-ML/assets/146696103/cf33bec8-167c-4f74-bb67-13b178aa6c85)

3.2 - Em **Try it out**, marque a caixa de seleção. Selecione uma imagem em seus arquivos e clique em **Browse for a file**. No campo **Detected attributes**, será exibida uma descrição da imagem.

![7](https://github.com/GustavoBCode/Reconhecimento-Facial-e-transformacao-de-imagens-em-Dados-no-Azure-ML/assets/146696103/a8604267-02ff-42e5-a118-fdfa99260aaf)

# 4 - Extrair texto de imagens

4.1 - Clique em **Optical character recognition**, e em seguida clique em **Extract text from imagens**.

![8](https://github.com/GustavoBCode/Reconhecimento-Facial-e-transformacao-de-imagens-em-Dados-no-Azure-ML/assets/146696103/449d8ca5-18ce-4dac-aaf3-529d4566cb3a)

4.2 - Selecione uma imagem em seus arquivos, clique em **Browse for a file**. No campo **Detected attributes**, serão exibidas as palavras que estão na imagem.

![9](https://github.com/GustavoBCode/Reconhecimento-Facial-e-transformacao-de-imagens-em-Dados-no-Azure-ML/assets/146696103/8163cfb5-143a-452b-bb4a-29a55e72d442)

# 5 - Adicionar legendas a imagens

5.1 - Clique em **Image analysis**, e em seguida clique em **Add captions to images**.

![10](https://github.com/GustavoBCode/Reconhecimento-Facial-e-transformacao-de-imagens-em-Dados-no-Azure-ML/assets/146696103/2dcebcec-e578-425d-ae82-ac91c73d18f6)

5.2 - Selecione uma imagem em seus arquivos, clique em **Browse for a file**. No campo **Detected attributes**, será descrito o conteúdo da imagem.

![11](https://github.com/GustavoBCode/Reconhecimento-Facial-e-transformacao-de-imagens-em-Dados-no-Azure-ML/assets/146696103/f7c361ed-8209-44c8-8dd2-c717669a3387)

