Puna me Blloqe nga Kategoria e Radios
=============================================

Në këtë mësim, do të njihemi me blloqet nga kategoria |Radio|, d.m.th. blloqet të cilat përdoren për krijimin e një lidhjeje dhe komunikimi midis dy ose më shumë pajisjeve Micro:bit. Ashtu si në këtë rast ne nuk do të përdorim Micro:bit, në ekranin e simulatorit do të shfaqen dy Micro: bit.
Në simulator, të gjitha kodet e krijuara do të funksionojnë në të dy Micro:bit virtuale.

.. |Radio| image:: ../_images/_imageMicroBit/s21.png

Krijoni një program i cili, kur shtypet butoni A, dërgon një numër të rastit nga intervali 0 në 100. Kur merret ky informacion, në mes të ekranit shfaqet një dritë, duke formuar një katror 3x3 nëse numri i marrë është i barabartë; përndryshe, shfaqet vlera e këtij numri.

Duke krijuar një grup ID, ne në fakt krijojmë një hapësirë ku pajisjet do të komunikojnë.

Për të krijuar një grup ID, duhet të tërheqim bllokun |radioset| nga kategoria |Radio| në bllokun |onstart|. Në fushën e hyrjes për numra dhe tekst, ne mund të vendosim numrin e dëshiruar për grupin e identitetit, i cili mund të jetë çdo numër. Do ta lëmë që të jetë 1. Në këtë mënyrë krijuam grupin ID 1, ku të dyja Microt:bitet mund të komunikojnë.

.. |onstart| image:: ../_images/_imageMicroBit/s20.png

.. |radioset| image:: ../_images/_imageMicroBit/s22.png

.. image:: ../_images/_imageMicroBit/s24.png
      :align: center

SHENIM: Kur ne përdorim blloqet nga kategoria ``Radio`` do të ketë dy Micro:bit të shfaqura në simulues.

Variabli ``Counter`` ruan vlerën e marrë nga përdorimi i bllokut |select|, ose më saktë, variabli ``Counter`` merr një nga vlerat e rastit nga intervali 0 deri në 100.
Kur shtypet butoni A, biti Micro: dërgon vlerën e variablit ``Counter`` duke përdorur bllokun |send| nga kategoria |Radio|.

Pamja e kodit:

.. |pickrandom| image:: ../_images/_imageMicroBit/p49.png
.. |send| image:: ../_images/_imageMicroBit/s30.png

.. image:: ../_images/_imageMicroBit/p73.png
      :align: center

Kur informacioni dërgohet (në rastin tonë Counter), këto informacione duhet të merren. Bazuar në këtë informacion, përcaktohet ekzekutimi i programit (sheshi do të shfaqet nëse numri i marrë është i barabartë; përndryshe, do të shfaqet vlera e numrit të marrë). Për këtë, ne do të tërheqim një bllok nga kategoria |Radio|:

.. image:: ../_images/_imageMicroBit/p73.png
      :align: center

Në këtë bllok, ne do të tërheqim bllokun që përcakton variablin ``Remainder``, e cila ruan vlerën për ndarjen e plotë të ``Counter`` me 2:

.. image:: ../_images/_imageMicroBit/p64.png
      :align: center

Kjo pasohet nga blloku |ifthen|. Në pjesën |uslov| do të kontrollojmë nëse ka një pjesë të mbetur pas ndarjes së plotë të Counter me 2. Nëse kjo është e vërtetë, do të shfaqet një katror 3x3. Përndryshe, nëse kushti nuk është përmbushur, që do të thotë që pjesa tjetër nuk është 0, do të shfaqet vlera e variablit ``Counter``:

.. image:: ../_images/_imageMicroBit/p75.png
      :align: center

.. |ifthen| image:: ../_images/_imageMicroBit/s3.png
.. |uslov| image:: ../_images/_imageMicroBit/s5.png

Linku final i kodit:

.. image:: ../_images/_imageMicroBit/p76.png
      :align: center

Kinku për kodin: https://makecode.microbit.org/_f31EfHcv6Kpy

Për të provuar programin, ne do ta ekzekutojmë në simulator duke klikuar në butonin |play|.

.. |play| image:: ../_images/_imageMicroBit/p3.png

.. mchoice:: L8Z1
    :answer_a: Kur të dhënat janë marrë, asgjë nuk do të shfaqet.
    :answer_b: Kur të dhënat janë marrë, LED me koordinatat (2,2) do të ndizet.
    :answer_c: Kur të dhënat janë marrë, mesazhi "Përshëndetje" do të shfaqet.
    :feedback_a: Përgjigja është e saktë!
    :feedback_b: Përgjigja është e saktë!
    :feedback_c: Përgjigja është e saktë!
    :correct: a

    Studio blloqet me kujdes.

    .. image:: ../_images/_imageMicroBit/p77.png
          :align: center

    Çfarë do të shfaqet pas ekzekutimit të blloqeve më lart?

**Detyrë** Organizoni blloqet në mënyrë që ata të simulojnë funksionimin e një Telegrafi, më saktësisht kur sinjali (numri) dërgohet, LED-të ndizen në vende të zgjedhura rastësisht.

**Ndihmë e vogël:** Vlerat e koordinatave x dhe y janë nga intervali 0 deri në 4

Krahaso zgjidhjen tënde me një nga zgjidhjet tona: https://makecode.microbit.org/_JgFC5vRpudkq
