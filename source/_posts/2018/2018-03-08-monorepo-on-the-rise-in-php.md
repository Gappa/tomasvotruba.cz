---
id: 82
title: "Monorepo on the Rise in PHP"
perex: '''
    Do you know what monorepo is? How to start with it? What you need and do even other programming languages use it? And what about Facebook and Google think about it?
    <br><br>
    [Gomonorepo.org](https://gomonorepo.org/) will brief you with all important answers.
'''
tweet: "New post on my blog: State of Monorepo in PHP"
related_items: [41, 26, 25]
tweet_image: "/assets/images/posts/2018/monorepo/monorepo-website.png"
---

## Javasript, Java, C++, Android, iOS, Facebook, Google? Monorepo is Standard

When you pop out of PHP bubble, you can see in [awesome-monorepo](https://github.com/korfuri/awesome-monorepo) a collection of monorepo tools, that are used out in a wild by another languages. Google has [Bazel](https://bazel.build/), Facebook has [Buck](https://buckbuild.com/), Twitter and Foursqaure have [Pants](https://www.pantsbuild.org/).

**Still a PHP-related tool is missing**. Why? It might be the case, that no global company that goes open-source uses PHP as their main language.   

## Symfony Monorepo Spreads the Word
 
PHP is aware of monorepo term mainly thanks to [Symfony](https://github.com/symfony/symfony),  that uses it to maintain **all its components, that are split to standalone** read-only repositories, e.g. [Symfony\Console](https://github.com/symfony/console), [Symfony\EventDispatcher](https://github.com/symfony/event-dispatcher).

### Tool to Split With

Since Symfony needed a fast tool to split over 30 repositories across 3 and more branches, Fabien Potencier came with [splits](https://twitter.com/fabpot/status/739860138564149248?lang=en) tool.

He had also [very interesting talk about it](https://www.youtube.com/watch?v=4w3-f6Xhvu8) ([slides](https://speakerdeck.com/fabpot/a-monorepo-vs-manyrepos)), where he explains in details, how Symfony monorepo works, what is spliting, what are the needs for a build tool managing monorepo.

**But it's still to complex to start with and it doesn't cover the most common case - building monorepo from already existing repositories**. 

## Shopsys Monorepo to Spread a bit more Word

I work on [Shopsys Framework](https://shopsys-framework.com), an open-source e-commerce platform on Symfony and the monorepo topic finally came to the sprint to be realized. If you've read until now, **you know there is not much shared know-how or support for new-commers to adopt a monorepo pattern in PHP**. 

That's how [`shopsys/monorepo-tools`](https://github.com/shopsys/monorepo-tools), that covers both build and split was given birth by [Petr Heinz](https://github.com/PetrHeinz).

It's slowly getting better with monorepo in PHP. But still many people don't know what is difference between *a monorepo* and *a monolith*.

## New to monorepo? Start on GoMonorepo.org

Inspired by [GoPHP71.org](http://gophp71.org/), **to boost this progress even further and answer some basic questions about monorepo, I build a simple site [Gomonorepo.org](https://gomonorepo.org/)**.

<img src="/assets/images/posts/2018/monorepo/monorepo-website.png" class="img-thumbnail">

### What you'll Find There?

- What monorepo is and what monorepo isn't,
- what is *single repo*, *monolith* - all terms explained,
- what **tools** to use in PHP to simplify work with monorepo,
- when to use it and **when rather not**,
- historical must-read posts, **why to use it** included
- what talk to watch... 

...and **also list of open-source that run on monorepo**. Got monorepo on your open-source project? **[Add it there](https://github.com/TomasVotruba/gomonorepo.org/edit/master/_data/projects.yaml)** to inspire others. Symfony, Laravel, Sylius and Symplify are already there.

[Go check it](https://gomonorepo) and if you'd like to improve it, just send PR to [repository on Github](https://github.com/tomasvotruba/gomonorepo.org).

<br><br>

Happy rapping!