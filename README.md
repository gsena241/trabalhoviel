Conversão de imagem RGB em imagem Grayscale:

No começo do código são importadas as bibliotecas cv2(Open CV), a numply, nomeada como ‘np”, a matplotlib.pyplot, nomeada como ptl e a cv2_imshow, importada do google.colab.patches.
Posteriormente, utilizando o código cv2.imread(), lê-se a imagem que será armazenada na variável img. Logo depois utiliza-se a função cv2_imshow(img), que abre uma nova janela onde é mostrada a variável “img” em imagem. Depois, a imagem colorida é separada em canais de cores (R, G, B) usando a função cv2.split(). Após isso é feito a ponderação dos canais de cor para converter a imagem colorida em escala cinza ponderada, nela os valores R, G, B são multiplicados, respectivamente, pelos coeficientes 0.299, 0.587 e 0.114 e são somados. O resultado da operação é armazenado na variável img_grayscale_pondered. Usando novamente a função cv2_imshow() é mostrada a imagem resultante da operação.

Transformações:

Na primeira linha, a variável recebe o valor 1, onde basta receber o valor 0 para mudar para escala cinza. Novamente, é utilizado a função cv2.imread para ler a imagem onde é armazenado na variável img_in. Na terceira linha, cria-se a variável img_out e recebe o resultado da operação de 255 - img_in. A operação anterior subtrai cada pixel da imagem de 255 afim de obter o valor negativo, consequentemente a imagem negativa. É usado o cv2_imshow(img_in) para mostrar a imagem original da variável img_in, na linha posterior é usado o mesmo comando para mostrar a imagem processada da variável img_out.

O primeiro comando, cv2.imread, usado para ler a imagem e armazená-la na variável img_in. Em seguida são criadas duas váriveis, 'a' que recebe -1 e 'b' que recebe 1, assim alterando o contraste e o brilho respectivamente. Na linha posterior, a variável 'a' é multiplicada por img_in e, depois, o variável 'b' é somada ao resultado com a finalidade de ajustar a intensidade da transformação. O resultado, a imagem, é armazenado na variável img_out. Na quinta linha a imagem da variável img_out é convertida para uma matriz da bliblioteca NumPy, utilizando o comando np.array. A sexta apresenta a imagem original e a sétima a imagem alterada.

Filtro Especial:

Na primeira linha, a imagem é lida e armazenada na variável img_in. Na segunda linha, nessa linha é criada uma matriz de 5x5 e usa-se Kernel em uma imagem, onde o cálculo servirá para a suavização da imagem. A quarta apresenta a imagem original e a quinta a imagem alterada.

Gustavo Sena Vieira.

David Smith Souza.
