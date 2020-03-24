Micro:bit – Karakteristika bazike dhe komponentë
==========================================

Para se të fillojmë mësimin e Programimit Micro:bit përmes MakeCode, le të njihemi me përbërësit themelorë dhe tiparet e Micro:bit dhe mjedisin e punës.

Micro:bit – Karakteristika bazike dhe komponentë
:::::::::::::::::::::::::::::::::::::::::

Micro:bit është një kompjuter portativ, i programueshëm për përdoruesin, i cili ka një procesor 32-bitësh ARM Cortex-M0 që punon në 16MHz me vetëm memorie RAM 16KB, si dhe sensorë dhe një ekran të bërë nga 25 LED. Ka lidhës, pesë hyrje dhe dalje (I / O) të përdorura për të lidhur Micro:bit me pajisje ose sensorë të tjerë, ai gjithashtu ka Bluetooth, dhe është i mundësuar nga dy bateri AA.
Më e rëndësishmja, ajo ka aftësinë për të programuar.

.. image:: ../_images/_imageMicroBit/0.png
      :align: center

Micro: bit përbëhet nga përbërësit fizikë të mëposhtëm:

- 25 LED, të cilat janë individualisht të programueshme

- 2 butona të programueshëm të etiketuar A dhe B

- kunjat e lidhjes

- Sensorë të temperaturës dhe dritës

- Sensorë lëvizjeje (akselerometri dhe busulla)

- Komunikim pa tel përmes radio dhe Bluetooth

- Ndërfaqe USB

- Butoni i rivendosjes

**Dioda e lëshimit të dritës (LED)**

**Light Emitting Diode (LED)**

.. image:: ../_images/_imageMicroBit/60.png
      :width: 192px
      :align: center


Light Emitting Diode (LED) është një diodë, e cila lëshon dritë. Micro:bit ka 25 LED (rregulluar në një rrjet 5x5), ato janë individualisht të programueshme dhe në varësi të programit, ata mund të shfaqin tekst, numra dhe imazhe.

**Butonat A and B**

.. image:: ../_images/_imageMicroBit/66.png
      :align: center


Në pjesën e përparme të pajisjes Micro:bit, ka dy butona (të etiketuar A dhe B). Shtypja e secilit buton individualisht ose të dy butonave njëkohësisht shkakton kodin në pajisje.

**Pins**

.. image:: ../_images/_imageMicroBit/67.png
      :align: center


Ato përdoren për të lidhur Micro:bit me pajisje ose sensorë të tjerë.

**Sensorët e dritës**

.. image:: ../_images/_imageMicroBit/63.png
      :align: center


LED janë vendosur në pjesën e përparme të Micro:bit. Në këtë rast, ata luajnë pjesën e një pajisje hyrëse. Ekrani LED funksionon si një sensor themelor i dritës, i cili mund të zbulojë intensitetin e dritës së ambientit.

**Sensori i Temperaturës**

.. image:: ../_images/_imageMicroBit/65.png
      :width: 192px
      :align: center


Sensori i temperaturës lejon Micro:bit të zbulojë temperaturën aktuale të ambientit, në gradë Celsius.

**Akselerometri**

.. image:: ../_images/_imageMicroBit/68.png
      :align: center


Akselerometri - është përbërësi që regjistron lëvizjet, ndryshimet në shpejtësinë dhe pozicionin, domethënë është e mundur të matni shpejtësinë e lëvizjes. Me këtë komponent, Micro:bit regjistrohet kur është zhvendosur. Është gjithashtu e mundur të zbulohen veprime të tjera, të tilla si lëkundja, pjerrësia ose rënia e lirë.

**Kompas**

.. image:: ../_images/_imageMicroBit/68.png
      :align: center


Kjo busull zbulon fushën magnetike të tokës, e cila na lejon të zbulojmë se në cilin drejtim është përballur Micro: bit. Busulla duhet të kalibrohet para se të përdoret. "Kalibrimi" i busullës siguron një lexim të saktë të drejtimit. Kur të fillojë kalibrimi, Micro:bit do të shfaq udhëzimin "Vizato një rreth" ose "vizato për të mbushur ekranin". Për të bërë kalibrimin e busullës, do të duhet të ndiqni udhëzimin dhe ta rrotulloni Micro:bit në një rreth për të lëvizur pikën në qendër të ekranit derisa të shfaqet skica e rrethit ose të gjithë ekranin të mbushet me pika.

**Radio dhe Bluetooth**

.. image:: ../_images/_imageMicroBit/65_.png
      :width: 192px
      :align: center


Komponenti i radios mundëson komunikim pa tel midis dy ose më shumë Micro:bit. Radioja mund të përdoret për dërgimin e mesazheve në Micro:bit, krijimin e lojërave multiplayer, kuize dhe të ngjashme. Antena Bluetooth Low Energy (BLE) lejon që Micro:bit të dërgojë dhe të marrë sinjale Bluetooth, d.m.th. të komunikojë pa tel me kompjuterë, telefona celularë dhe tableta.

