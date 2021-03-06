---
output:
  html_document: default
  pdf_document: default
---

# Task 1: Как настроить репозиторий на GitHub?

Это задание составлено для студентов и исследователей, которые хотят создать свой первый проект с открытым исходным кодом (по программному обеспечению или нет) в GitHub. GitHub - это место для того, чтобы поиграть (??) и поэкспериментировать с новыми исследовательскими процессами и в действительности это только начало, чтобы помочь подготовить почву для ваших собственных путей и идей 

Не забывайте, что вы можете присоединиться к обсуждениям в нашем открытом [**канале в Слак**](https://osmooc.herokuapp.com/). Пожалуйста, представьтесь в разделе  #module5opensource, расскажите, кто вы, из какой сферы, и как оказались здесь.

**ОБРАТИТЕ ВНИМАНИЕ** что экранная запись этого задания также доступна на [YouTube](https://www.youtube.com/watch?v=AnftV9HBPSc&).

Примерное время выполнения: 30-45 минут.

Примерное сэкономленное время после выполнения: Невообразимо.

## Оглавление

* [Начало работы](#Getting_started)
  * [Настройка профиля GitHub](#Profile)
  * [Язык GitHub](#Language)
  * [Создание нового репозитория](#Create_new)
* [Главные шаги](#Foundation)
  * [Выбор лицензии](#License)
  * [Создание README файла](#Readme)
  * [Создание правил участия](#Contributing)
  * [Создание кодекса поведения](#Conduct)
  * [Как сделать ваш код цитируемым](#Citation)
* [Сохраняем проблемы своевременно (???)](#Issues)
* [Чеклист для запуска вашего проекта](#Check-list)

<p align="center">
  <img src="https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/Task1.png?raw=true" alt="Task 1 workflow" width="600" height="861" style="margin-right: 30px; margin-left: 10px;" onmouseover="this.width='1200'; this.height='1722'" onmouseout="this.width='600'; this.height='861'">
</p>

<p align="center"><i>The workflow for Task 1. Keep this handy as you work through the task!</i></p>

<br/>

## Начало работы <a name="Getting_started"></a>

Репозиторий в действительности всего лишь модное слово для проекта на GitHub. GitHub это место в онлайне, где вы можете управлять проектами, хранить файлы, и открыто сотрудничать с другими. Все это достижимо за счет использования контроля версий,  с тем чтобы отслеживать как развиваются проекты. Таким образом, GitHub - мощный инструмент как для проектов по программному обеспечению, так и для других проектов. 

Одна из самого важного, о чем нужно подумать на этом раннем этапе это, то, как вам хотелось бы, чтобы широкая общественность взаимодействовала с вашим проектом. Так как вы работаете открыто, вам хочется удостовериться, что остальным удобно при доступе, просмоте и участии в вашей работе. Настройка репозитория таким образом, чтообы снизить барьеры для входа и страх быть "аутсайдером"  - вот первый шаг к выполнению успешного проекта.


<p align="center">
  <img src="https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/octocat.png?raw=true" width="150px" height="125px"/>
</p>

<p align="center"><i>Octocat, GitHub's little mascot</i></p>

<br/>

### Настройка профиля в GitHub <a name="Profile"></a>

Для настройки профиля в GitHub, просто отправьтесь на главную страницу и нажмите [Sign Up for GitHub](https://github.com/join). Здесь вы можете настроить ваш личный аккаунт, вклюячая логин, почту и пароль, как обычно. 

<p align="center"><img src="https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/github_signup.png?raw=true" width="800" /></p>

<p align="center"><i>Sign up for GitHub</i></p>

<br/>

Следуюзий шаг - настроить личный план. Пока что просто выберите 'Unlimited public repositories for free'/Неограниченный публичный репозиторий бесплатно/, если только вы не обеспокоены вопросами приватности, в этом случае выберите private plan /частный план/. Если вы намерены настроить проект для организации, можете выбрать эту опцию.

<br/>

### Язык Github <a name="Language"></a>

Это, возможно, один из самых сбивающих с толка и отталкивающих аспектов GitHub. Вот некоторые из наиболее часто используемых терминов и их определения:  

- **Initialise / Запустить, иницииализировать**: Создать пустой репозиторий.
- **Checkout / Проверить**: Создать рабочую копию локального репозитория 
- **Clone / Клонировать**: Скопировать репозиторий с локальную папку на вашем компьютере
- **Fork / сделать fork!!!**: Создать персональную копию репозитория, чтобы рабоать над ней параллельно. 
- **Branch / Ветвь**: Независимая и параллельная версия репозитория. Изменения в ней не  влияют на главную ветвь
- **Master**: Главная ветвь репозитория по умолчанию.
- **Clean / чисто, без изменений**: В ветви нет коммитов ожидающих рассмотрения.
- **Stage / **: Add updates ready to be committed to a branch.
- **Commit / коммит, фиксация изменений**: Исправление/ новая версия в репозитории, своего рода функция "сохранить".
- **Commit message / сообщение о коммите, т.е. фиксации изменений**: Описание изменений, содержащихся в коммите. 
- **Check / проверка**: проверка статуса.
- **Fetch / получить**: Никакого отношения к собакам (fetch - команда "апорт" для собак) . Относится к получению последних изменений из онлайн репозитория без их слияния. 
- **Index / индекс, кеш**: The 'tree' which acts as a staging area.
- **Working Directory / рабочая папка**: дерево, где хранятся файлы 
- **Head/ "голова"**: Дерево, которые показывает последние сделанные коммиты. 
- **Push/ добавить элемент**: Добавить закомиченные изменения в "шапку" вашего удаленного репозитория  
- **Merge/ слияние, объединение**: Объединение изменений сделанных в ветке с Главной веткой (master branch) по завершении. 
- **Pull / извлечение**: Обновление вашего репозитория путем получения и слияния новейших фиксированных изменений (коммитов) 
- **Pull request / запрос на извлечение**: Запрос на объединение и обновление измененной ветви в главную ветвь. 
- **Issue / проблема**: Предлагаемые улучшения, задачи, или вопросы, относящиеся к репозиторию. 

Фффух! Не волнуйтесь по поводу запоминания *всех* их прямо сейчас. Как и во всех прочих навыках, осведомленность придет с опытом  

Вы, вероятно, смогли заметить, что некоторые из них похожи на такие штуки как сохранить, скопировать, вставить - стандартные рабочие операции, но адаптированные для процесса управления програмной разработкой. Вот еще [несколько](https://mirrors.edge.kernel.org/pub/software/scm/git/docs/gitglossary.html) , но перечисленных должно быть достаточно для начала.

Если вам интересно, то большинство этих терминов пришло из основополагающей [Git системы](https://git-scm.com). Git был создан для того, чтобы разработчики могли управлять разными версиями исходного кода распределенным способом, и это здорово. У него есть множество качеств и способность делать всяческие сложные штуки, прописанные  [очень умным парнем](https://www.linuxfoundation.org/blog/2015/04/10-years-of-git-an-interview-with-git-creator-linus-torvalds/).  Тем не менее, [пользовательский интерфейс не был спроектирован с учетом новых пользователей](https://xkcd.com/1597/), так что учиться может быть тяжеловато.

<p align="center">
  <img src="https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/git.png?raw=true" width="150px"/>
</p>

<p align="center"><i>Unbeatable guide to using Git. (Source: XKCD)</i></p>

<br/>


### Создание нового репозитория <a name="Create_new"></a>

На вашей страничке GitHub нажмите на 'Create new repository' / "создать новый репозиторий". Первый шаг - придумать имя как торговую марку вашего проекта. В идеале, оно должно быть запоминающимся и давать некоторые указания на то, чем занимается проект. 
<p align="center"><img src="https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/new_repo.png?raw=true" width="800" /></p>

<p align="center"><i>Create a new repository</i></p>

<br/>

Проверьте, что имя не дублируется, что оно не наносит ущерб прочим торговым маркам и не содержит ничего, что могло быть рассмотрено как оскорбление. 

<br/>

## Основополагающие шаги <a name="Foundation"></a>

Для каждого GitHub репозитория требуются 4 ключевых элемента для запуска и начала развития доброжелательного сообщества:

1. Лицензия на открытое программное обеспечение;
2. Файл `README`;
3. Правила участия; и
4. Правила поведения.

Это важнейшие аспекты и лучшая практика любого проекта, необходимая для того, чтобы пользователи понимали свои законные права, свои ожидания, цели проекта, и вообще, чтобы облегчить их клиентский опыт. (???)

Все эти четыре файла следует хранить в корневой папке репозитория вашего проекта. Традиционно для большинства этих файлов используется markdown формат (`.md`) (хотя для файлов с лицензией чаще используют текстовый формат (`.txt`)). В именах файлов используют заглавные буквы. Вместо пробелов в именах файлов пожалуйста используйте нижние подчеркивания `_` .

Итак, у вас должен получиться базовый набор файлов, такого вида: 

1. `LICENSE.md`
2. `README.md`
3. `CONTRIBUTING.md`
4. `CODE_OF_CONDUCT.md`

<p align="center"><img src="https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/foundation.png?raw=true" width="800" /></p>

<p align="center"><i>The basic repository structure</i></p>

<br/>

### Выбор лиценции <a name="License"></a>

Choosing an appropriate license is what will differentiate your Open Source repository from publicly available software. While you are not obliged to choose a license, doing so guarantees that others will be able to modify, share, re-use, and build upon your project within a legal framework.

To start with, you want to check [Choose A License](https://choosealicense.com/) to find a license that best suits your intentions for the repository.

The three primary ones to choose from are:

* **MIT License**: A permissive license that lets people do whatever they want with your code as long as they provide appropriate attribution to you, and do not hold you liable.
* **Apache License 2.0**: Similar permissions to the MIT License, but also provides an express grant of patent rights from contributors to users.
* **GNU General Public License (GPL) v3**: A [copyleft](https://en.wikipedia.org/wiki/Copyleft) license that requires anyone who redistributes your code, or a derivative work, to make the source available under the same terms as the original license; also provides an express grant of patent rights from contributors to users.

Thankfully, when you start a new repository on GitHub, you are given the option to select an existing license from a drop-down menu.  You should always (with very few exceptions) use an existing license, since this is what potential users and contributors will see before they choose to use or contribute to your software.

<p align="center"><img src="https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/license.png?raw=true" width="800" /></p>

<p align="center"><i>Choosing an example license</i></p>

<br/>

If they don't have one you want, you can add one you like manually. To do this, simply click 'Create new file' in the repository, and copy and paste an existing license text in. Name the file something like `LICENSE.txt` or `LICENSE.md` to make it clear, and keep it in the main repository folder (i.e., the root). Make sure to add a clean commit message, and you're done!

> **Helping hand**: This MOOC uses a different combination of licenses for code content and non-code content. Here you can find an example of the [MIT License](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/LICENSE.md) that we apply for all code and software generated as part of the MOOC production.

<br/>

### Creating a README file <a name="Readme"></a>

When you initialise your new repository, there should be an option to do so with a `README` file. Just like Alice in Wonderland, these do exactly what they say - provide key information about the project. These are typically the first thing outside contributors will see when they come to your repository, so making them informative and welcoming is key.

<p align="center"><img src="https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/readme.png?raw=true" width="800" /></p>

<p align="center"><i>Part of the README file for this module</i></p>

<br/>

The file will originally be in markdown (`.md`) format. This is a lightweight markup language with a plain text format. To learn some basic markdown, see [this cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet). But for now, we can just use plain text.

There are several things you will want to include in your `README` file:

* What is this project about and what does it do.
* Why should people care, and why is it useful.
* How can someone get started contributing to the project.
* Who can be contacted in case someone needs help.
* A link to the license, contributing guidelines, and code of conduct.
* A description of the project structure.
* Who is involved, and what are their roles.
* The current status of the project.

> **Pro-tip**: Later on as your project develops, you might want to add FAQs based on community feedback, or a tutorial to help users understand how your project works.

Remember that not everyone coming to your project will be an expert, or understand what it is you are doing and why. Having a well-documented `README` file will enhance the user experience for people with a range of prior knowledge.

When the `README` file is included in the root directory, GitHub will automatically display this on the homepage of your repository. This means it is the first thing people will often see, so make it count!

> **Helping hand**: Here, you can find the `README` file used for this [MOOC module](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/README.md). This includes information on the status, rationale, learning outcomes, development team, key documents, and license to help. You can copy and adapt this structure for your own projects as needed.

<br/>

### Creating contributing guidelines <a name="Contributing"></a>

Contributing guidelines are designed to communicate to potential contributors a short guide on how to engage with your project and community. You want to make sure to be welcoming, and indicate that you are eager for participants to engage with your project. Whenever a participant opens a new pull request or creates a new issue, they will see a link to your contribution file.

<p align="center"><img src="https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/contributing.png?raw=true" width="800" /></p>

<p align="center"><i>Part of the `CONTRIBUTING` guidelines for this module</i></p>

<br/>

Sticking with the all caps file names, the next step is to create a `CONTRIBUTING` file. Click 'Create new file', and make sure to save it in markdown format as before. This file will tell other users how they can engage with and participate in your project. This is the first step towards establishing a community around your project, so make it engaging, concise, and informative.

The `CONTRIBUTING` file should include information on:

* What sort of contributions you are looking for.
* How to suggest updates or new features.
* How to interact with the project using GitHub's functions (e.g., the pull request protocol).
* How to file a bug report or create an issue.
* The ultimate goal, vision, or roadmap for the project.
* How to contact those in charge of the project.
* Links to any external documentation or websites.

> **Pro-tip**: Consider starting off with a short thank you note for people taking the time to consider contributing - they have clicked on the file to learn more after all! If there are other methods of recognition that you have in mind, make sure to include them in here too.

Here, you are essentially trying to encourage people to volunteer their time to advance your project. Make sure to be welcoming and friendly, and be precise about how people can engage. When writing this, make sure to think about it from the user perspective - how can you make their life easier when submitting pull requests and opening issues to make the whole project run more smoothly.

> **Helping hand**: The [Contributing guidelines](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/CONTRIBUTING.md) for this MOOC module include some very specific things: an introduction to using Git and GitHub, tips for getting started, contact information, how to alter the content and repor issues, a link to the `README` file, and information on the preferred content and code styles. Feel free to copy and adapt this for your own project as needed.

<br/>

### Creating a Code of Conduct <a name="Conduct"></a>

A code of conduct is important for setting the ground rules for expected behaviour and participation for project contributors, and is an easily referenced document for showing that your project team takes constructive dialogues seriously. Therefore, it is a critical element for creating and maintaining a healthy community that engages in a constructive and productive manner within a positive social atmosphere.

A code of conduct not only provides expectations of behaviour, but also describes who those expectations apply to, when they apply, what to do should a violation of the code occur, and what the action items for this will be. As such, points of contact need to be made clear in the code of conduct. Typically, this should be in a private way such as an email address.

> **Pro-tip**: In case a violation needs to be reported about the person who receives those reports, make sure to include an option to contact a secondary party.

To add a code of conduct, you can create your own from scratch by adding a new markdown file, or use existing templates such as the [Contributor Covenant](https://contributor-covenant.org/). Name your file `CODE_OF_CONDUCT.md`, and make sure it is visible in the `README` file.

> **Helping hand**: This MOOC also has a [Code of Conduct](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/CODE_OF_CONDUCT.md) based on the Contributor Covenant. As you can see, it includes information on expected standards of behaviour, responsibilities of those in the community, and enforcement of the CoC including contact details. Feel free again to re-use and adapt this to your project as you see fit.

<p align="center"><img src="https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/code_of_conduct.png?raw=true" width="800" /></p>

<p align="center"><i>Part of the CODE OF CONDUCT file for this module, based on the Contributor Covenant</i></p>

<br/>

Making sure to enforce the code of conduct is important, as it shows that not only do you value the code, but you respect the influence that it has on your community. It is important to treat each member of the community with the respect, courtesy, and importance that they deserve. Should a violation occur, or a repeat offender makes consistent violations, it is best to refer to the [Open Source Guide](https://opensource.guide/code-of-conduct/#enforcing-your-code-of-conduct) to see how to enforce the code of conduct.

<br/>

### Making your code citable <a name="Citation"></a>

If you want to make your code citable from the start, you should store the metadata needed for a citation from the start, by creating a `[codemeta.json](https://codemeta.github.io)` file or a `[CITATION.cff](https://citation-file-format.github.io)` file. Both will allow tooling that is currently being developed to automatically create citation information, rather than asking you to type it in a form later.

If you're interested, [cite.research-software.org](https://cite.research-software.org) provides further background information about software citation in academia.

<br/>

## Keeping your issues up to date <a name="Issues"></a>

Issues are not necessarily problems with a project, but also suggestions for improvement, things to develop in the future, and comments and feedback about the project to work through. They can be openly shared and discussed with contributors as needed, sort of like a forum.

If you are a project lead, it is important to maintain a list of issues that make it clear to contributors what aspects of the project need attention. It is also important to engage with as many issues as possible from others in a positive manner, to show that you take their contributions seriously.

Key elements for issues include:

* An informative title and description;
* Coloud-coded labels/tags to help categorise and filter;
* Milestones to associate issues with specific features or project phases;
* Assignees indicate who is responsible for working on an issue;
* Comments for providing feedback.

<p align="center"><img src="https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/issues.png?raw=true" width="800" /></p>

<p align="center"><i>The issue tracker for the Open Scholarship Strategy project</i></p>

<br/>

Within issues it is possible to use @ mentions to notify other contirbutors about the issue, and to get the right people engaged in an effective manner. GitHub has an internal system of notifications, just like Facebook or Twitter, and can also send emails to people who are mentioned in the issue tracker. This can all be customised for individuals within the user settings.

<br/>

## Checklist for launching your project <a name="Checklist"></a>

So now you are ready to launch your project, begin advertising it, and getting contributions! Before continuing, make sure that you have:

- [ ] Project has a memorable and informative name
- [ ] Project has a `LICENSE` file that is an exact copy of an Open Source license
- [ ] Complete documentation including a `README`, `CONTRIBUTING`, and `CODE_OF_CONDUCT` files
- [ ] Project has at least one clearly labelled issue
- [ ] Any code included at this stage is clearly structured and annotated


**CONGRATULATIONS!**

You have now launched an Open Source research project! Hopefully, from here on out, your work will act to benefit the wider community, forge new collaborations, and create new and fantastic opportunities for you all. Try and think about ways in which these skills can be applied to future projects, and how they might also have helped with some in the past.

From now on, it is all up to you! Some advice is to:

* Write clean code;
* Have a well-structured project;
* Make frequent commits with clean messages;
* Keep projects well-documented;
* Have clear contributing guidelines;
* Make use of the description and tag functions;
* Don't fork someone else's repository unless you intend to work on them;
* Make sure to contribute to other people's projects too.

**Know a way this content can be improved?**

Time to take your new GitHub skills for a test-run! All content development primarily happens [here](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/Task_1.md). If you have a suggested improvement to the content, layout, or anything else, you can make it and then it will automatically become part of the MOOC content after verification from a moderator!

[![CC0 Public Domain Dedication](https://img.shields.io/badge/License-CC0%201.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)