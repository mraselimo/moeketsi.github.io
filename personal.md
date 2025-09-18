---
layout: page
css: personal

icon: user-circle
title: Personal
---

#### <i class='fas fa-fw fa-volume-up'></i>&nbsp; Pronouncing My Name

<div class='pure-g' style='text-align: center; font-size: 1.25em;'>
    <div class='pure-u-md-7-24 pure-u-1-2' style='margin-top: -1em;'>
        <p>
            <a class='color-faded color-medium-accent syl1'>MOH</a>-<a class='color-faded color-medium-accent syl2'>E</a>-<a class='color-faded color-medium-accent syl3'>KEH</a>-<a class='color-faded color-medium-accent syl4'>TSEE</a> 
            <a class='color-faded color-medium-accent syl5'>RAH</a>-<a class='color-faded color-medium-accent syl6'>SEH</a>-<a class='color-faded color-medium-accent syl7'>DEE</a>-<a class='color-faded color-medium-accent syl8'>MOH</a>
        </p>
        <p style='margin-top: -1em;'>
            <em style='font-size: 0.75em;'>
                (&hairsp;Approximate <a href='https://en.wikipedia.org/wiki/Pronunciation_respelling_for_English'>Respelling</a>&hairsp;)
            </em>
        </p>
    </div>
</div>
<div style='text-align: center; font-size: 1.125em; margin: -0.5em 0 0.5em 0;'>
Listen to <a onclick='play_steps();'>individual syllables</a>,
or my <a onclick='play_name();'>full name</a>.
</div>


<script>
    var audio_dict = {
        'syl1': new Audio('{{ site.baseurl }}/assets/mp3/Mo.m4a'),
        'syl2': new Audio('{{ site.baseurl }}/assets/mp3/E.m4a'),
        'syl3': new Audio('{{ site.baseurl }}/assets/mp3/Ke.m4a'),
        'syl4': new Audio('{{ site.baseurl }}/assets/mp3/Tsi.m4a'),
        'syl5': new Audio('{{ site.baseurl }}/assets/mp3/Ra.m4a'),
        'syl6': new Audio('{{ site.baseurl }}/assets/mp3/Se.m4a'),
        'syl7': new Audio('{{ site.baseurl }}/assets/mp3/Li.m4a'),
        'syl8': new Audio('{{ site.baseurl }}/assets/mp3/Moo.m4a'),
        'syl123': new Audio('{{ site.baseurl }}/assets/mp3/Moeketsi.m4a'),
        'syl45': new Audio('{{ site.baseurl }}/assets/mp3/Raselimo.m4a')
    };

    function activate(syl) {
        Array.prototype.forEach.call(document.getElementsByClassName(syl),
                                     e => e.classList.add('hovering'));
    }

    function deactivate(syl) {
        Array.prototype.forEach.call(document.getElementsByClassName(syl),
                                     e => e.classList.remove('hovering'));
    }

    function play(syl, callback, highlight) {
        if (!highlight) highlight = [syl];
        highlight.forEach(activate);
        audio_dict[syl].currentTime = 0;
        audio_dict[syl].onended = () => { highlight.forEach(deactivate); if (callback) callback(); }
        audio_dict[syl].play();
    }

    ['syl1','syl2','syl3','syl4','syl5', 'syl6', 'syl7', 'syl8'].forEach(function (syl) {
        Array.prototype.forEach.call(document.getElementsByClassName(syl), function (e) {
            e.onmouseenter = () => activate(syl);
            e.onmouseleave = () => deactivate(syl);
            e.onclick = () => play(syl);
        });
    });

    function play_steps() {
        play('syl1',
             () => play('syl2',
                        () => play('syl3',
                                  () => play('syl4',
                                        () => setTimeout(play, 300,
                                                    'syl5', () => play('syl6',
                                                    () => play('syl7',
                                                        () => play('syl8'))))))));
    }

    function play_name() {
        play('syl123', () => setTimeout(() => play('syl45', null, ['syl5','syl6', 'syl7', 'syl8']), 150),
             ['syl1','syl2','syl3', 'syl4']);
    }
</script>
