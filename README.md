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

In my experience, to avoid errors

- cd /Users/YourName/Desktop/YourFolderProject/
- /Applications/YourSever/bin/php/php5.3.6/bin/php /Users/YourName/Desktop/YourFolderProject/composer.phar install

In the errors check and install

- http://git-scm.com/downloads
- http://getcomposer.org/download

Integration
========================
```php
  $sm  = $this->getServiceLocator();
  $pdf = $sm->get('QuTcPdf');
  $pdf = $pdf->MyPdf();
  $pdf->Output('test.pdf','I');
```

References usage and conditions in TcPdf
========================
- View read me in QuTcPdf/src/TcPdf
