# Deteção de objetos em tempo real com Tensorflow js

Programando redes neurais com Tensorflow JS e ML5

![Detecção de objetos em tempo real](./ml.gif)

## Vamos começar!

Essas instruções fornecerão uma cópia do projeto em execução na sua máquina local, para fins de desenvolvimento e teste. Consulte me  para obter notas sobre como implantar o projeto em produção.

### Pré-requisitos

O que você precisa para instalar o software e como instalá-lo

```
npm
node.js ^12.16.3
```

### Instalação

```
git clone https://github.com/alessandroprudencio/Machine-Learning.git
```

```
cd Machine-Learning 
```

```
npm install
```

```
npm start
```

Pronto sua aplicação estará  rodando no endereço http://localhost:3000.
___

# API endpoints

## http://localhost:3000/automatic

Modelo de detecção de objetos que visa localizar e identificar vários objetos em uma única imagem ou video.

Este modelo é uma porta TensorFlow.js do modelo COCO-SSD. Para obter mais informações sobre a API de detecção de objetos do Tensorflow, consulte este leia-me em https://github.com/tensorflow/models/blob/master/research/object_detection/README.md.

Este modelo detecta objetos definidos no conjunto de dados COCO, que é um conjunto de dados de detecção, segmentação e legenda de objetos em larga escala. Você pode encontrar mais informações aqui . O modelo é capaz de detectar 90 classes de objetos .

Para testar basta colocar em frente  a camera do dispositvo qualquer objeto que ele indentificara.


## http://localhost:3000/manual
   
Nesta rota sera exibida uma pagina html aonde pedira permissão de acesso a sua camera, é necessario permitir, pois as imagens captadas pela camera sera usada para as entradas.

Nesta rota voce tera a capacidade de criar seu modelo e treina lo.

Tera 3 botoes garrafas, perfume e foto celular, ao clicar em cada um desses opçoes sera "tirada" foto do video em tempo real, que automaticamente é salva em uma variavel no projeto. contudo para que o algoritmo indentifique que é uma garrafa precisamos mostrar isto a ele, então,por exemplo para treinar as fotos de garrafas devera fazer o seguinte, posicione a garrafa em frente a camera do seu dispositivo e clique no botão garrafas, cada clique é como se fosse um foto da tela ao vivo, ou seja tire fotos  da garrafa de varios angulos.Faça isso para os outros botões.Ao finalizar clique no botão treinar  e pronto seu algoritmo de ml estara pronto, para testar bastas colocar os objetos em frente a camera e ver o resultado logo abaixo...

Foi utilizado o Transfer Learning permitindo extrair recursos de uma imagem por meio de um modelo pré-treinado e treiná-lo novamente com novos dados.


___

## Construído com

* [TensorFlow.js ](https://www.tensorflow.org/js)
* [Node JS](https://nodejs.org/)
* [ML5.js](https://ml5js.org/)

## Contribuição

Faça um Fork do projeto
Crie uma Branch para sua Feature (git checkout -b feature/FeatureIncrivel)
Adicione suas mudanças (git add .)
Comite suas mudanças (git commit -m 'Adicionando uma Feature incrível!)
Faça o Push da Branch (git push origin feature/FeatureIncrivel)
Abra um Pull Request

## Author

* Alessandro Prudencio 
* alessandroconectado@gmail.com
* +55 (67) 99269-6705
* [Linkedin](https://www.linkedin.com/in/alessandro-prudencio/)


