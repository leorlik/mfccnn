# ![](https://i.imgur.com/mdYYSwk.jpg)

# Versão em Português

## Redes Convolucionais para Classificação de Áudios

**Dataset analisado:** [Free Spoken Digit Dataset](https://github.com/Jakobovski/free-spoken-digit-dataset)

### Sobre o estudo

Nesse projeto nós analisamos o desempenho de uma adaptação da ResNET, famosa rede convolucional, para classificação dos áudios do Free Spoken Digit Dataset (FSDD).

### Sobre o FSDD

O Free Spoken Digit Dataset é uma base de dados simples de arquivos de áudio .wav de 8kHz. Nele, 6 locutores pronunciaram em inglês os números de 0 a 9 50 vezes cada um, resultando em 500 áudios por locutor, 300 áudios por digito e, portanto, 3000 áudios no total.

### Técnica

A principal técnica utilizada para transformar os arquivos .wav em entradas para a rede neural foram os Mel-frequency cepstral coefficients(MFCCs), uma representação cepstral de um espectro de poder de curta duração de um áudio que é comumente usada nos problemas de reconhecimento de fala.

### Resultados

Nós transformamos os áudios em MFCCs, com algum processamento explicado no código, e treinamos nosso modelo em dois tipos diferentes de divisão treino/validação: sem critério e separando Jackson como locutor separado.

#### Divisão sem critério:

![](https://i.imgur.com/zTvQDTN.png)

#### Divisão em locutor:

![](https://i.imgur.com/o9kp5sl.png)

### Conclusão

Além de avaliar a performance do modelo na classificação de áudios do FSDD, nosso objetivo na elaboração desse repositório foi também mostrar que considerando a divisão sem critério dos conjuntos de treino e validação nosso trabalho beiraria a perfeição, porém em algo mais perto de uma situação real, como é na divisão dos locutores, o modelo não performa como gostaríamos.

Acreditamos que as redes neurais convolucionais podem ser muito úteis ao trabalhar com áudio, porém nossa técnica ainda precisa de muitas melhorias para atingir o ideal.

### Próximos passos

Queremos agora explorar outras técnicas, arquiteturas e modelos para a classificação de áudio na busca de uma abordagem verdadeiramente efetiva para o problema. Algumas das coisas que queremos explorar é o processo de Data Augmentation para áudios e modelos não-relacionados a redes neurais.

### Agradecimentos

Esse projeto foi desenvolvido com o apoio do [Grupo CiDAMO UFPR](http://cidamo.com.br/).

Esse trabalho não teria sido desenvolvido sem a ajuda do Doutorando Paulo Sergio da Conceição Moreira, que não só se disponibilizou para nos ajudar como nos encaminhou ótimos materiais que foram cruciais para o desenvolvimento do projeto.

## Contatos

**Autor:** Leonardo Lima Dionizio

**LinkedIn:** https://www.linkedin.com/in/leonardo-dionizio-5aa4611b3/

**E-mail:** leo.l.dionizio@gmail.com

**Orientador**: Lucas Garcia Pedroso

**LinkedIn:** https://www.linkedin.com/in/lucas-pedroso-14a76a206/

# English Version

## Convolutional Neural Networks for Audio Classification

**Used Dataset:** [Free Spoken Digit Dataset](https://github.com/Jakobovski/free-spoken-digit-dataset)

### About the Study

In this poject we analyse the performance of a ResNET adaptation, a famous convolutional network, to the taks of classify the Free Spoken Digit Dataset (FSDD).

### About the FSDD

The Free Spoken Digit Dataset is a simple data base of 8kHz .wav audio file. In it, six speakers pronounced in english the numbers between 0 and 9 50 times eachs, resulting in 500 audios per speaker, 300 files per digit and, therefore, 3000 audios files in total.

### Technique

The main technique used to transform the .wav files in input for the neural network were the Mel-Frequency Cepstral Coefficients (MFCCs), a cepstral representation of a short-term power spectrum of an audio that's commonly used in speak recognition problems.

### Results

We transformed the audio data into MFCCs, with some pre-processing explaned in the code, and we trained our model in two different train-test sets: without criterion and separating Jackson as a validation speaker.

#### No criterion:

![](https://i.imgur.com/zTvQDTN.png)

#### Speaker division:

![](https://i.imgur.com/o9kp5sl.png)

### Conclusion

Besides evaluate the model performance in the FSDD audio classification, our objective in this work elaboration was also to show how the right train-test split can influence the model and perhaps leads to wrong conclusions.

We believe that the convolutional neural networks can be very usefull to work with audios, but our technique still needs a lot of improvements to reach the ideal performance.

### Next Steps

We want to explore another techniques, architectures and models to audio classification in the search of a truthfully effective approach to the problem. Something that we want to explore is Data Augmentation for audios and non-neural networks models.

### Special Thanks


This project was developed with the support of the [Grupo CiDAMO UFPR](http://cidamo.com.br/).

This work wouldn't be possible if it were developed without the help of Paulo Sergio da Conceição Moreira, who not only made himself available to help us but sent us great material that were crucial to the project development.



## Referências/References

K. Sreenivasa Rao and K. E. Manjunath. 2017. Speech Recognition Using Articulatory and Excitation Source Features (1st. ed.). Springer Publishing Company, Incorporated.

W. Junqin and Y. Junjun, "An improved arithmetic of MFCC in speech recognition system," 2011 International Conference on Electronics, Communications and Control (ICECC), 2011, pp. 719-722, doi: 10.1109/ICECC.2011.6066676.

Y. Wang and B. Lawlor, "Speaker recognition based on MFCC and BP neural networks," 2017 28th Irish Signals and Systems Conference (ISSC), 2017, pp. 1-4, doi: 10.1109/ISSC.2017.7983644.



