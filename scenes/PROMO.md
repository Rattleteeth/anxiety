# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[PELAA!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Ennen kuin aloitamme, miten *sinä* haluaisit lukea?

`publish("show_options_bottom")`

# intro-start-2

n3: Aloittakaamme tarina...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: TÄMÄ ON IHMINEN

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: JA TÄMÄ ON IHMISEN AHDISTUS

n: _SINÄ_ OLET AHDISTUS

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Ei. Ei, ei, en kuuntele. Katson jotain puhelimelta.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: SINUN TEHTÄVÄSI ON SUOJELLA IHMISTÄSI *VAARALTA*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Selaat elämäsi hukkaan Twitterissä! Taas!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Juu mietinkin miksen vain istu ja kuuntele ajatuksiani useammin

`hong({eyes:"neutral"});`

n: ÄKKIÄ, VAROITA HÄNTÄ *VAARASTA!*

```
bb({eyes:"look"});
```

[Voi ei, katso tuota kamalaa uutista!](#act1d_news)

[Voi ei, onko tuo twiitti salaisesti kirjoitettu *meistä?*](#act1d_subtweet)

[Hei, GIF kissasta juomassa maitoa](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: Heh joo tuo on söpö, taidan--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: KISSAT EIVÄT VOI SULATTAA MAITOA OLEMME KAMALIA IHMISIÄ JOTKA NAUTTIVAT ELÄINTEN HYVÄKSIKÄYTÖSTÄ

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



