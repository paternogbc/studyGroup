Grupo de Estudo Mozilla
============

Bem vindo ao [Mozilla Science Lab](https://www.mozillascience.org/)'s Projeto grupo de estudo! A partir daqui, iremos disponibilizar tudo que você precisa para começar o seu
próprio grupo de estudo.

### Pera ai, o que é um 'Grupo de Estudo Mozilla'?

Grupos de estudo Mozilla são divertidos, encontros informais com seus amigos e colegas ao redor de instituições locais e cidades para compatilhar habilidades,
histórias e ideias sobre o uso de programação em pesquisa. O objetivo é criar um ambiente
amigável e sem pressão onde as pessoas podem compartilhar seus trabalhos, pedir ajuda
para resolver problemas de programação e aprender e trabalhar junto com seus parceiros.

## Para participantes

Bem-vindo ao Grupo de Estudos Mozilla! Algumas coisas que você precisa saber e fazer agora que está aqui:

 - **Acompanhe este repositório:** lá em cima à direita, há um botão que diz "Watch"; clique nele e selecione 'Watching'. Isso fará com que você recebe notificações de novas discussões do grupo no seu e-mail; se você não quer receber e-mails com atualizações, mas gostaria de ser alertado no GitHub, altere as configurações em Settings -> Notification Center ('Settings' é a pequena engrenagem na barra lateral à direita). 
 - **Acompanhe nossas discussões:** clique em 'issues' na barra lateral à direita; é neste local onde todas as discussões desse grupo de estudos acontecem. Use esse espaço para fazer perguntas, requisitar eventos, fazer sugestões ou apenas dar um alô.
 - **Leia nosso código de conduta:** este Grupo de Estudos é para todos - nós somos guiados por um [conjunto de regras](https://www.mozillascience.org/code-of-conduct/) que solicita que todos sejam tratados com respeito. Ajude-nos a manter um espaço onde todos sintam-se bem-vindos e assim teremos um ótimo tempo juntos!
 - **Adicione-se a lista de membros:** Se você quiser aparecer na seção 'Quem somos nós' do nosso site, dê uma olhada em `_data/members.yml`; envie-nos um 'pull request' com os seus dados, ou abra um novo 'issue' com o seu pedido e nós faremos isso por você.

## Para Organizadores

### Não está funcionando, eu preciso de ajuda

Se algumas de nossas instruções não funcionar ou não fizer sentido, abra um [issue](https://github.com/mozillascience/studyGroup/issues) or email sciencelab@mozillafoundation.org.

### Confira o manual
Check out the Handbook

As intruções abaixo irão ajudar você a organizar as ferramentas online para o seu Grupo de Estudos Mozilla – mas se você estiver procurando por informações sobre estratégias de organização, planajemaneto de eventos e aulas, confira o [Manual do Grupo de Estudo Mozilla](https://mozillascience.github.io/studyGroupHandbook/)!

## Como criar o seu próprio Website Grupo de Estudo Mozilla?

Aqui você vai encontrar tudo que precisa para criar o seu próprio Website Grupo de Estudo Mozilla e organizar os seus eventos. Siga os próximos passos e seu site estará funcionando em breve. Se você encontrar problemas, [abra um issue](https://github.com/mozillascience/studyGroup/issues) e nós podemos te ajudar.

 1. **Crie um conta no GitHub.** O plano gratuito é suficiente.
 2. **Fork esse repositório.** No canto superior direito desta página tem um botão que diz 'Fork'; clique nele! Isso irá fazer uma cópia de todo esse material na sua própria conta do GitHub; Quando a cópia estiver pronta, o GitHub irá automaticamente te redirecionar para lá. 
 3. **Ative o monitoramento de issues.** O monitoramento de issues é um quadro de mensagens que o GitHub cria para cada repositório; você irá usar esse quadro para postar informações sobre seus eventos e conversar com os participantes. Para ativar o monitoramento de issues: 
   - clique em 'Settings' no canto direito da barra lateral do seu repositório. 
   - clique no botão de marcar 'Issues', na aba 'Features'; 
   - retorne ao seu repositório cliquando em `studyGroup` no topo da página. 
 4. **Edite o arquivo `_config.yml`** em seu repositório:
   - clique em `_config.yml`;
   - clique no pequeno lápis perto do canto superior direito;
   - siga as instruções de edição no próprio arquivo 
   - quando você terminar, clique no botão verde 'Commit Changes' no final da página.

É isso, você conseguiu! Você pode ver o seu website em 
`https://yourUserName.github.io/studyGroup/`, substitua `yourUserName` pelo nome de usuário da sua conta do GitHub. Se essa for a primeira vez que você estiver criando uma página no GitHub, esse processo pode demorar 30 minutos para que tudo flua pelos computadores do GitHub – não se preocupe, é assim mesmo. Verifique novamente depois e o seu website estará no ar funcionando normalmente. 

### Opcional: Configurando um Google Calendário para o seu Grupo de Estudos

Se você gostaria de oferecer um calendário de eventos para a sua comunidade para que eles possam importar seus próprios calendários, tente usar o Google Calendar. Para configurá-lo, faça um nova conta no Google, e atualize os campos no arquivo `_config.yml`, na seção 'Setup Google Calendar'.

Você pode adicionar eventos ao seu calendário manualmente, mas se quiser automatizar esse processo, existe um script para fazer isso `scripts/updateCalendar.py`; as instruções de uso estão no topo do arquivo. 

## Como lançar um novo evento

Quando você estiver pronto para apresentar um novo evento para o seu Grupo de Estudos, siga os próximos passos, ou [assista esse vídeo](https://youtu.be/abglQgEIccw) onde nós iremos te mostrar o passo a passo da lista de eventos.

 1. **Crie um novo Issue para descrever o seu evento.** 
   - clique em 'Issues' no canto direito do seu repositório, 
   - clique no botão verde 'New Issue' perto do canto direito superior. 
   - Você irá ver um formulário onde é possível dar um título e uma descrição para o seu evento – preencha esses campos com todas as informações relevantes:
     - Onde irá ocorrer o evento? Inclua o link para um mapa.
     - Quando será? Data e hora.
     - As pessoas precisam se preparar antes do evento? (instalar algum pacote?)
 2. **Vá para a pasta `_posts`**. Esta pasta se encontra em `https://github.com/yourUserName/studyGroup/tree/gh-pages/_posts` - ou você pode clicar em `_posts` no seu repositório.
 3. **Crie um novo arquivo** cliquando no sinal `+` ao lado de `_posts/`. Nomeie o arquivo seguindo esse padrão:
 4. 
    ```
    YYYY-MM-DD-word.markdown
    ```

    onde `YYYY-MM-DD` é a data do seu evento e `word` é qualquer palavra que quiser.
 4. **Cut and paste the following into your new file:**
 
    ```
    ---
    title: Study Group Meetup
    text: a one sentence description of your event
    location: Hacky Hour Stadium
    link: https://github.com/yourUserName/studyGroup/issues/1234
    date: 2016-01-04
    startTime: '15:00'
    endTime: '16:00'
    ---
    ```

    Change all the fields to describe your event; make sure the `link` is the address of the issue you created When you're done, click 'Commit Changes' at the bottom.

That's it! Your event is now listed on your webpage, and there's a discussion thread where people can ask questions and discuss the details. Events will be automatically removed from the schedule on the webpage when they're more than a week in the past - but the issue you created will always be there as a record of what you've done.

> **Event Listing Gotchas:** here are a few things to look out for when listing an event:
>  - Did you remember to include the `---` above and below? The website builder needs those.
>  - Can't find the issue tracker? Remember to turn it on under the 'Settings' menu on the right.
>  - The seven fields need to be on exactly one line each; some text editors will insert line breaks into lines that are too long; remove these if so.

## How to Stay in Touch With Your Members

Now that you're all set up, GitHub provides several ways to stay in touch with the people involved in your Study Group.

  - **Ask users to Watch your repo.** Make sure all your users click 'Watch' at the top of your repository. This way, they'll be automatically notified of all the events you post in your issue tracker. 
  - **Use the Issue Tracker.** The Issue Tracker is your public message board to make announcements, ask questions and start conversations with your members. You can find yours at `https://github.com/yourUserName/studyGroup/issues`.
  - **Use the Mozilla Science Forum** to chat with study groups worldwide. Find the [forum here](https://forum.mozillascience.org/category/events/study-groups); use this to share your stories, ask questions to the wider community, and find out who's out there.

## Feature Your Community in the 'Who We Are' Section

Your website includes a gallery of participants in your Study Group; adding people here is a great way to show off your community and highlight your new friends and colleagues. To add someone to the list, edit the `_data/members.yml` file by adding the following section for them:

```
- name: their human name
  affiliation: school, lab, department, business....
  github: their GitHub handle
  interests:
    - list one to three
    - different interests
```
