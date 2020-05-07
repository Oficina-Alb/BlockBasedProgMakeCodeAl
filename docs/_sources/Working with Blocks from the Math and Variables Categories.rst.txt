Puna me blloqet nga kategoria Math dhe Varibles
==========================================================

MakeCode mbështet katër operacione themelore aritmetike:
- mbledhja (+),
- zbritja (-),
- shumëzimi (*) dhe
- pjesëtimi (/).

Blloqet që mundësojnë llogaritjen quhen operatorë aritmetikë. Ato janë të vendosura në kategorinë |Math|.

.. |Math| image:: ../_images/_imageMicroBit/p41.png

Operatorët aritmetikë kthejnë një **NUMËR** (rezultati i një operacioni aritmetik).

.. image:: ../_images/_imageMicroBit/p40.png
      :align: center

Ju mund të përdorni rezultatin (numrin) e kthyer nga një operator aritmetik si një vlerë hyrëse për blloqe, të cilët pranojnë numra. Kjo mund të shihet qartë në figurën e mësipërme. Blloku i numrit të shfaqjes ... pranon një numër si një input dhe e shfaq atë në ekran.

Ne vendosëm para jush një shprehje aritmetike më komplekse: (2 + 1) * (12 - 10). Në MakeCode, llogaritja e rezultatit mund të duket kështu:

.. image:: ../_images/_imageMicroBit/p42.png
      :align: center

Duke analizuar shprehjen komplekse, mund të konkludojmë se ai përbëhet nga njësi më të vogla - rezultate të përkohshme.

Shuma e (2 + 1) është një rezultat i përkohshëm. Diferenca e (12-10) është rezultati i dytë i përkohshëm. Do të marrim rezultatin e tërë shprehjes kur shumojmë shumën dhe ndryshimin (shuma * ndryshimi).

Në programim, është e përshtatshme të përdoren rezultatet e përkohshme (vlerat e përkohshme), të cilat i quajmë **variabla**. Ju mund të mendoni për variablat si hapësira në kujtesën e kompjuterit, të ngjashme me kutitë, në të cilat ruhen rezultatet e përkohshme. Variablat kanë emra.

Kur doni të përdorni vlerën e një variable specifike në një program, mjafton vetëm të tregoni emrin e saj.

Në MakeCode, ju krijoni variabla në kategorinë |Variables|.

.. |Variables| image:: ../_images/_imageMicroBit/p43.png

Krijojmë variabla duke klikuar në butoninMake a Variable (2) në kategorinë Variable (1), duke futur emrin e variablës (3), në rastin tonë emrin Counter, dhe më pas klikojmë në butonin OK (4).

.. image:: ../_images/_imageMicroBit/11.png
      :align: center

Është e qartë, ju mund ta paraqisni shprehjen tonë (2 + 1) * (12 - 10) ndryshe. Duke krijuar dy variabla: |Zbir| dhe |Razlika|.

.. |Zbir| image:: ../_images/_imageMicroBit/p45.png

.. |Razlika| image:: ../_images/_imageMicroBit/p44.png

Ne do ta vendosim vlerën fillestare të variablit ``Counter`` të jetë 0. Kjo mund të bëhet duke tërhequr bllokun |set| nga kategoria |Variables| në bllokun |onstart|.

.. |onstart| image:: ../_images/_imageMicroBit/s20.png

.. |set| image:: ../_images/_imageMicroBit/p47.png

Pamja finale e kodit:

.. image:: ../_images/_imageMicroBit/p46.png
      :align: center

.. mchoice:: L5Z1
   :answer_a: 2.
   :answer_b: 10.
   :answer_c: 4.
   :feedback_a: Përgjigja është e saktë!
   :feedback_b: Përgjigja nuk është e saktë!
   :feedback_c: Përgjigja nuk është e saktë!
   :correct: a
   

Krijoni një program, i cili ka dy variabla: x dhe y. Vlera e caktuar e variablës x duhet të jetë 2 (x = 2), dhe vlera e caktuar e variblit y duhet të jetë 4 (y = 4).

Kur programi ekzekuton bllokun e treguar në figurën më poshtë, rezultati do të jetë:

    .. image:: ../_images/_imageMicroBit/p48.png
          :align: center


Le të përdorim operatorët aritmetikë dhe variablat për të krijuar një program, i cili llogarit perimetrin dhe sipërfaqen e një katrori.

Për të llogaritur sipërfaqen e një katrori, është e nevojshme të përcaktoni gjatësinë e anës ``a``, vlera e së cilës do të ndryshojë rastësisht, sa herë që përdoruesi shtyp butonin ``A``, dhe kur butoni ``B`` shtypet, programi do të llogarisë perimetrin dhe sipërfaqen e sheshit të dhënë.

Në fillim, duhet të krijojmë variablat ``a``, ``P`` dhe ``A``, të cilat përfaqësojnë përkatësisht anën, perimetrin dhe zonën e sheshit.

Ndryshimi i rastësishëm i vlerës së variablit do të përcaktohet me përdorimin e bllokut |pickrandom|

.. |pickrandom| image:: ../_images/_imageMicroBit/p49.png

Pamja e kodit kur vlera fillestare përcaktohet dhe vendoset në bllokun |onbutton| tregohet më poshtë:

.. |onbutton| image:: ../_images/_imageMicroBit/p18.png


.. image:: ../_images/_imageMicroBit/p50.png
      :align: center

Për të parë vlerën e gjatësisë së brinjës ``a``, mund të tërheqim bllokun e ekranit |shownumber|.


.. |shownumber| image:: ../_images/_imageMicroBit/15.png

Pamja e bllokut:

.. image:: ../_images/_imageMicroBit/p51.png
      :align: center

Për të llogaritur perimetrin dhe sipërfaqen e një kartori, duhet të kujtojmë se perimetri i një kutie është 4 * gjatësia e brinjës (``4 * a``) dhe se zona e një sheshi është produkti të gjatësisë së brunjëve të saj (``a * a``). Ne përdorim shumëzimin për llogaritjen e kësaj. Pamja e bllokut për llogaritjen e perimetrit dhe sipërfaqes së një kartori është:

.. image:: ../_images/_imageMicroBit/p52.png
      :align: center

Për të provuar programin, ne do ta ekzekutojmë në simulator duke klikuar në butonin |play|.

.. |play| image:: ../_images/_imageMicroBit/p3.png

.. mchoice:: L5Z2
   :answer_a: Çdo vlerë nga intervali 0 deri në 15, pa përfshirë 0.
   :answer_b: Çdo vlerë nga intervali 0 deri 15, përfshirë ato vlera.
   :answer_c: Çdo vlerë nga intervali 0 deri në 15, pa përfshirë 15.
   :correct: b
   :feedback_a: Përgjigja nuk është e saktë!
   :feedback_b: Përgjigja është e saktë!
   :feedback_c: Përgjigja nuk është e saktë!


Studio bllokun me kujdes:

    .. image:: ../_images/_imageMicroBit/p53.png
          :align: center

Cila do të jetë vlera e variablit Counter kur të bëhet një lëvizje (tronditje)?
