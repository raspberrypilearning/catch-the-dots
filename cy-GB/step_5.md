## Gwneud y gêm yn anoddach

Fe wnawn ni wneud y gêm i fynd yn anoddach yr hirach mae’r chwareuwr yn ei chwarae. Rwyt ti am wneud hyn gan wneud i'r dotiau ymddangos yn gynt ac yn gynt dros amser.

\--- task \--- Bydd angen creu `newidyn`{:class="block3variables"} newydd o’r enw 'oedi'.

![Corlun llwyfan](images/stage-sprite.png) \--- /task \---

\--- task \--- Ar dy lwyfan, bydd angen creu sgript newydd sydd yn gosod y newidyn `oedi`{:class="block3variables"} i `8`, ac yna yn lleihau yr amser `oedi`{:class="block3variables"} yn araf.

![Corlun llwyfan](images/stage-sprite.png)

```blocks3
    when flag clicked
    set [delay v] to (8)
    repeat until < (delay) = (2)>
        wait (10) seconds
        change [delay v] by (-0.5)
    end
```

\--- /task \---

Sylwa fod y côd yma yn debyg iawn i gôd y fyddet wedi ei ddefnyddio i greu amserydd!

Fe alli di ddefnyddio’r newidyn `oedi`{:class="block3variables"} ar gyfer sgriptiau’r dotiau 'coch', 'melyn' a 'glas'.

\--- task \--- Bydd angen cael gwared o’r côd sydd yn aros nifer o eiliadau rhwng creu cloniau. Ail-osoda'r bloc rwyt ti wedi cael gwared ohono gyda’r newidyn `oedi`{:class="block3variables"}:

![sgrinlun](images/all-dots.png)

```blocks3
<br />-   wait (pick random (5) to (10)) secs
    wait (delay :: variables) secs
```

Gwna hyn ar gyfer y tri corlun dot.

\--- /task \---

\--- task \--- Profa dy gêm i weld os yw'r dotiau yn ymddangos yn gynt wrth i'r gêm barhau.

+ Ydy hyn yn gweithio ar gyfer y tri lliw?
+ Wyt ti’n gallu gweld gwerth y newidyn `oedi`{:class="block3variables"} yn lleihau? \--- /task \---