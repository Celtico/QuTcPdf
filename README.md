QuTcPdf 1.0.0
========================

ZF2 module for TcPdf

Release Notes
========================

1.0.0-dev:

- Initiation TcPdf in zf2

Requirements
========================
- ZendSkeletonApplication https://github.com/zendframework/ZendSkeletonApplication

Installation
========================
- Drag a folder into modules folder or vendor folder
- Enable the module application.config.php

### Composer / Packagist
```
% composer.phar require qu/elfinder
Please provide a version constraint for the qu/elfinder requirement: 1.0.0-dev
```

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
