## Gwneud y gêm yn anoddach

Fe wnawn ni wneud y gêm i fynd yn anoddach yr hirach mae’r chwareuwr yn ei chwarae. Rwyt ti am wneud hyn gan wneud i'r dotiau ymddangos yn gynt ac yn gynt dros amser.

\--- task \--- Bydd angen creu `newidyn`{:class="block3variables"} newydd o’r enw 'oedi'.

![Corlun llwyfan](images/stage-sprite.png) \--- /task \---

\--- task \--- Ar dy lwyfan, bydd angen creu sgript newydd sydd yn gosod y newidyn `oedi`{:class="block3variables"} i `8`, ac yna yn lleihau yr amser `oedi`{:class="block3variables"} yn araf.

![Corlun llwyfan](images/stage-sprite.png)

```blocks3
    pan fo'r flag werdd yn cael ei glicio
gosod [oedi v] i (8)
ailadrodd hyd at <(oedi) = (2)> 
  aros (10) eiliad
  newid [oedi v] gan (-0.5)
end
```

\--- /task \---

Sylwa fod y côd yma yn debyg iawn i gôd y fyddet wedi ei ddefnyddio i greu amserydd!

Fe alli di ddefnyddio’r newidyn `oedi`{:class="block3variables"} ar gyfer sgriptiau’r dotiau 'coch', 'melyn' a 'glas'.

\--- task \--- Bydd angen cael gwared o’r côd sydd yn aros nifer o eiliadau rhwng creu cloniau. Ail-osoda'r bloc rwyt ti wedi cael gwared ohono gyda’r newidyn `oedi`{:class="block3variables"}:

![sgrinlun](images/all-dots.png)

```blocks3
<br />aros (dewis ar hap (5) i (10)) eiliad
aros (oedi :: variables) eiliad
```

Gwna hyn ar gyfer y tri corlun dot.

\--- /task \---

\--- task \--- Profa dy gêm i weld os yw'r dotiau yn ymddangos yn gynt wrth i'r gêm barhau.

+ Ydy hyn yn gweithio ar gyfer y tri lliw?
+ Wyt ti’n gallu gweld gwerth y newidyn `oedi`{:class="block3variables"} yn lleihau? \--- /task \---