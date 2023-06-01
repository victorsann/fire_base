<div align="center">
  <img src="">
</div>
<br>

<img src="https://img.shields.io/badge/Firebase-F6C915?style=for-the-badge&logo=firebase&logoColor=black"/>

<h2>Google Analytics</h2>

O Google Analytics é uma solução de medida que provê insights sobre o uso e o engajamento de um app. Com o intuito de auxiliar no entendimento de comportamentos do usuário, permite que decisões sejam tomadas com base nas necessidades que tais comportamentos demonstram.

<h3>Como funciona ?</h3>

O firebase SDK captura automaticamente números sobre sua aplicação, mas como o Analytics, é possível criar [eventos](https://support.google.com/firebase/answer/9234069?visit_id=638212277264765325-3351094573&rd=1) de acordo com o que mais interessa para determinado negócio. Uma vez que as informações são obtidas, estas são dispinibilizadas em um dashboard do Firebase Console. Nele há detalhes sobre as informações resultantes, como por exemplo, o número de usuários ativos e a demografia de uso do seu app.

<h3>Quickstart</h3>

Este quickstart demonstra como adicionar o Google Analytics ao seu projeto e como iniciar a registrar eventos.

Antes de instalar qualquer recurso, é importante entender quais os tipos de informações que o SDK é capaz de registrar:

- <b>Events</b>: Eventos registam as ações do usuário na aplicação, como quais telas e recusros acessou. Além disso, pode registrar eventos do sistema e também erros.
- <b>User properties</b>: As propriedades do usuário corresponde ao seguimento de informação relevante para o seu negócio que pode ser provida pela cliente, como preferências linguísticas e localização geográfica.

O Analytics automaticamente registra alguns [events](https://support.google.com/firebase/answer/9234069?visit_id=638212277264765325-3351094573&rd=1) e [user properties](https://support.google.com/firebase/answer/6317486), não sendo necessário criar uma funcionalidade no seu sistema para tal.

<h3>Antes de iniciar</h3>

- Instale `[firebase_core](https://firebase.google.com/docs/flutter/setup)` e adicione o código de inicialização ao seu app se não o tiver feito.
- Adicione seu app a um projeto no [Firebase Console](https://console.firebase.google.com/?_gl=1*1etj5gf*_ga*MTUwMzYzMzQ2OS4xNjU2OTYwMDM2*_ga_CW55HF8NVT*MTY4NTYyNzAzOS4xMy4xLjE2ODU2MzA4ODYuMC4wLjA.)

<h3>Adicione o Analytics ao seu app</h3>

1 - Da raiz do seu app Flutter, execute o seguinte comando para instalar o plugin:

    flutter pub add firebase_analytics

2 - Uma vez que o pluging foi instalado, faça um rebuild da aplicação:

    flutter run

3 - Uma vez instalado é possível acessar o `firebase_analytics` ao importa-lo da seguinte forma:

    import 'package:firebase_analytics/firebase_analytics.dart';

4 - Para iniciar seu uso, crie uma instância do Firebase Analytics chamando o getter `instance` no `FirebaseAnalytics`:

    FirebaseAnalytics analytics = FirebaseAnalytics.instance;
