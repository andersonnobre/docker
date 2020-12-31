<h2 align="center"> 01 - Primeiro Desafio Go - Docker Code Education -  </h2>
<p align="center">  
  <img alt="Made by Anderson Nobre" src="https://img.shields.io/badge/Made%20by-Anderson Nobre-%2304D361">

  <img alt="Made with Golang" src="https://img.shields.io/badge/Made%20with-Golang-%1f425f">  

  <img alt="Made with Docker" src="https://img.shields.io/badge/Made%20with-Docker-%1f425f">    

</p>

<h3> Objetivo </h3>
<p> Criar uma image Docker visando atender o desafio baixo: </p>
Esse desafio é muito empolgante principalmente se você nunca trabalhou com a linguagem Go!
Você terá que publicar uma imagem no docker hub. Quando executarmos:

docker run <seu-user>/codeeducation

Temos que ter o seguinte resultado: Code.education Rocks!

Se você perceber, essa imagem apenas realiza um print da mensagem como resultado final, logo, vale a pena dar uma conferida no próprio site da Go Lang para aprender como fazer um "olá mundo".

Lembrando que a Go Lang possui imagens oficiais prontas, vale a pena consultar o Docker Hub.

3) A imagem de nosso projeto Go precisa ter menos de 2MB =)

Dica: No vídeo de introdução sobre o Docker quando falamos sobre o sistema de arquivos em camadas, apresento uma imagem "raiz", talvez seja uma boa utilizá-la.

--------------------------------------------
<h3> Solução </h3>

<h4>Fonte do github</h4>
https://github.com/andersonnobre/docker/tree/master/golang

1- Relizar o build da image: 
docker build -t nobre/codeeducation . </br>
2- Executar docker run --rm -it nobre/codeeducation</br>

<h4>Image no docker hub</h4>
https://hub.docker.com/repository/docker/nobre/codeeducation</br>

<h4>Tamanho</h4>
Reduziu para 1.22MB