**Ndërfaqja USB**

.. image:: ../_images/_imageMicroBit/69.png
      :align: center


Sensori i temperaturës lejon Micro:bit të zbulojë temperaturën aktuale të ambientit, në gradë Celsius.

Ambjenti i punës
::::::::::::::::::

Ne mund të fillojmë mjedisin e punës përmes shfletuesit tonë duke shkuar në faqen web https://makecode.microbit.org.

Hapim një projek të ri duke klikuar butonin New Project |newproject|.

.. |newproject| image:: ../_images/_imageMicroBit/p1.png
    :width: 90px


Ky redaktues në internet ofron mundësinë e kodimit në JavaScript ose programim bllok, ku komandat janë grumbulluar duke përdorur teknikën "drag and drop". Ne do të merremi me programimin e bllokut.

Mjedisi në internet Micro: bit në redaktorin MakeCode ka një simulator (1) në anën e majtë, i cili drejton programin menjëherë pasi të jetë shkruar; prandaj, përmes vizualizimit, përdoruesi mund të zbulojë lehtësisht gabimet, të cilat mund të ndodhin në program. Në mes të mjedisit të uebit ekziston një menu (2) ku komandat janë rregulluar në grupe. Në anën e djathtë, ekziston një zonë pune (3) ku mund të tërhiqni komanda dhe të ndërtoni programe.

.. image:: ../_images/_imageMicroBit/2.png
      :align: center

Kur fillon një projekt i ri, dy blloqe shfaqen në sipërfaqen e punës MakeCode: në fillim dhe përgjithmonë. Blloku|forever|  është një nga blloqet nga kategoria basic, dhe blloqet që vendosen në të ekzekutohen vetëm një herë gjatë ekzekutimit të programit. Ndërsa blloku | përgjithmonë | është një bllok brenda të cilit komandat do të ekzekutohen një herë të pafundme. Drejtimi i këtij blloku nuk ndalet kurrë më vete. Ai do të përfundojë kur përdoruesi klikon butonin e ndalimit të programit (|stop|).
Në MakeCode, programet përbëhen nga blloqe të ndryshme të lidhura. Blloqet (komandat) ndahen në kategori, të cilat kanë qëllime të ndryshme.

.. |stop| image:: ../_images/_imageMicroBit/p2.png
.. |onstart| image:: ../_images/_imageMicroBit/s20.png
.. |forever| image:: ../_images/_imageMicroBit/s1.png

.. image:: ../_images/_imageMicroBit/3_.png
      :align: center

Emri i kategorisë (p.sh. ``Music``) i tregon përdoruesit se cili lloj i komandave (blloqeve) përfshihet në atë kategori specifike. Të gjitha blloqet që i përkasin një kategorie janë të njëjtën ngjyrë.
Çdo bllok tërhiqet në sipërfaqen e punës dhe lidhet me blloqe të tjera në një mënyrë të përcaktuar nga programi, i cili është duke u krijuar.

Duke klikuar me të djathtën në një bllok hapet një menu drop-down që përmban opsionin i cili ju lejon të krijoni kopje (``Copy``), shtoni komente (``Ad Comment``), fshini blloqe (``Delete Block``) , si dhe opsionin me të cilin mund të hapni seksionin e informacionit për ndihmë shtesë në lidhje me blloqe të caktuara (``Help``).

.. image:: ../_images/_imageMicroBit/4_.png
      :align: center


Para se të fillojmë krijimin e projekteve interesante duke përdorur pajisje Micro:bit, ne do të përpiqemi të njihemi me bazat e programimit në mjedisin e punës MakeCode.

.. toctree::
   :maxdepth: 2

   Blocks from the Basic Category.rst
   Working with Blocks from the Input Category.rst
   Blocks from the Music Category.rst
   Working with Blocks from the Led Category.rst
   Working with Blocks from the Math and Variables Categories.rst
   Working with Blocks from the Logic Category.rst
   Working with Blocks from the Loops Category.rst
   Working with Blocks from the Radio Category.rst


Projekte
:::::::::

Në mësimet e mëposhtme, ne do të prezantojmë disa projekte interesante që lidhen me Micro:bit duke përdorur platformën MakeCode.
Të gjitha projektet bëhen hap pas hapi, kështu që të gjithë mund t'i bëjnë përsëri. Të gjitha procedurat për ndërtimin e projekteve janë shtjelluar, nga mënyra se si është krijuar pajisja deri në atë se si krijohet dhe testohet programi.

.. toctree::
   :maxdepth: 2
   
   Project Task - the Bracelet.rst
   Project Task - the Singing Fruits.rst
   Project Task - the Traffic Light.rst
   Project Task - the House Alarm.rst
   Project Task - the Wire.rst
