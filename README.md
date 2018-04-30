<?php
  $diretorio = 'admin/';
  $extensao = '.php';

  if( isset($_GET['pagina']) )
  {
    $pagina = ($_GET['pagina']);
  }
  else
  {
    $pagina = "index";
  }

  if(file_exists($dir.$pagina.$ext))
  {
    include($dir.$pagina.$ext);
  }
  else
  {
    echo "Página não encontrada!";
  }
?>
