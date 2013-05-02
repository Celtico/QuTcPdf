QuTcPdf 0.0.1-dev:
========================

ZF2 module for TcPdf

Release Notes
========================

0.0.1-dev:

- Initiation TcPdf in zf2

Requirements
========================
- ZendSkeletonApplication https://github.com/zendframework/ZendSkeletonApplication

Installation
========================
- Drag a folder into modules folder or vendor folder
- Enable the module application.config.php

Installation by Composer
========================
See the information if not known composer and clone git
=========================================================
- http://git-scm.com
- http://getcomposer.org

```
cd YourFolderProject/
php composer.phar require "qu-modules/qu-tcpdf":"dev-master"
```

Integration
========================
```php
  $sm  = $this->getServiceLocator();
  $pdf = $sm->get('QuTcPdf');
  $pdf = $pdf->MyPdf();

  $pdf->setHeaderData($ln = 0,$lw = 0,$ht = 0,$hs = 0,$tc = array(255,255,255),$lc = array(255,255,255));
  $pdf->setFooterData($tc = array(255,255,255),$lc = array(255,255,255));
  $pdf->setPageOrientation($orientation='P', $autopagebreak='L', $bottommargin=-200);

  foreach($pages as $page){

    $pdf->AddPage();

    //Your function
    $this->multiPag($pdf,$page);

    $pdf->lastPage();

  }

  $pdf->Output('test.pdf','I');
```

References usage and conditions in TcPdf
========================
- View read me in QuTcPdf/src/TcPdf
