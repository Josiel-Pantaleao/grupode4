Participantes

ARTHUR JUNG BARRETO – 202105833

Paulo Victor Brandão – 202105862

GABRIEL HENRIQUE BARCELOS – 202005476

JULIERME AUGUSTO ALVES – 202005491

Josiel Pantaleão Cardoso Silva – 202010404

Email: <josielpantaleao123@gmail.com>


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

Proposta de Solução

Nossa abordagem para o reconhecimento de placas de carro combina a eficiência do algoritmo YOLO (You Only Look Once) com a poderosa análise das Transformadas de Fourier para melhorar a detecção e a classificação das placas.


Detecção Inicial com YOLO

Utilizaremos a arquitetura YOLO para detectar a presença de placas de carro nas imagens. O YOLO é escolhido devido à sua capacidade de detecção em tempo real e eficiência.


Planejamento Fantasma:

Pré-processamento e Ajuste com Transformadas de Fourier

`   `- Após a detecção da placa, extraia a região correspondente da imagem original.

`   `- Aplique as Transformadas de Fourier nessa região para converter o domínio espacial em domínio de frequência.

`   `- Identifique as frequências significativas que representam padrões e texturas do texto da placa.

`   `- Realce essas frequências e reverta a transformada para obter a informação aprimorada da placa.

Pós-processamento e Classificação

`   `- Com a imagem da placa aprimorada, execute a segmentação de caracteres usando técnicas de processamento de imagem, como binarização e detecção de contornos.

`   `- Use uma rede neural treinada para reconhecimento de caracteres (CNN ou RNN) para classificar cada caractere segmentado.

`   `- Monte a sequência de caracteres reconhecidos para formar o texto da placa.

Avaliação e Otimização

`   `- Avalie o desempenho do sistema usando métricas apropriadas, comparando as detecções e reconhecimentos obtidos com as informações reais.

`   `- Otimize os hiperparâmetros do modelo YOLO, das redes neurais de reconhecimento de caracteres e de quaisquer outras partes do sistema.

`   `- Realize ajustes de limiares e parâmetros de pós-processamento para encontrar um equilíbrio entre sensibilidade (recall) e precisão

`  `Referências para Transformadas de Fourier:

Pós-processamento e Classificação

Com as informações das Transformadas de Fourier, aplicaremos um algoritmo de reconhecimento de caracteres para interpretar o texto da placa. Isso nos permitirá identificar o veículo com base na placa.


Outras Abordagens

Além das Transformadas de Fourier, existem outras maneiras de aprimorar a tarefa de reconhecimento de placas:

Aprendizado de Pós-processamento Utilizar algoritmos de aprendizado profundo, como redes neurais recorrentes (RNNs) ou transformers, para melhorar a classificação de caracteres nas placas.

Aumento de Dados Utilizar técnicas de aumento de dados para criar variações realistas no conjunto de treinamento, melhorando a robustez do modelo.

Pós-processamento de Texto Aplicar técnicas de processamento de linguagem natural para corrigir possíveis erros de reconhecimento de caracteres.

Benefícios e Impacto:

Uma solução eficaz para o reconhecimento de placas de carro tem o potencial de melhorar significativamente a segurança rodoviária, o controle de tráfego e a aplicação da lei. Além disso, essa tecnologia pode ser integrada a sistemas de estacionamento inteligente, cidades inteligentes e monitoramento de tráfego, contribuindo para a otimização das operações urbanas e do transporte.

Conclusão

O problema de reconhecimento de placas de carro é complexo devido às várias variações e desafios que as imagens de trânsito apresentam. No entanto, nossa abordagem que combina YOLO e Transformadas de Fourier visa superar esses obstáculos, fornecendo uma solução robusta e eficaz para a detecção e reconhecimento de placas de carro, com aplicações práticas em segurança, tráfego e infraestrutura urbana.

































Referências Bibliográficas

`   `- Artigo: "Vehicle License Plate Recognition Using Deep Learning" (Disponível em: [Link](https://www.researchgate.net/publication/338498036))

`   `- Tutorial: "License Plate Recognition with OpenALPR and YOLO" (Disponível em:[Link](https://www.pyimagesearch.com/2020/09/21/opencv-automatic-license-number-plate-recognition-anpr-with-python/))

`   `- Livro: "Digital Image Processing" por Gonzales & Woods.

`   `- Artigo: "License Plate Recognition using Fourier Transform" (Disponível em:[Link](https://ieeexplore.ieee.org/document/7302206))

