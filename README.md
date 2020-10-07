# TCC-Melanoma

Trabalho de Conclusão de Curso sobre Análise de Imagens Dermatoscópicas

Esse trabalho tem como objetivo criar uma rede convolucional capaz de analisar imagens dermatoscópicas e avaliar se a imagem em questão é de um cancêr melanoma do tipo benigno ou maligno.

Abaixo estarei explicando o que cada um dos scripts fazem:

1 - Imagens: esse script baixa as imagens dermatoscópicas do site da ISIC (um instituto que estuda o cancêr de pele). Esse é o dataset desse projeto.

2 - copyimages: script responsável por separar 70% das imagens para treinamento e 30% das imagens para testes.

3 - smote: técnica utilizada para balanceamento do dataset, porém descobrimos que ela não é adequada para datasets de imagens. Esse script foi um teste, ele acabou não sendo utilizado no modelo final.

4 - Flip: técnica que consiste em virar as imagens para que dessa forma novas imagens sejam criadas e assim balancear o dataset. Esse foi um outro experimento que acabou não sendo utilizado no modelo final.

5 - TCC_Melanoma: script com a criação do modelo final.

6 - Grad_CAM: script com a função de criar mapas de calor, com isso mostrar como que o modelo aprendeu a avaliar imagens benignas e malignas. Essa técnica não foi implementada 100%, para algumas imagens o mapa de calor é gerado, mas para a grande maioria delas acontece um erro onde não é possível a criação do mapa de calor. Esse script precisa ser aperfeiçoado.
