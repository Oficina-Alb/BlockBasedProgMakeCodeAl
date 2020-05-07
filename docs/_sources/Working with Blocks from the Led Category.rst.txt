Puna me blloqet nga kategoria Led
=========================================

Në këtë pjesë do të njihemi me blloqet nga kategoria |led|, si dhe me atë se si mund të përcaktojmë vendndodhjen e LED në ekran, kështu që mund t'i kthejmë ato bazuar në pozicionin e tyre në ekran.

.. |led| image:: ../_images/_imageMicroBit/p24.png

Sistemi i koordinatave Karteziane përdoret në matematikë për të përcaktuar pozicionin e pikave në një aeroplan. Në sistemin koordinativ Kartezian, ekzistojnë dy akse koordinative të përcaktuara: ``x`` dhe ``y``.

Ekranet e Micro:bit dhe simulimi MakeCode përdorin këtë sistem për të përcaktuar pozicionin e LED-ve në ekran. Akset ``x`` dhe `` y`` formojnë një rrjet 5 x 5, rrjetin e rreshtave dhe kolonave, ku ka 5 LED në akset horizontale, boshti koordinativ ``x`` (rreshti), dhe 5 LED në boshtet vertikale, boshti i koordinatave ``y`` (kolona). Këndi i sipërm i majtë ka koordinatat (0,0), ndërsa vlerat e x koordinatave shkojnë nga 0 në 4, dhe ato rriten me 1 nga e majta në të djathtë; vlerat e koordinatës y shkojnë nga 0 në 4, dhe ato rriten me 1 nga lart poshtë. Për shembull, nëse LED është e vendosur në rreshtin e parë dhe në kolonën e tretë, koordinatat e saj janë (0,2).

.. image:: ../_images/_imageMicroBit/p25.png
      :align: center

Krijoni një program, i cili do të ndizet LED me koordinatat (3,3).

Zvarrit bllokun |plot| nga kategoria |led| në bllokun |onstart|, i cili tashmë është në sipërfaqen e punës.

.. |onstart| image:: ../_images/_imageMicroBit/s20.png
.. |plot| image:: ../_images/_imageMicroBit/p26.png

.. |play| image:: ../_images/_imageMicroBit/p3.png

Pamja finale e kodit:

.. image:: ../_images/_imageMicroBit/p29.png
      :align: center

Për të provuar programin, ne do ta ekzekutojmë në simulator duke klikuar në butonin |play|.

.. mchoice:: L4Z1
   :answer_a: LED në simulatorin A.
   :answer_b: LED në simulatorin B.
   :answer_c: LED në simulatorin C.
   :feedback_a: Përgjigja është e saktë!
   :feedback_b: Përgjigja nuk është e saktë!
   :feedback_c: Përgjigja nuk është e saktë!
   :correct: a
   
   Shikoni me kujdes bllokun.

.. image:: ../_images/_imageMicroBit/p31.png
      :align: center

Cila LED do të ndizet në ekran pasi programi të fillojë të funksionojë?

    .. image:: ../_images/_imageMicroBit/p30.png
      :align: center


Nëse duam të fikim LED-in, do të përdorim bllokun |unplot|, në të cilin do të përcaktojmë pozicionin (koordinatat) e ZHEL që duam të fikim. Me fjalë të tjera, ne përcaktojmë koordinatat x dhe y të LED.

.. |unplot| image:: ../_images/_imageMicroBit/p27.png

**Detyrë.** Bëni të ndezura të gjitha LED në fillim të programit. Kur përdoruesi shtyp butonin A, LED-et e vendosura në qoshet e ekranit do të fiken.

Ju mund ta krahasoni zgjidhjen tuaj me tonën: https://makecode.microbit.org/_4e6RXM5FmA8M

**Detyrë.** Krijoni një program, i cili do të simulojë semaforët duke ndezur dhe fikur LED-et e vendosura në rreshtin e tretë dhe kolonën e dytë, të tretë dhe të katërt.

**Ndihmë e vogël:** Ndërsa semaforët ndizen dhe fiken në interval të caktuar (le të themi 1 sekondë), duhet të përdorni bllokun |pause| për të përcaktuar atë interval.

.. |pause| image:: ../_images/_imageMicroBit/s39.png

Ju mund ta krahasoni zgjidhjen tuaj me tonën: https://makecode.microbit.org/_TRPRj98xj2Ap

|Toogle| është blloku i përdorur për të ndezur LED nëse është i fikur ose për ta fikur nëse është i ndezur. Sigurisht, në këtë bllok, duhet të vendosim vlerat për koordinatat x dhe y.

.. |toogle| image:: ../_images/_imageMicroBit/p28.png

.. mchoice:: L4Z2
   :answer_a: Drita do të fiket pas 1 milisekondi.
   :answer_b: Drita do të ndizet dhe fiket çdo 1 milisekondi.
   :answer_c: Drita do të ndizet pas 1 milisekondi.
   :feedback_a: Përgjigja nuk është e saktë!:feedback_b: Përgjigja është e saktë!
   :feedback_c: Përgjigja nuk është e sakte!
   :correct: b
   
Shiko me kujdes bllokun.

    .. image:: ../_images/_imageMicroBit/p32.png
          :align: center

    Çfarë do të shfaqet pas ekzekutimit të blloqeve të paraqitura më lart?

Shtesë: Për të analizuar të dhënat hyrëse (grafikisht), në rastin tonë, nivelin e dritës, mund të përdorim bllokun |plotbar| ku do të futim vlerën fillestare dhe përfundimtare të intervalit që duhet të analizohet.

.. |plotbar| image:: ../_images/_imageMicroBit/p33.png

Në rastin tonë, vlera fillestare do të jetë blloku |level| (e cila ruan vlerën e leximit të sensorit të dritës), dhe vlera përfundimtare do të jetë 255 sepse sasia e dritës së matur varion nga 0 në 255.

.. |level| image:: ../_images/_imageMicroBit/s54.png
.. |forever| image:: ../_images/_imageMicroBit/s1.png
.. |Basic| image:: ../_images/_imageMicroBit/s2.png

Blloku |plotbar| është tërhequr në bllokun |forever| nga kategoria |Basic|.

Pamja e bllokut:

.. image:: ../_images/_imageMicroBit/p34.png
      :align: center


Për të provuar programin, ne do ta ekzekutojmë në simulator duke klikuar në butonin |play|.

Në këtë rast, ne do të hapim simulatorin, i cili tregon të dhënat si një graf.

.. image:: ../_images/_imageMicroBit/p37.png
      :align: center

.. image:: ../_images/_imageMicroBit/p38.png
      :align: center


Ky imitues do të funksionojë derisa ta ndalojmë duke klikuar në butonin |stop|. Nëse duam të shkarkojmë të dhënat e mbledhura të hyrjes, mund t'i shkarkojmë në kompjuterin tonë në formatin CSV, duke klikuar në butonin |preuzmi|. Ky dokument përmban kolonat me kohën (në milisekonda) dhe nivelin e dritës së matur.

.. |stop| image:: ../_images/_imageMicroBit/p39.png
.. |preuzmi| image:: ../_images/_imageMicroBit/p36.png
