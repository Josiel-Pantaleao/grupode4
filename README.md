# Detecção de Placas de Veículos Utilizando YOLOv8


**Arthur Jung Barreto**

Universidade Federal de Goiás
jung@discente.ufg.br


**Gabriel Henrique Barcelos**

Universidade Federal de Goiás

gabriel.barcelos@discente.ufg.br


**Josiel Pantaleao Cardoso Silva**

Universidade Federal de Goiás

josielpantaleao@discente.ufg.br


**Julierme Augusto Alves**

Universidade Federal de Goiás

julierme.alves@discente.ufg.br


**Paulo Victor Brandao Faria Borges**

Universidade Federal de Goiás

paulobrandao@discente.ufg.br


Resumo

Este seminário abordará a relevância do reconhecimento de placas de carro na visão computacional, destacando aplicações vitais como segurança, controle de tráfego, estacionamentos inteligentes e cidades inteligentes. A proposta de solução combina a eficiência do algoritmo YOLO com a análise das Transformadas de Fourier para aprimorar detecção e classificação de placas. O processo envolve pré-processamento com Transformadas de Fourier para identificar padrões e texturas, seguido por segmentação de caracteres e reconhecimento com redes neurais.

Introdução

O reconhecimento de placas de carro é um desafio importante na área de visão computacional e tem uma ampla gama de aplicações práticas, incluindo:

1\. Segurança e Vigilância - Identificação de veículos em áreas de acesso restrito, detecção de veículos roubados ou suspeitos em tempo real.

2\. Controle de Tráfego - Monitoramento de fluxo de veículos, detecção de violações de trânsito (por exemplo, semáforos e limites de velocidade).

3\. Estacionamentos Inteligentes - Registro automático de entrada e saída de veículos em estacionamentos, facilitando o controle e pagamento.

4\. Monitoramento de Cidades Inteligentes - Coleta de dados sobre tráfego para otimização urbana e planejamento de infraestrutura.

Contexto e Motivação

O reconhecimento de placas de carro é um problema desafiador e de grande importância na área de visão computacional. Com o aumento constante do número de veículos nas estradas e o crescimento das cidades, há uma demanda crescente por sistemas de monitoramento e controle de tráfego eficazes. Além disso, a segurança pública e a aplicação da lei se beneficiam da capacidade de identificar e rastrear veículos.

Desafios do Reconhecimento de Placas: O problema de reconhecimento de placas de carro apresenta diversos desafios devido à natureza variável e complexa das cenas de trânsito. Alguns dos principais desafios incluem:

Variações na Iluminação: As condições de iluminação podem variar amplamente, resultando em placas mal iluminadas, sombras e reflexos que afetam a detecção e leitura.

Oclusões e Obstruções: As placas podem ser parcialmente ocluídas por outros veículos, objetos ou obstáculos, dificultando sua detecção completa.

Distorção Geométrica: As placas podem estar em ângulos diferentes, distorcidas ou inclinadas, o que afeta a precisão da detecção e do reconhecimento.

Variações de Fundo: As placas podem estar localizadas em fundos complexos, como áreas urbanas movimentadas ou estradas com paisagens diversas.

Variações de Estilo e Formato: Placas de diferentes países e regiões possuem formatos e estilos variados, incluindo variações na fonte, tamanho e disposição dos caracteres.

Condições Climáticas: Fatores climáticos como chuva, neblina e neve podem reduzir a visibilidade das placas e dificultar a detecção.


Proposta:
Neste relatório, apresentamos uma análise abrangente dos resultados obtidos após o treinamento de um modelo YOLOv8 para o reconhecimento de placas de carros. O modelo foi treinado utilizando o conjunto de dados e a estrutura fornecida pelo Roboflow. O objetivo principal foi avaliar a eficácia do modelo na detecção precisa de placas de carros em imagens e vídeos, com a possibilidade de aplicação em cenários do mundo real.

