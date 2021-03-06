<!-- README template, populated using this action:
     https://github.com/kip93/kip93/blob/main/.github/workflows/readme.yml. -->

<h1 align="center">๐ Hello world! I'm @{{ LOGIN }}</h1> <!-- LOGIN => username -->

### ๐ค About me

I am a passionate self-taught backend software developer, and a strong advocate for libre software.


### ๐ฌ Some facts

* ๐ Coding since 2013.
* ๐ผ Currently working @ [OroraTech](https://ororatech.com/).
* ๐จโ๐ป [Python](https://github.com/search?q=user%3A{{ LOGIN }}&l=python) is โค๏ธ. <!-- LOGIN => username -->
* ๐ป [NixOS](https://github.com/NixOS/) /
     [Awesome](https://github.com/awesomeWM/) /
     [kitty](https://github.com/kovidgoyal/kitty/) /
     [xonsh](https://github.com/xonsh/).
* ๐ I have a [portfolio website](https://kip93.net/) with some more information.
* ๐ Checkout my [rรฉsumรฉ](https://kip93.net/resume/) for even more detail.
* ๐ซ Reach me @ [leandro@kip93.net](mailto:leandro@kip93.net).
* ๐ฒ Fun fact: My first program was not a "Hello World" (it was simple R/W in an [HC11 ยตC](https://en.wikipedia.org/wiki/68HC11) emulator).


-----------------------------------------------------------------------------------------------------------------------


### ๐ Stats

![](./stats.svg)


### ๐ Most used languages <!-- by percentage, in decreasing order -->

![](./languages.svg)


### ๐ Achievements

![](./achievements.svg)


-----------------------------------------------------------------------------------------------------------------------


<%- await include(`partials/activity.ejs`) %> <!-- Last activity -->


<h6 align="right"><em>
    Generated with <a href="https://github.com/lowlighter/metrics/tree/latest/">lowlighter/metrics v{{ VERSION }}</a> ๐ ๏ธ<br> <!-- VERSION => MAJOR.minor.patch -->
    Last updated @ {{ meta.generated }} / All times UTC โ <!-- meta.generated => DD/MM/YYYY, hh:mm -->
</em></h6>
