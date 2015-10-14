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

Welcome to our Mozilla Study Group! A few things to do & know now that you're here:

 - **Watch this repo:** up in the top right, there's a button that says 'Watch'; click it, and set yourself to 'Watching'. This will send you email notifications of new discussions; if you don't want email, but would like an alert just on GitHub, change the setting in Settings -> Notification Center (Settings is the little cog in the top right).
 - **Check out the issue tracker:** click on 'issues' in the sidebar on the right; this is where all the conversations this study groups is having live. Use this space to ask questions, request events, make suggestions, or just say hi.
 - **Read the code of conduct:** this Study Group is for everyone - we abide by a [set of rules](https://www.mozillascience.org/code-of-conduct/) that require everyone be treated with respect. Help us make a space where everyone feels welcome, and we'll all have a better time!
 - **Add yourself to the website:** If you'd like to appear on the website under the 'Who we Are' section, have a look at the `_data/members.yml`; send us a pull request with an entry for yourself, or open an issue and we'll do it for you.

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
### Optional: Setting up a Google Calendar for your Study Group

If you'd like to offer your community a calendar of events they can import into their own calendars, try using a Google Calendar. To set up, make a new google account, and update the variables in `_config.yml` under the heading 'Setup Google Calendar'.

You can add events to your calendar by hand, but if you'd like to manage it automatically, there's a script to do so in `scripts/updateCalendar.py`; instructions for use are at the top of that file.

## How to Launch a New Event

When you're ready to list a new event for your Study Group, follow these steps, or [watch this video](https://youtu.be/abglQgEIccw) where we walk you through event listing.

 1. **Make a new Issue to describe your event.** 
   - Click on 'Issues' over on the right sidebar of your repo, 
   - click the green 'New Issue' button near the top right. 
   - You'll then see a form where you can give your event a title and a description - fill these out with all the relevant information:
     - Where will your event be? Include a link to a map.
     - When will it be? Date and time.
     - Should people do anything to prepare beforehand (install any dependencies, set something up?)
 2. **Go to the `_posts` directory**. It'll be at `https://github.com/yourUserName/studyGroup/tree/gh-pages/_posts` - or you can click on `_posts` in your repo.
 3. **Make a new file** by clicking on the `+` sign beside `_posts/` Name it like the following:

    ```
    YYYY-MM-DD-word.markdown
    ```

    where `YYYY-MM-DD` is the date of your event, and `word` is anything you want.
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