Métodos:
O modelo YOLOv8 foi escolhido devido à sua eficiência e capacidade de detecção em tempo real. O treinamento foi realizado em um ambiente controlado, com um total de 4 horas de processamento. Utilizamos um conjunto de dados diversificado, contendo imagens e vídeos de diferentes ângulos, condições de iluminação e fundos para garantir a robustez do modelo. Durante o treinamento, utilizamos uma taxa de aprendizado adaptativa e um batch size otimizado para maximizar a convergência do modelo.

Resultados:
Após o treinamento de 4 horas, o modelo YOLOv8 demonstrou resultados promissores. A precisão da detecção de placas de carros atingiu uma média de [89%] nas imagens de teste e [78%] nos vídeos de teste. Observamos que o modelo conseguiu detectar placas de carros em diferentes condições de iluminação, distâncias e ângulos, o que indica sua capacidade de generalização.

Testes em Vídeos e Imagens:
Para avaliar a robustez do modelo, realizamos testes em uma variedade de vídeos e imagens de diferentes cenários. O modelo conseguiu detectar corretamente placas de carros em cenas urbanas, estradas, estacionamentos e ambientes de baixa visibilidade. A taxa de falsos positivos foi mantida em um nível aceitável, demonstrando a eficácia do modelo em distinguir entre placas de carros reais e objetos semelhantes.

Aplicação em Tempo Real:
Com base nos resultados obtidos, estamos confiantes de que o modelo YOLOv8 pode ser aplicado com sucesso em cenários do mundo real que exigem detecção de placas de carros em tempo real. A arquitetura eficiente do modelo permitirá sua implementação em sistemas de vigilância de tráfego, monitoramento de estacionamentos, controle de acesso e muito mais.

Problemas: Decidimos inicialmente considerar o uso da Transformada de Fourier para identificar placas de carros em imagens. No entanto, após análises mais detalhadas, descobrimos que essa abordagem não seria eficaz devido às complexas características espaciais das placas, como formas e padrões de letras/números, além das variações de tamanho, orientação e iluminação. Devido a essas limitações, optamos por não seguir com a Transformada de Fourier e, em vez disso, escolhemos abordagens avançadas de processamento de imagem e aprendizado de máquina, como redes neurais convolucionais, que podem capturar diretamente as características das placas e oferecer uma identificação mais precisa e confiável, adaptada a diversos cenários e condições.

Conclusão:
O treinamento e teste do modelo YOLOv8 para reconhecimento de placas de carros resultaram em desempenho consistente e promissor. Os resultados obtidos nas imagens e vídeos de teste demonstram a capacidade do modelo em lidar com uma variedade de situações do mundo real. Recomendamos a consideração deste modelo para aplicações práticas que envolvam a detecção de placas de carros em tempo real, dada sua precisão e eficiência.

Próximos Passos:
À medida que continuamos a desenvolver essa solução, pretendemos explorar a possibilidade de melhorar ainda mais o desempenho do modelo por meio de ajustes finos e expansão do conjunto de dados. Além disso, consideraremos a integração do modelo em um sistema de processamento em tempo real para validação em ambientes do mundo real.

Agradecemos a oportunidade de conduzir esse projeto e estamos à disposição para quaisquer esclarecimentos adicionais.


Referências Bibliográficas

`   `- Artigo: "Vehicle License Plate Recognition Using Deep Learning" (Disponível em: [Link](https://www.researchgate.net/publication/338498036))

`   `- Tutorial: "License Plate Recognition with OpenALPR and YOLO" (Disponível em:[Link](https://www.pyimagesearch.com/2020/09/21/opencv-automatic-license-number-plate-recognition-anpr-with-python/))

`   `- Livro: "Digital Image Processing" por Gonzales & Woods.

`   `- Artigo: "License Plate Recognition using Fourier Transform" (Disponível em:[Link](https://ieeexplore.ieee.org/document/7302206))

 cÓdigo: https://colab.research.google.com/drive/1mzL6WyY9BRx4xX476eQdhKDnd_eixBlG#scrollTo=GNVU7eu9CQj3

 site:  https://roboflow.com/
