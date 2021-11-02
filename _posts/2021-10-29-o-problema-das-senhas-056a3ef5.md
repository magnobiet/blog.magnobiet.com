---
title: O problema das senhas
layout: post
date: '2021-10-29 17:51:00 -0300'
permalink: o-problema-das-senhas-056a3ef5
categories: [Security, Password]
---

Infelizmente esta cada vez mais comum notícias de vazamento de dados nos últimos anos. Em 2021, por exemplo, foi postado em um forum na Internet uma compilação contendo mais de 8 bilhões de senhas ([rockyou2021.txt](https://cybernews.com/security/rockyou2021-alltime-largest-password-compilation-leaked/)). Senhas como `123456`, `qwerty`, `1q2w3e` infelizmente ainda estão entre as top 10 senha mais comuns, como mostra [este artigo do CyberNews](https://cybernews.com/best-password-managers/most-common-passwords/).

É bem possível que alguma de suas senhas já possa ter sido exporta em algum dos vazamentos que aconteceram nos últimos anos. Existem diversos sites na Internet que compilam estes vazamentos e permitem que qualquer um faça buscas para ver se alguma de suas senhas já foram vazadas.

No site [haveibeenpwned.com](https://haveibeenpwned.com/), por exemplo, é possível informar seu endereço de e-mail ou telefone, e verificar se o mesmo foi exposto em algum vazamento e quais dados relacionados ao vazamento em questão foram vazados.

![Imagem do site Have I Been Pwned mostrando que um endereço de e-mail consta em 13 vazamentos diferentes](./uploads/have-i-been-pwned-check-if-your-email-has-been-compromised-in-a-data-breach.png "Imagem do site Have I Been Pwned mostrando que um endereço de e-mail consta em 13 vazamentos diferentes.")

A Mozilla tem um serviço chamado [Firefox Monitor](https://monitor.firefox.com/) que usa os dados do site [Have I Been Pwned](https://www.haveibeenpwned.com/) para mostrar os vazamentos, e também permite você se cadastrar para receber alertas caso seu e-mail seja relacionado em algum novo vazamento quando ocorrer.

O site [cybernews.com/password-leak-check](http://cybernews.com/password-leak-check/) permite buscas por senhas vazadas, é possível informar uma senha e verificar se a mesma esta em algum vazamento que já se tornou público.

![Imagem do site CyberNews mostrando que a senha `q1w2e3` esta exposta 33.832 vezes em bancos de dados vazados](./uploads/leaked-password-check--has-my-password-been-hacked.png "Imagem do site CyberNews mostrando que a senha `q1w2e3` esta exposta 33.832 vezes em bancos de dados vazados")

## Senhas fracas e repetidas

O problema de usar senhas fracas e comuns, como por exemplo `q1w2e3` é que em caso de vazamentos, um atacante usando um [ataque de força bruta](https://www.kaspersky.com.br/resource-center/definitions/brute-force-attack) pode conseguir facilmente roubar suas contas em sites na Internet. Usar a mesma senha em diversos serviços online também é muito perigoso, pois basta que apenas uma senha vaze para que um atacante tente usar a mesma senha em outros site e ver se consegue acesso.

A melhor forma de se proteger é usar senhas únicas para cada serviço e senhas fortes.

## Minha senha é segura?

Senhas fortes podem ser geradas de diversas formas, cada um pode criar seu próprio algoritmo de como gerar senhas fortes e únicas que apenas você saberá.

Para cada exemplo de senha dos exemplos abaixo, vou usar o site [howsecureismypassword.net](http://howsecureismypassword.net/) para exemplificar quando tempo um computador levaria para descobrir a sua senha em um ataque de força bruta.

Vou usar a sequencia `minhasenha` como exemplo. Bom, usando apenas `minhasenha` como senha, um computador levaria menos de uma hora para descobrir esta senha.

Trocando vogais por números: `m1nh4s3nh4` (1 dia)

Trocando vogais por números e adicionando letras maiúsculas e minúsculas: `M1nh4S3nh4` (7 meses)

Trocando vogais por números e adicionando letras maiúsculas, minúsculas e caracteres especiais: `M1nh4_S3nh4!` (34 mil anos)

Da para perceber que usando a mesma base de senha, mas fazendo algumas substituições relativamente simples podem deixar a senha bem mais segura e difícil de descobrir. Você pode criar seu próprio padrão deixando ainda mais exclusiva e segura sua senha.

Um exemplo bem simples `Minha-Senha-1` levaria aproximadamente 2 milhões de anos para quebrar a senha. Note que ela é bem mais simples de lembrar, contem apenas palavras começando com letras maiúsculas, separado por traços e com um numero no final. Você pode gerar essas senhas com pequena sentença de palavras que so você sabe, ou gerar alguma usando algum site como o [correcthorsebatterystaple.net](http://correcthorsebatterystaple.net/) por exemplo.

Outro fator que ajuda muito a deixar as senhas mais seguras é o tamanho dela, quanto mais caracteres ela tiver, mais tempo demoraria para quebrar a mesma. Pegando o mesmo exemplo acima e fazendo algo como `Minha-Senha-Bem-Segura-1` levaria 1 octilhão de anos para quebrar, por exemplo.

Uma outra estratégia muito boa é gerar senhas aleatórias com mais de 16 caracteres contendo letras maiúsculas e minúsculas, números e caracteres especiais, como por exemplo: `VWN8VHoPUuGhVx,U~Z9T` que levaria quintiliões de anos para quebrar.

É possível gerar essas senhas simplesmente apertando aleatoriamente no teclado (😂) ou usar algum gerador online como por exemplo: [1Password](https://1password.com/pt/password-generator/), [Norton](https://my.norton.com/extspa/passwordmanager?path=pwd-gen), [Avast](https://www.avast.com/pt-br/random-password-generator), entre diversos outros disponíveis.

Tenho quase certeza que chegando até aqui você ja entendeu que ter senhas diferentes e fortes é muito importante, mas também já deve ter percebido um dos grandes problemas de usar senhas fortes, que é lembrar delas. Usar senhas complexas ou aleatória fica impossível de memorizar.

Eu sempre gostei de testar sistemas, redes sociais e plataformas novas em geral pela Internet, hoje para ter uma ideia eu tenho mais de 2.300 senhas, o que é impossível de lembrar.

Como resolver este problema então? Salvar em um arquivo de texto puro e salvar no seu computador, acho que nem precisamos falar dos porquês de não fazer isso.

Eu a mais de 10 anos atras fazia de uma forma "simples", mas que era útil na época, armazenava minhas senhas em uma planilha. Sim, uma boa e velha planilha. Era uma planilha bem simples, contento o nome do serviço, endereço, usuário e senha. É bem óbvio que qualquer um tendo este arquivo em mãos teria acesso a todas as minhas senhas. Então para ter um pouquinho a mais de segurança, o arquivo tinha uma senha para abrir. Este arquivo era armazenado dentro de uma pasta compactada com outra senha diferente, e ficava armazenado em uma pasta oculta do sistema.

Dava um pequeno trabalho para algum invasor achar o arquivo e abrir, mas eras bem possível de isto acontecer caso tivesse o computador invadido.

Não era muito fácil de pegar um senha também para entrar em um site. Precisava abrir a pasta oculta, abrir o arquivo compactado com a senha dele, abrir a planilha com a senha dela, ai então buscar, copiar a senha e colar no sistema para acessar.

Com o passar dos anos e com o advento dos smartphones fica ainda mais inviável manter uma solução arcaica como esta. A mais de uma década atrás até funcionava, mas hoje é um pouco mais complicado fazer assim por diversos fatores.

## Gerenciadores de senhas

Para resolver estes problemas temos no mercado diversas soluções para gerenciamento de senhas. Desde as soluções mais simples que funcionam offline até soluções mais completas que sincronizam entre múltiplos dispositivos que dão suporte a acesso online, via aplicativos para smartphone, aplicativos para computador e até via extensão para navegadores.

Tem soluções muito boas e seguras que são gratuitas até as mais robustas e com mais funcionalidades que custam algumas dezenas de reais ao ano.

Minha migração para gerenciadores de senhas começou migrando elas da minha planilha para o [KeePass](https://keepass.info/). Uma aplicação de computador e com opções de aplicativos para celular. Com o passar do tempo o KeePass ficou meio parado e migrei para o [KeePassXC](https://keepassxc.org/) que é uma ramificação do KeePass original mas que é guiada pela comunidade e que esta com mais evoluções e com uma interface mais moderna.

O [KeePassXC](https://keepassxc.org/) é uma solução offline, ou seja, ele gera um arquivo criptografado no seu dispositivo que so pode ser acessado com sua senha mestre (gerada durante a criação do seu arquivo cofre). No meu caso caso durante a geração do arquivo cofre também gerei um arquivo chave complementar, o que significa que para acessar o meu cofre é necessário a minha senha e meu arquivo chave, o que gera uma segunda camada de proteção. O KeePass também permite que além da senha mestre e do arquivo chave você usa alguma chave de criptografia via hardware para gerar mais uma camada de proteção para o seu arquivo.

É uma ótima solução para quem quer começar a armazenar suas senhas de forma mais segura e sem custo algum. Ele tem suporte também a extensões para navegador que ajudam a auto completar o preenchimento dos formulários em sites.

O problema que por ele ser uma solução offline, para ter acesso as senhas no smartphone por exemplo, era preciso enviar o arquivo para uma plataforma de armazenamento em nuvem e ficar sincronizando entre os dispositivos a cada atualização das senhas.

Por segurança o arquivo do cofre eu armazenava em uma plataforma e o arquivo de chave em outra, o que me gerava uma certa complexidade para gerenciar.

Até hoje eu uso o KeePassXC mas para senhas relacionadas ao trabalho e a clientes. Mas para simplificar o gerenciamento das minhas senhas de uso pessoal comecei a pesquisar por soluções que trabalham de forma online.

Após algumas pesquisas e testes acabei migrando para o 1Password, uma solução robusta com diversas funcionalidades como suporte as plataformas (Windows, Linux, macOS, Android, iOS e Chrome OS) além das extensões para todos os principais navegadores (Chrome, Firefox, Edge, Brave, Safari), suporte a autenticação de múltiplo fator, armazenamento de arquivos de forma segura entre diversas outras. Mas todas estas comodidades e seguranças tem um custo que começa em $2,99 por mês (que na conversão atual do dólar custa mais de R$ 200,00 por ano).

No 1Password, além da senha do cofre que da acesso a tudo é necessário informar um segundo fator de autenticação e por motivos óbvios este segundo fator não pode ser salvo dentro do cofre principal. Uma solução para segundo fator de autenticação que é gratuita e muito boa é o [Authy](https://authy.com/) que possui sincronização entre múltiplos dispositivos.

Existem diversas outras opções de gerenciadores de senhas com opções gratuitas para você começar a cuidar mais da segurança das suas senhas. Mas essas versões gratuitas obviamente tem algumas limitações que vão desde a quantidade de senhas armazenadas, ou quantidade de dispositivos que você pode usar.

Segue abaixo alguns dos gerenciadores que já usei ou testei que tem opções gratuitas para uso para que você possa testar e escolher o melhor para você.

### [KeePassXC](https://keepassxc.org/)

Se você quiser usar o KeePassXC para começar eu recomendaria além da chave mestre e do arquivo de chave armazenar no seu computador de forma segura usando o [NordLocker](https://nordlocker.com/).  😉

### [BitWarden](https://bitwarden.com/)

O [BitWarden](https://bitwarden.com/) é uma solução *open-source* muito boa. Tem planos gratuitos com sincronização em múltiplos dispositivos, extensão para navegadores, número ilimitado de senhas armazenadas entre diversas outras funcionalidades. Por ser *open-source*, é possível instalar ele em seu servidor pessoal ou da sua empresa e manter dentro de casa se próprio servidor de gerenciamento de senhas.

### [Dashlane](https://www.dashlane.com/)

O [Dashlane](https://www.dashlane.com/) tem opção gratuita que permite armazenamento de até 50 senhas e acesso por apenas um dispositivo. Parece limitado, mas se você usa majoritariamente apenas um dispositivo e não tem muitas senhas para armazenar, é uma excelente opção.

### [NordPass](https://nordpass.com/)

O [NordPass](https://nordpass.com/) conta com uma opção gratuita que oferece amazanamento ilimitado de senhas, auto-preenchimento de formulários, mas limita o acesso a apenas um dispositivo por vez.

### LastPass

[LastPass](https://www.lastpass.com/) oferece uma versão gratuita com armazenamento ilimitado de senhas mas limitado a apenas um tipo de dispositivo.

Para manter suas senhas ainda mais seguras você pode fazer algumas pequenas melhorias nas sua senhas geradas por essas ferramentas seguindo essas dicas do Gabriel Pato. Segue o vídeo:

<iframe width="100%" height="480" src="https://www.youtube.com/embed/AHRyEZdrXt8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Além de manter suas senhas mais seguras, você pode navegar de forma mais segura na internet usando navegadores como o [Firefox](https://www.mozilla.org/) ou [Brave](https://brave.com/) e manter suas buscas com mais privacidade usando buscadores como o [DuckDuckGo](https://duckduckgo.com/) e o [Brave Search](https://search.brave.com/).

## Referências

- [RockYou2021: Largest Ever Password Compilation Leaked, CyberNews](https://cybernews.com/security/rockyou2021-alltime-largest-password-compilation-leaked/)
- [Most Common Passwords [2021] - Is Yours on the List?, CyberNews](https://cybernews.com/best-password-managers/most-common-passwords/)
- [Have I Been pwned](https://haveibeenpwned.com/)
- [Find out if you've been part of a data breach](https://monitor.firefox.com/)
- [Leaked Password Check: Has My Password Been Hacked?](https://cybernews.com/password-leak-check/)
- [O que é um ataque de força bruta?](https://www.kaspersky.com.br/resource-center/definitions/brute-force-attack)
- [How Secure Is My Password?](https://howsecureismypassword.net/)
- [Correct Horse Battery Staple](http://correcthorsebatterystaple.net/)
- [Estimating Password Cracking Times](https://www.betterbuys.com/estimating-password-cracking-times/)
- [KeePass Password Safe](https://keepass.info/)
- [KeePassXC Password Manager](https://keepassxc.org/)
- [Authy, Two-factor Authentication (2FA) App & Guides](https://authy.com/)
- [Bitwarden Open Source Password Manager](https://bitwarden.com/)
- [Password Manager App for Home, Mobile, Business, Dashlane](https://www.dashlane.com/)
- [Securely Store, Manage & Autofill Passwords](https://nordpass.com/)
- [#1 Password Manager & Vault App with Single-Sign On & MFA Solutions, LastPass](https://www.lastpass.com/)
- [1Password](https://1password.com/)
