---
title: Monitorando serviços de terceiros usando o Slack
layout: post
date: '2017-04-04 16:51:16 -0300'
permalink: monitorando-servicos-de-terceiros-usando-o-slack-8cc8cbdca62f
categories: [Monitoring, Slack, DevOps]
---

![Meu canal #status-page no Slack](/uploads/1*ZbaDdPv6w8WQTxKtttFssw.png)

No nosso dia a dia de desenvolvimento usamos diversos serviços que vão do versionamento do código, a plataformas de hospedagem, além das suítes para escritório e de armazenamento de arquivos. Muitas vezes estes serviços por diversos motivos podem ficar instáveis ou até mesmo indisponíveis.

Uma de nossas primeiras ações nestas situações é correr às redes sociais para ver se algo está sendo reportado, ou procurar pelas páginas de *status* desses serviços.

## Serviços de status

As páginas de status normalmente contêm um histórico de incidentes, histórico de status (está disponível, com interrupção ou indisponível) além do *status* atual da serviço.

Temos disponíveis diversos serviços que provêm paginas de status, e vários destes possuem *feeds* [RSS](https://pt.wikipedia.org/wiki/RSS){:target="_blank"} com as atualizações. Destaco alguns deles que já usei ou testei em alguns projetos que participei: [Cachet](https://cachethq.io/){:target="_blank"}, [Site24x7](https://www.site24x7.com/){:target="_blank"}, [SorryApp](https://www.sorryapp.com/){:target="_blank"}, [Status](https://status.io/){:target="_blank"} e o [StatusPage](https://www.statuspage.io/){:target="_blank"}.

![Minha página de status (status.magnobiet.com) usando o serviço do Site24x7 da Zoho](/uploads/1*3kbrt55KjOzIkZ9ZuFQWUg.png)

## Como fazer?

Monitorar os diversos serviços que usamos no dia a dia pode ser uma tarefa cansativa se ficarmos acessando cada página de *status* de todos estes serviços. Para facilitar o monitoramento destes serviços podemos usar o [Slack](https://medium.com/@slackhq){:target="_blank"} a nosso favor.

Recomendo criar um novo canal para concentrar estas notificações para não poluir os canais de comunicação de sua equipe.

Se precisar de mais informações sobre a criação de canais abaixo deixei o *link* do Help Center do [Slack](https://medium.com/@slackhq){:target="_blank"}.

[https://get.slack.help/hc/en-us/articles/201402297-Create-a-channel](https://get.slack.help/hc/en-us/articles/201402297-Create-a-channel){:target="_blank"}

Com um canal especifico para receber estas notificações, basta adicionar a integração dos *feeds* RSS neste canal. Deixo *link* da documentação do Slack caso não saiba como fazer uma integração.

[https://get.slack.help/hc/en-us/articles/218688467-Add-RSS-feeds-to-Slack](https://get.slack.help/hc/en-us/articles/218688467-Add-RSS-feeds-to-Slack){:target="_blank"}

A partir de agora toda vez que algum destes *feeds* receber alguma atualização você receberá uma notificação diretamente neste canal.

Deixo uma lista com alguns *feeds* de serviços que podem ser úteis.

- [BitBucket](https://status.bitbucket.org/history.rss){:target="_blank"}
- [CloudFlare](https://www.cloudflarestatus.com/history.rss){:target="_blank"}
- [G Suite](https://www.google.com/appsstatus/rss/en){:target="_blank"}
- [GitHub](https://status.github.com/messages.rss){:target="_blank"}
- [Heroku](https://status.heroku.com/feed){:target="_blank"}
- [KingHost](http://status.kinghost.net.br/history.rss){:target="_blank"}
- [Locaweb](https://statusblog.locaweb.com.br/feed){:target="_blank"}
- [Medium](https://medium.statuspage.io/history.rss){:target="_blank"}
- [New Relic](https://status.newrelic.com/history.rss){:target="_blank"}
- [OpenShift](https://status.openshift.com/history.rss){:target="_blank"}
- [Pingdom](http://status.pingdom.com/history.rss){:target="_blank"}
- [Pusher](https://status.pusher.com/history.rss){:target="_blank"}
- [Rollbar](http://status.rollbar.com/history.rss){:target="_blank"}
- [Runscope](https://runscope.statuspage.io/history.rss){:target="_blank"}
- [Trello](http://www.trellostatus.com/history.rss){:target="_blank"}
- [Twilio](https://status.twilio.com/history.rss){:target="_blank"}
- [Twitter](http://status.twitterstat.us/pages/564314ae3309c22c3b0002fa/rss){:target="_blank"}

O AWS da Amazon é um pouquinho mais complicado, pois eles possuem centenas de *feeds* divididos por região e serviço. Através da página [https://status.aws.amazon.com/](https://status.aws.amazon.com/){:target="_blank"} é possível selecionar a região e serviço que deseja acompanhar o *status* e adicionar ao seu canal no [Slack](https://medium.com/@slackhq){:target="_blank"}.

---

Espero que esta dica tenha sido útil a você e sua equipe.
