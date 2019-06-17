[![Build Status](https://travis-ci.org/jollheef/free-as-in-freedom-v2-ru.svg?branch=master)](https://travis-ci.org/jollheef/free-as-in-freedom-v2-ru)
[![@faif_ru](https://img.shields.io/static/v1.svg?label=Telegram&message=@faif_ru&color=blue)](https://t.me/faif_ru)

# [free-as-in-freedom-v2-ru](https://code.dumpstack.io/etc/free-as-in-freedom-v2-ru)

Русский перевод второго издания [Free as in Freedom: Richard Stallman's Crusade for Free Software](https://www.fsf.org/faif/).

## Как скомпилировать книгу?

На данный момент перевод еще не закончен, а готовые части в формате pdf выкладываются в [Releases](https://github.com/jollheef/free-as-in-freedom-v2-ru/releases) на GitHub.

Тем не менее, если вы хотите собрать книгу из исходников .tex, вам необходимо:

1 Установить texlive и rubber.

NixOS:

    nix-env -iA nixos.texlive.combined.scheme-full nixos.rubber

Debian/Ubuntu:

    sudo apt install texlive-full rubber

2 Склонировать репозиторий и запустить сборку.

    git clone https://code.dumpstack.io/etc/free-as-in-freedom-v2-ru.git
	cd free-as-in-freedom-v2-ru
    make

В текущей директории появится файл faif-2.0.pdf.

## fb2, markdown или html версии

Для получения fb2, markdown или html версии можно воспользоваться [pandoc](https://pandoc.org/). Одноименный пакет есть во всех основных дистрибутивах.

fb2:

    pandoc -t fb2 faif-2.0.tex > faif-2.0.fb2

markdown:

    pandoc -t markdown faif-2.0.tex > faif-2.0.md

html:

    pandoc -t html faif-2.0.tex > faif-2.0.html

## Как следить за проектом?

По мере перевода глав будут происходить релизы с приложением добавленных глав. Следовательно, если вы хотите получать уведомления о появлении перевода новых глав — [подпишитесь на релизы с помощью штатной функциональности GitHub](https://help.github.com/en/articles/watching-and-unwatching-releases-for-a-repository).

## Чем можно помочь проекту?

Непосредственно перевод уже выполняется оплаченным мной переводчиком, поэтому за текст беспокоиться не стоит. Если вы хотите поддержать подобные инициативы, то напишите мне на почту root@dumpstack.io, и я расскажу вам о том, какой следующий шаг мы можем сделать.

Тем не менее, если вы обнаружите ошибки, неточности, либо у вас будут любые мысли по поводу проекта — не стоит стесняться [создавать Issue](https://github.com/jollheef/free-as-in-freedom-v2-ru/issues/new) либо присылать правки [посредством Pull Requests](https://help.github.com/en/articles/creating-a-pull-request-from-a-fork).
