---
title: Monitorando serviços de terceiros usando o Slack
layout: post
date: '2017-04-04 16:51:16 -0300'
permalink: monitorando-servicos-de-terceiros-usando-o-slack-8cc8cbdca62f
categories: monitoring slack devops
---

![Meu canal #status-page no Slack](/uploads/1*ZbaDdPv6w8WQTxKtttFssw.png)

No nosso dia a dia de desenvolvimento usamos diversos serviços que vão do versionamento do código, a plataformas de hospedagem, além das suítes para escritório e de armazenamento de arquivos. Muitas vezes estes serviços por diversos motivos podem ficar instáveis ou até mesmo indisponíveis.

Uma de nossas primeiras ações nestas situações é correr às redes sociais para ver se algo está sendo reportado, ou procurar pelas páginas de *status* desses serviços.

## Serviços de status

As páginas de status normalmente contêm um histórico de incidentes, histórico de status (está disponível, com interrupção ou indisponível) além do *status* atual da serviço.

Temos disponíveis diversos serviços que provêm paginas de status, e vários destes possuem *feeds* [RSS](https://pt.wikipedia.org/wiki/RSS) com as atualizações. Destaco alguns deles que já usei ou testei em alguns projetos que participei: [Cachet](https://cachethq.io/), [Site24x7](https://www.site24x7.com/), [SorryApp](https://www.sorryapp.com/), [Status](https://status.io/) e o [StatusPage](https://www.statuspage.io/).

![Minha página de status (status.magnobiet.com) usando o serviço do Site24x7 da Zoho](/uploads/1*3kbrt55KjOzIkZ9ZuFQWUg.png)

## Como fazer?

Monitorar os diversos serviços que usamos no dia a dia pode ser uma tarefa cansativa se ficarmos acessando cada página de *status* de todos estes serviços. Para facilitar o monitoramento destes serviços podemos usar o [Slack](https://medium.com/@slackhq) a nosso favor.

Recomendo criar um novo canal para concentrar estas notificações para não poluir os canais de comunicação de sua equipe.

Se precisar de mais informações sobre a criação de canais abaixo deixei o *link* do Help Center do [Slack](https://medium.com/@slackhq).

[https://get.slack.help/hc/en-us/articles/201402297-Create-a-channel](https://get.slack.help/hc/en-us/articles/201402297-Create-a-channel)

Com um canal especifico para receber estas notificações, basta adicionar a integração dos *feeds* RSS neste canal. Deixo *link* da documentação do Slack caso não saiba como fazer uma integração.

[https://get.slack.help/hc/en-us/articles/218688467-Add-RSS-feeds-to-Slack](https://get.slack.help/hc/en-us/articles/218688467-Add-RSS-feeds-to-Slack)

A partir de agora toda vez que algum destes *feeds* receber alguma atualização você receberá uma notificação diretamente neste canal.

Deixo uma lista com alguns *feeds* de serviços que podem ser úteis.

- [BitBucket](https://status.bitbucket.org/history.rss)
- [CloudFlare](https://www.cloudflarestatus.com/history.rss)
- [G Suite](https://www.google.com/appsstatus/rss/en)
- [GitHub](https://status.github.com/messages.rss)
- [Heroku](https://status.heroku.com/feed)
- [KingHost](http://status.kinghost.net.br/history.rss)
- [Locaweb](https://statusblog.locaweb.com.br/feed)
- [Medium](https://medium.statuspage.io/history.rss)
- [New Relic](https://status.newrelic.com/history.rss)
- [OpenShift](https://status.openshift.com/history.rss)
- [Pingdom](http://status.pingdom.com/history.rss)
- [Pusher](https://status.pusher.com/history.rss)
- [Rollbar](http://status.rollbar.com/history.rss)
- [Runscope](https://runscope.statuspage.io/history.rss)
- [Trello](http://www.trellostatus.com/history.rss)
- [Twilio](https://status.twilio.com/history.rss)
- [Twitter](http://status.twitterstat.us/pages/564314ae3309c22c3b0002fa/rss)

O AWS da Amazon é um pouquinho mais complicado, pois eles possuem centenas de *feeds* divididos por região e serviço. Através da página [https://status.aws.amazon.com/](https://status.aws.amazon.com/) é possível selecionar a região e serviço que deseja acompanhar o *status* e adicionar ao seu canal no [Slack](https://medium.com/@slackhq).

---

Espero que esta dica tenha sido útil a você e sua equipe.