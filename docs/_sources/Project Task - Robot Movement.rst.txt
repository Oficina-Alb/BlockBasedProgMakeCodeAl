Detyrë - Lëvizja e robotit
================================

Ne do ta fillojmë aventurën tonë me një program të thjeshtë, i cili lejon që roboti të ecë përpara për 2 sekonda dhe pastaj të kthehet prapa për 2 sekonda.

Hapi i parë në shembullin tonë është fillimi i motorit. Duhet të zgjedhim bllokun |tankmotor| nga kategoria |Motors|, dhe e tërhiqim atë në sipërfaqen e punës dhe në bllokun |onstart|. Fillimisht, ne duhet të vendosim se në cilat porta do të lidhim motorët. Ne kemi përmendur tashmë se EV3 ka katër porta për motorë - A, B, C dhe D.

.. |tankmotor| image:: ../_images/_imageEV3/6.png
.. |Motors| image:: ../_images/_imageEV3/5.png
.. |start| image:: ../_images/_imageEV3/8.png

Në rastin tonë motorët janë të lidhur me portet B dhe C, dhe shpejtësia e tyre 50%. Meqenëse, bazuar në vendosjen e detyrës, roboti duhet të ecë përpara për 2 sekonda, duhet të klikojmë në shenjën plus në bllokun |tankmotor|, kjo do të na japë mundësinë për të zgjedhur mënyrën në të cilën lëviz roboti .

Në rastin tonë, duhet të zgjedhim opsionin "sekonda".

.. image:: ../_images/_imageEV3/7.png
      :align: center

Pas kësaj, ne duhet të rregullojmë kohëzgjatjen e lëvizjes së robotit duke shtypur 2 në fushën e hyrjes |broj|. Në këtë mënyrë, ne do të lejojmë që roboti të lëvizë për 2 sekonda.

.. |broj| image:: ../_images/_imageEV3/10.png

Pamja e kodit, e cila lejon që roboti të lëvizë për 2 sekonda:

.. image:: ../_images/_imageEV3/9.png
      :align: center

Më në fund, për të lejuar që roboti të lëvizë prapa, duhet të vendosim vlerën e shpejtësisë së motorit të jetë negative. Ne do ta vendosim vlerën në -50.

Pamja e kodit përfundimtar:

.. image:: ../_images/_imageEV3/11.png
      :align: center

Lidheni Brick EV3 me kompjuterin përmes kabllit USB dhe klikoni në butonin e shkarkimit të vendosur në fund të ekranit. Ndiqni udhëzimet se si të ruani programin në tullën EV3.

Shkarkoni skedarin .uf2 në kompjuterin tuaj duke klikuar butonin |dugme1|. Duke tërhequr skedarin mbi EV3, është gati të fillojë punën.

.. |dugme1| image:: ../_images/_imageEV3/download.png
      :width: 199px

Për të demonstruar se si lëviz roboti, do të japim një shembull tjetër të thjeshtë të një programi, i cili lejon që roboti të lëvizë nga vija e fillimit në vijën e mbarimit, dhe mbrapa. Distanca deri në fund është 50cm.

.. image:: ../_images/_imageEV3/11_.png
      :align: center

Bazuar në vendosjen e detyrës, roboti po ecën përpara 5 rotacione (360 degreed = 1 rotacion), prandaj, duhet të tërheqim bllokun |tankmotor| nga kategoria |Motors|, mbi sipërfaqen e punës dhe në bllokun |onstart|.

Në rastin tonë, motorët janë të lidhur me portet B dhe C me shpejtësi 50%. Meqenëse, bazuar në vendosjen e detyrës, roboti lëviz 5 rotacione, duhet të klikojmë në shenjën plus në bllok, i cili do të hapë mundësinë për të zgjedhur mënyrën në të cilën roboti do të lëvizë. Këtë herë, duhet të zgjedhim opsionin "rotation".
Pastaj, duhet të vendosim kohëzgjatjen e lëvizjes së robotit duke futur vlerën 5 në fushën e hyrjes. Në këtë mënyrë, roboti do të lëvizë për 5 rrotullime.

Pjesa e kodit, e cila lejon që roboti të lëvizë 5 rotacione:

.. image:: ../_images/_imageEV3/12.png
      :align: center

Ne do të përdorim bllokun për të rrotulluar robotin. Kthimi përcaktohet si ndryshim në shpejtësinë e një motori në raport me një motor tjetër, ose më saktë, nëse duam të bëjmë një kthesë të shpejtë ose të mprehtë në të djathtë, motori i majtë duhet të funksionojë të paktën dy herë më shpejt se sa djathtas. Në mënyrë që roboti të bëjë ndonjë lloj kthesash, duhet të përdorim fushën e hyrjes ``turn ratio``. Nëse duam që roboti të kthehet majtas, do të vendosim një vlerë negative, dhe nëse duam që ai të kthehet djathtas, do të vendosim një vlerë pozitive. Për të lejuar që roboti të kthehet nga vija e mbarimit në vijën e fillimit, ne do të përdorim të njëjtin bllok. Për të ndaluar funksionimin e të gjithë motorëve ne do të përdorim bllokun |blok1|.

.. |blok1| image:: ../_images/_imageEV3/14.png

Pamja e kodit, e cila lejon që roboti të lëvizë nga fillimi në vijën e mbarimit:

.. image:: ../_images/_imageEV3/15.png
      :align: center

Shkarkoni skedarin .uf2 në kompjuterin tuaj duke klikuar butonin |dugme1|. Duke tërhequr skedarin mbi EV3, është gati të fillojë punën.
