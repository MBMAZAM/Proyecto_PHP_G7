# Proyecto_PHP
carpeta vista

pantalla de inicio

<?php 
require_once('include/session.php'); 
$home_menu=1;
?>

<!DOCTYPE html>
<html lang="en">

<head>

    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="description" content="">
    <meta name="author" content="">

    <title>Inicio - Sistema de Inventario Farmacéutico </title>

  
    <link href="assets/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" type="text/css" href="assets/css/bootstrap-theme.min.css">

   
    <link href="assets/css/sb-admin.css" rel="stylesheet">

    
    <link href="assets/css/plugins/morris.css" rel="stylesheet">

  
    <link href="assets/font-awesome/css/font-awesome.min.css" rel="stylesheet" type="text/css">

    <link href="assets/css/dataTables.bootstrap.min.css" rel="stylesheet">
</head>

<body>

    <div id="wrapper">

      
        <?php include('navbar.php');?>

        <div id="page-wrapper">

            <div class="container-fluid">

              
                <div class="row">
                    <div class="col-lg-12">
                        <h1 class="page-header">
                            Bienvenid@ <small>Administrador</small>
                        </h1>
                        <ol class="breadcrumb">
                            <li class="active">
                                <i class="fa fa-home"></i> Inicio
                            </li>
                        </ol>
                    </div>
                </div>
              
                <div id="order"></div>         
               
            </div>
          

        </div>
       

    </div>
    


<?php include_once('modal/to_cart.php'); ?>
<?php include_once('modal/confirmation.php'); ?>
<?php include_once('modal/add_new_item.php'); ?>
<?php include_once('modal/message.php'); ?>

    <script type="text/javascript" src="assets/js/jquery-3.1.1.min.js"></script>
    <script type="text/javascript" src="assets/js/jquery-1.12.3.js"></script>
    <script type="text/javascript" src="assets/js/bootstrap.min.js"></script>
    <script type="text/javascript" src="assets/js/jquery.dataTables.min.js"></script>
    <script type="text/javascript" src="assets/js/dataTables.bootstrap.min.js"></script>
    <script type="text/javascript" src="assets/js/regis.js"></script>

</body>

</html>


index.php



<!DOCTYPE html>
<html >
  <head>
    <meta charset="UTF-8">
    <title>Sistema de Inventario Farmacéutico</title>
	
    
        <link rel="stylesheet" href="assets/css/style.css">

    
  </head>

  <body style="background: #262626;">
  <br/>
  <br/>    
    
  

    <div class="container">

  <div id="login-form">

    <h3>Iniciar sesión
</h3>

    <fieldset>

      <form id="form-login">
        <input type="text" autofocus id="un" placeholder="Usuario" required autocomplete="off"> 

        <input type="password" id="up" placeholder="Contraseña" required autocomplete="off">  

        <input type="submit" name="log" value="Ingresar">
      </form>

    </fieldset>

  </div> 

</div>
    
    
    
<script type="text/javascript" src="assets/js/jquery-1.12.3.js"></script>
<script type="text/javascript" src="assets/js/bootstrap.min.js"></script>
<script type="text/javascript" src="assets/js/regis.js"></script>

    
  </body>
</html>

index.php

<?php 
require_once('include/session.php'); 
$item_menu=1;
?>
<!DOCTYPE html>
<html lang="en">

<head>

    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="description" content="">
    <meta name="author" content="">

    <title> Lista de productos - Sistema de Inventario Farmacéutico</title>

   
    <link href="assets/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" type="text/css" href="assets/css/bootstrap-theme.min.css">

    
    <link href="assets/css/sb-admin.css" rel="stylesheet">

    
    <link href="assets/css/plugins/morris.css" rel="stylesheet">

    
    <link href="assets/font-awesome/css/font-awesome.min.css" rel="stylesheet" type="text/css">

    <link href="assets/css/dataTables.bootstrap.min.css" rel="stylesheet">


</head>

<body>

    <div id="wrapper">

       
        <?php include('navbar.php');?>

        <div id="page-wrapper">

            <div class="container-fluid">

              
                <div class="row">
                    <div class="col-lg-12">
                        <h1 class="page-header">
                        </h1>
                    </div>
                </div>
              
                <button class="btn btn-default" id="add-new-item">Agregar producto
                    <span class="glyphicon glyphicon-plus-sign" aria-hidden="true"></span>
                </button>
               <div id="all-item"></div>

            </div>
           

        </div>
     

    </div>
  

<?php include_once('modal/add_new_item.php'); ?>
<?php include_once('modal/message.php'); ?>

<script type="text/javascript" src="assets/js/jquery-3.1.1.min.js"></script>
<script type="text/javascript" src="assets/js/jquery-1.12.3.js"></script>
<script type="text/javascript" src="assets/js/bootstrap.min.js"></script>
<script type="text/javascript" src="assets/js/jquery.dataTables.min.js"></script>
<script type="text/javascript" src="assets/js/dataTables.bootstrap.min.js"></script>
<script type="text/javascript" src="assets/js/regis.js"></script>


</body>

</html>


navbar.php

<nav class="navbar navbar-inverse navbar-fixed-top" role="navigation">
           
            <div class="navbar-header">
                <button type="button" class="navbar-toggle" data-toggle="collapse" data-target=".navbar-ex1-collapse">
                    <span class="sr-only">Toggle navigation</span>
                    <span class="icon-bar"></span>
                    <span class="icon-bar"></span>
                    <span class="icon-bar"></span>
                </button>
                <a class="navbar-brand" href="index.html">FARMACIA R&G </a>
            </div>
         
            <ul class="nav navbar-right top-nav">
                <li class="dropdown">
                    <a href="#" class="dropdown-toggle" data-toggle="dropdown"><i class="fa fa-user"></i>  Administrador <b class="caret"></b></a>
                    <ul class="dropdown-menu">
                        <li>
                            <a href="#"><i class="fa fa-fw fa-gear"></i> Configuración</a>
                        </li>
                        <li class="divider"></li>
                        <li>
                            <a href="logout.php"><i class="fa fa-fw fa-power-off"></i> Salir</a>
                        </li>
                    </ul>
                </li>
            </ul>
           
            <div class="collapse navbar-collapse navbar-ex1-collapse">
                <ul class="nav navbar-nav side-nav">
                    <li class="<?php if (isset($home_menu)){echo "active";}?>">
                        <a href="home.php"><span class="glyphicon glyphicon-home" aria-hidden="true"></span></i> Inicio</a>
                    </li>
                    <li class="<?php if (isset($item_menu)){echo "active";}?>">
                        <a href="item.php"><span class="glyphicon glyphicon-list" aria-hidden="true"></span> Lista de productos</a>
                    </li>
                    <li class="<?php if (isset($products_menu)){echo "active";}?>">
                        <a href="product.php"><span class="glyphicon glyphicon-th-list" aria-hidden="true"></span> Perfil del producto</a>
                    </li>
                    <li class="<?php if (isset($stock_menu)){echo "active";}?>">
                        <a href="stock.php"><span class="glyphicon glyphicon-book" aria-hidden="true"></span> Inventario</a>
                    </li>
                   
                    <li class="<?php if (isset($sales_menu)){echo "active";}?>">
                        <a href="sales.php"><span class="glyphicon glyphicon-record" aria-hidden="true"></span> Ventas</a>
                    </li>
                </ul>
            </div>
           
        </nav>

product.php

<?php 
	require_once('include/session.php'); 
	$products_menu=1;
?>
<!DOCTYPE html>
<html lang="en">

<head>

    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="description" content="">
    <meta name="author" content="">

    <title>Lista de productos - Sistema de Inventario Farmacéutico</title>

  
    <link href="assets/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" type="text/css" href="assets/css/bootstrap-theme.min.css">

   
    <link href="assets/css/sb-admin.css" rel="stylesheet">

   
    <link href="assets/css/plugins/morris.css" rel="stylesheet">

   
    <link href="assets/font-awesome/css/font-awesome.min.css" rel="stylesheet" type="text/css">

    <link href="assets/css/dataTables.bootstrap.min.css" rel="stylesheet">


</head>

<body>

    <div id="wrapper">

      
        <?php include("navbar.php");?>

        <div id="page-wrapper">

            <div class="container-fluid">

              
                <div class="row">
                    <div class="col-lg-12">
                        <h1 class="page-header">
                        </h1>
                    </div>
                </div>
               
                <button class="btn btn-default" id="add-stock">Agregar inventario
                    <span class="glyphicon glyphicon-plus-sign" aria-hidden="true"></span>
                </button>

                <button class="btn btn-danger" id="del-stock">Borrar seleccionados
                    <span class="glyphicon glyphicon-trash" aria-hidden="true"></span>
                </button>

               <div id="all-stocklist"></div>

            </div>
           

        </div>
       

    </div>
    


<?php include_once('modal/stock.php'); ?>
<?php include_once('modal/confirmation.php'); ?>
<?php include_once('modal/message.php'); ?>

<script type="text/javascript" src="assets/js/jquery-3.1.1.min.js"></script>
<script type="text/javascript" src="assets/js/jquery-1.12.3.js"></script>
<script type="text/javascript" src="assets/js/bootstrap.min.js"></script>
<script type="text/javascript" src="assets/js/jquery.dataTables.min.js"></script>
<script type="text/javascript" src="assets/js/dataTables.bootstrap.min.js"></script>
<script type="text/javascript" src="assets/js/regis.js"></script>


</body>

</html>


sales.php

<?php
	require_once('include/session.php'); 
	$sales_menu=1;	
?>
<!DOCTYPE html>
<html lang="en">

<head>

    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="description" content="">
    <meta name="author" content="">

    <title>Ventas -  Sistema de Inventario Farmacéutico</title>

   
    <link href="assets/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" type="text/css" href="assets/css/bootstrap-theme.min.css">

   
    <link href="assets/css/sb-admin.css" rel="stylesheet">

    
    <link href="assets/css/plugins/morris.css" rel="stylesheet">

    
    <link href="assets/font-awesome/css/font-awesome.min.css" rel="stylesheet" type="text/css">

    <link href="assets/css/dataTables.bootstrap.min.css" rel="stylesheet">


</head>

<body>

    <div id="wrapper">

       
        <?php include("navbar.php");?>

        <div id="page-wrapper">

            <div class="container-fluid">

               
                <div class="row">
                    <div class="col-lg-12">
                        <h1 class="page-header">
                        </h1>
                    </div>
                </div>
               
                <strong>Ventas diarias:</strong>
                <input id="dailyDate" type="date" class="btn btn-default btn-sm" placeholder=""
                value="<?= date('Y-m-d'); ?>">
            
                <div id="printBut" class="pull-right">
                <button type="button" class="btn btn-success btn-sm">
                    Imprimir
                    <span class="glyphicon glyphicon-print" aria-hidden="true"></span>
                </button>
                </div>
               
               <div id="all-sales"></div>

            </div>
           

        </div>
       

    </div>
    

<script type="text/javascript" src="assets/js/jquery-1.12.3.js"></script>
<script type="text/javascript" src="assets/js/jquery-3.1.1.min.js"></script>
<script type="text/javascript" src="assets/js/bootstrap.min.js"></script>
<script type="text/javascript" src="assets/js/jquery.dataTables.min.js"></script>
<script type="text/javascript" src="assets/js/dataTables.bootstrap.min.js"></script>
<script type="text/javascript" src="assets/js/regis.js"></script>


</body>

</html>

stock.php

<?php
 require_once('include/session.php'); 
 $stock_menu=1;
 ?>
<!DOCTYPE html>
<html lang="en">

<head>

    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="description" content="">
    <meta name="author" content="">

    <title>Inventario -  Sistema de Inventario Farmacéutico</title>

    
    <link href="assets/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" type="text/css" href="assets/css/bootstrap-theme.min.css">

    
    <link href="assets/css/sb-admin.css" rel="stylesheet">

    
    <link href="assets/css/plugins/morris.css" rel="stylesheet">

   
    <link href="assets/font-awesome/css/font-awesome.min.css" rel="stylesheet" type="text/css">

    <link href="assets/css/dataTables.bootstrap.min.css" rel="stylesheet">


</head>

<body>

    <div id="wrapper">

       
        <?php include ("navbar.php")?>

        <div id="page-wrapper">
            <div class="container-fluid">
               
                <div class="row">
                    <div class="col-lg-12">
                        <h1 class="page-header">
                        </h1>
                    </div>
                </div>
               
                <button class="btn btn-success btn-sm" id="stock-report">IMPRIMIR
                    <span class="glyphicon glyphicon-print" aria-hidden="true"></span>
                </button>
               <div id="all-stock"></div>

            </div>
           
        </div>
       

    </div>
   


<?php include_once('modal/confirmation.php'); ?>
<?php include_once('modal/message.php'); ?>

<script type="text/javascript" src="assets/js/jquery-3.1.1.min.js"></script>
<script type="text/javascript" src="assets/js/jquery-1.12.3.js"></script>
<script type="text/javascript" src="assets/js/bootstrap.min.js"></script>
<script type="text/javascript" src="assets/js/jquery.dataTables.min.js"></script>
<script type="text/javascript" src="assets/js/dataTables.bootstrap.min.js"></script>
<script type="text/javascript" src="assets/js/regis.js"></script>


</body>

</html>

logout.php

<?php 
if(session_status() == PHP_SESSION_NONE)
{
	session_start();
}

unset($_SESSION['logged_id']);
unset($_SESSION['logged_type']);

if(!isset($_SESSION['logged_id'])){
	header('location: index.php');
}


home.php

<?php 
require_once('include/session.php'); 
$home_menu=1;
?>

<!DOCTYPE html>
<html lang="en">

<head>

    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="description" content="">
    <meta name="author" content="">

    <title>Inicio - Sistema de Inventario Farmacéutico </title>

  
    <link href="assets/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" type="text/css" href="assets/css/bootstrap-theme.min.css">

   
    <link href="assets/css/sb-admin.css" rel="stylesheet">

    
    <link href="assets/css/plugins/morris.css" rel="stylesheet">

  
    <link href="assets/font-awesome/css/font-awesome.min.css" rel="stylesheet" type="text/css">

    <link href="assets/css/dataTables.bootstrap.min.css" rel="stylesheet">
</head>

<body>

    <div id="wrapper">

      
        <?php include('navbar.php');?>

        <div id="page-wrapper">

            <div class="container-fluid">

              
                <div class="row">
                    <div class="col-lg-12">
                        <h1 class="page-header">
                            Bienvenid@ <small>Administrador</small>
                        </h1>
                        <ol class="breadcrumb">
                            <li class="active">
                                <i class="fa fa-home"></i> Inicio
                            </li>
                        </ol>
                    </div>
                </div>
              
                <div id="order"></div>         
               
            </div>
          

        </div>
       

    </div>
    


<?php include_once('modal/to_cart.php'); ?>
<?php include_once('modal/confirmation.php'); ?>
<?php include_once('modal/add_new_item.php'); ?>
<?php include_once('modal/message.php'); ?>

    <script type="text/javascript" src="assets/js/jquery-3.1.1.min.js"></script>
    <script type="text/javascript" src="assets/js/jquery-1.12.3.js"></script>
    <script type="text/javascript" src="assets/js/bootstrap.min.js"></script>
    <script type="text/javascript" src="assets/js/jquery.dataTables.min.js"></script>
    <script type="text/javascript" src="assets/js/dataTables.bootstrap.min.js"></script>
    <script type="text/javascript" src="assets/js/regis.js"></script>

</body>

</html>


carpeta modal

add_new_item.php
<?php 
require_once('database/Database.php');
$db = new Database();
$sql = "SELECT *
		FROM item_type
		ORDER BY item_type_desc ASC";
$types = $db->getRows($sql);

 ?>
<div class="modal fade" id="modal-item">
	<div class="modal-dialog">
		<div class="modal-content">
			<div class="modal-header">
				<button type="button" class="close" data-dismiss="modal" aria-hidden="true">&times;</button>
				<h4 class="modal-title">Modal title</h4>
			</div>
			<div class="modal-body">
			
				<form class="form-horizontal" role="form" id="form-item">
				<input type="hidden" id="item-id">
				  <div class="form-group">
				    <label class="control-label col-sm-3" for="">Nombre del producto:</label>
				    <div class="col-sm-9">
				      <input type="text" maxlength="50" class="form-control" id="item-name" placeholder="Ingresa el nombre generico" required="" autofocus="">
				    </div>
				  </div>
				  <div class="form-group">
				    <label class="control-label col-sm-3" for="">Precio:</label>
				    <div class="col-sm-9"> 
				      <input type="number" min="0.1" step="any" class="form-control" id="item-price" placeholder="Ingresa el precio" required="">
				    </div>
				  </div>

				  <div class="form-group">
				    <label class="control-label col-sm-3" for="">Código:</label>
				    <div class="col-sm-9">
				      <input type="text" maxlength="50" class="form-control" id="code" placeholder="Ingresa el código" required="" autofocus="">
				    </div>
				  </div>

				  <div class="form-group">
				    <label class="control-label col-sm-3" for="">Fabricante:</label>
				    <div class="col-sm-9">
				      <input type="text" maxlength="50" class="form-control" id="brand" placeholder="Ingresa el fabricante" required="" autofocus="">
				    </div>
				  </div>

				  <div class="form-group">
				    <label class="control-label col-sm-3" for="">Gramos:</label>
				    <div class="col-sm-9">
				      <input type="text" maxlength="50" class="form-control" id="grams" placeholder="Ingresa los gramos" required="" autofocus="">
				    </div>
				  </div>

				  <div class="form-group">
				    <label class="control-label col-sm-3" for="">Tipo:</label>
				    <div class="col-sm-9"> 
				      <select id="item-type" class="btn btn-default">
				      	<?php foreach($types as $t): ?>
				      		<option value="<?= $t['item_type_id']; ?>"><?= ucwords($t['item_type_desc']); ?></option>
				      	<?php endforeach; ?>
				      </select>
				    </div>
				  </div>
				  <div class="form-group"> 
				    <div class="col-sm-offset-2 col-sm-10">
				      <button type="submit" id="submit-item" value="add" class="btn btn-default">Guardar datos
				      <span class="glyphicon glyphicon-save" aria-hidden="true"></span>
				      </button>
				    </div>
				  </div>
				</form>
				
			</div>
			<div class="modal-footer">
			</div>
		</div>
	</div>
</div>
<?php 
$db->Disconnect();
 ?>
 
confirmacion.php

<div class="modal fade" id="modal-confirmation">
	<div class="modal-dialog">
		<div class="modal-content">
			<div class="modal-header">
				<button type="button" class="close" data-dismiss="modal" aria-hidden="true">&times;</button>
				<h4 class="modal-title text-danger">Estas seguro?</h4>
			</div>
			<div class="modal-body">
				<div align="center">
						<strong class="text-danger">
							<div id="remove-stud-msg">
								<h1></h1>
							</div>
						</strong>
						<input type="hidden" id="confirm-type" value="null">
						<button id="confirm-yes" type="button" class="btn btn-default btn-lg del-expired" >Aceptar
							<span class="glyphicon glyphicon-ok" aria-hidden="true"></span>
						</button>
						&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
						<button type="button" class="btn btn-default btn-lg" data-dismiss="modal" >Cancelar
							<span class="glyphicon glyphicon-remove" aria-hidden="true"></span>
						</button>	
				</div>
			</div>
			<div class="modal-footer">
			</div>
		</div>
	</div>
</div>

message.php

 <div class="modal fade" id="modal-message">
	<div class="modal-dialog">
		<div class="modal-content">
			<div class="modal-header">
				<button type="button" class="close" data-dismiss="modal" aria-hidden="true">&times;</button>
				<h4 class="modal-title">Caja de mensajes</h4>
			</div>
			<div class="modal-body">
				<h4 id="msg-body">Todo bien</h4>
			</div>
			<div class="modal-footer">
				<button type="button" id="message-box-ok" class="btn btn-default" data-dismiss="modal">OK
				<span class="glyphicon glyphicon-ok" aria-hidden="true"></span>
				</button>
			</div>
		</div>
	</div>
</div>

stock.php

<?php 
	require_once('database/Database.php');
	$db = new Database();
	
	$sql = "SELECT *
			FROM item 
			ORDER BY item_name ASC";
	$items = $db->getRows($sql);
 ?>
<div class="modal fade" id="modal-stock">
	<div class="modal-dialog">
		<div class="modal-content">
			<div class="modal-header">
				<button type="button" class="close" data-dismiss="modal" aria-hidden="true">&times;</button>
				<h4 class="modal-title">Modal title</h4>
			</div>
			<div class="modal-body">
				
				<form class="form-horizontal" role="form" id="form-stock">
				  <div class="form-group">
				    <label class="control-label col-sm-3" for="">Producto:</label>
				    <div class="col-sm-9">
					    <select class="btn btn-default" id="item-id">
					    	<?php foreach($items as $i): ?>
					    		<option value="<?= $i['item_id']; ?>"><?= ucwords($i['item_name']); ?></option>
					    	<?php endforeach; ?>
					    </select>
				    </div>
				  </div>
				  <div class="form-group">
				    <label class="control-label col-sm-3" for="">Cantidad:</label>
				    <div class="col-sm-9"> 
				      <input type="number" min="1" class="form-control" id="qty" placeholder="Ingresa la cantidad" required="">
				    </div>
				  </div>

				  <div class="form-group">
				    <label class="control-label col-sm-3" for="">Vence:</label>
				    <div class="col-sm-9"> 
				      <input type="date" class="form-control" id="xDate" required="">
				    </div>
				  </div>

				  <div class="form-group">
				    <label class="control-label col-sm-3" for="">Fabricado:</label>
				    <div class="col-sm-9"> 
				      <input type="date" class="form-control" id="manu" required="">
				    </div>
				  </div>

				  <div class="form-group">
				    <label class="control-label col-sm-3" for="">Comprado:</label>
				    <div class="col-sm-9"> 
				      <input type="date" class="form-control" id="purc" required="">
				    </div>
				  </div>


				  <div class="form-group"> 
				    <div class="col-sm-offset-3 col-sm-9">
				      <button type="submit" class="btn btn-default">Guardar datos
				      <span class="glyphicon glyphicon-ok" aria-hidden="true"></span>
				      </button>
				    </div>
				  </div>
				</form>
				
			</div>
			<div class="modal-footer">
			</div>
		</div>
	</div>
</div>

to_cart.php

<?php 
	require_once('database/Database.php');
	$db = new Database();
	
	$sql = "SELECT *
			FROM item 
			ORDER BY item_name ASC";
	$items = $db->getRows($sql);
 ?>
<div class="modal fade" id="modal-stock">
	<div class="modal-dialog">
		<div class="modal-content">
			<div class="modal-header">
				<button type="button" class="close" data-dismiss="modal" aria-hidden="true">&times;</button>
				<h4 class="modal-title">Modal title</h4>
			</div>
			<div class="modal-body">
				
				<form class="form-horizontal" role="form" id="form-stock">
				  <div class="form-group">
				    <label class="control-label col-sm-3" for="">Producto:</label>
				    <div class="col-sm-9">
					    <select class="btn btn-default" id="item-id">
					    	<?php foreach($items as $i): ?>
					    		<option value="<?= $i['item_id']; ?>"><?= ucwords($i['item_name']); ?></option>
					    	<?php endforeach; ?>
					    </select>
				    </div>
				  </div>
				  <div class="form-group">
				    <label class="control-label col-sm-3" for="">Cantidad:</label>
				    <div class="col-sm-9"> 
				      <input type="number" min="1" class="form-control" id="qty" placeholder="Ingresa la cantidad" required="">
				    </div>
				  </div>

				  <div class="form-group">
				    <label class="control-label col-sm-3" for="">Vence:</label>
				    <div class="col-sm-9"> 
				      <input type="date" class="form-control" id="xDate" required="">
				    </div>
				  </div>

				  <div class="form-group">
				    <label class="control-label col-sm-3" for="">Fabricado:</label>
				    <div class="col-sm-9"> 
				      <input type="date" class="form-control" id="manu" required="">
				    </div>
				  </div>

				  <div class="form-group">
				    <label class="control-label col-sm-3" for="">Comprado:</label>
				    <div class="col-sm-9"> 
				      <input type="date" class="form-control" id="purc" required="">
				    </div>
				  </div>


				  <div class="form-group"> 
				    <div class="col-sm-offset-3 col-sm-9">
				      <button type="submit" class="btn btn-default">Guardar datos
				      <span class="glyphicon glyphicon-ok" aria-hidden="true"></span>
				      </button>
				    </div>
				  </div>
				</form>
				
			</div>
			<div class="modal-footer">
			</div>
		</div>
	</div>
</div>

carpeta interface

icart.php

<?php 
interface iCart{
	public function add_toCart($item_id, $qty, $stock_id, $user_id, $uniqid);
	public function all_cartDatas($user_id);
	public function delCart($cart_id); 
	public function dellAllCart();
	public function allCart();
}

iexpired.php

<?php 
interface iExpired{
	public function add_expired($name, $price, $qty, $expiredDate);
	public function all_expired();
}

item.php

<?php 
interface iItem{
	public function all_items();
	public function get_item($item_id);
	public function add_item($iName, $iPrice, $type_id, $code, $brand, $grams);
	public function edit_item($item_id, $iName, $iPrice, $type_id, $code, $brand, $grams);
}

isales.php

<?php 
interface iSales{
	public function new_sales($code,$generic,$brand,$gram,$type,$qty,$price);
	public function daily_sales($date);
}

istock.php

<?php 
interface iStock {
	public function all_stockList();
	public function get_stockList($stock_id);
	public function del_stockList($stock_id);
	public function add_stock($item_id, $qty, $xDate, $manu, $purc);
	public function all_stockGroup();
	public function update_stockQty($stock_id, $stock_qty);
	public function get_stockQty($stock_id);
	public function add_fuck($item_id, $qty, $xDate, $manu, $purc);
}


itransaccion.php

<?php 
interface iTransaction{
}

iUser.php

<?php 

interface iUser{
	public function user_login($username, $password);
}


carpeta include

sesion.php

<?php 
if(session_status() == PHP_SESSION_NONE)
{
	session_start();
}

if(!isset($_SESSION['logged_id'])){
	die('Access is Denied!');
}

carpeta database

connection.php

<?php 
class Connection{

	protected $isConn;
	protected $datab;
	protected $transaction;

							
	public function __construct($username="root", $password ="", $host="localhost", $dbname="inventario_farmacia", $options = []){
		
		$this->isConn = TRUE;
		try{
			$this->datab = new PDO("mysql:host={$host};  dbname={$dbname}; charset=utf8", $username, $password, $options);
			$this->datab->setAttribute(PDO::ATTR_ERRMODE, PDO::ERRMODE_EXCEPTION);
			$this->transaction = $this->datab;
			$this->datab->setAttribute(PDO::ATTR_DEFAULT_FETCH_MODE, PDO::FETCH_ASSOC);
			

		}catch(PDOException $e){
			throw new Exception($e->getMessage());			
		}

	}
 

	
	public function Disconnect(){
		$this->datab = NULL;
		$this->isConn = FALSE;
	}


	


}
 ?>
 
 database.php
 
 <?php 

include_once('Connection.php'); 

class Database extends Connection{


	public function __construct(){

		parent::__construct();
		if(session_status() == PHP_SESSION_NONE)
		{
			session_start();
		}
	}

	
	public function getRow($query, $params = []){
		try {
			$stmt = $this->datab->prepare($query);
			$stmt->execute($params);
			return $stmt->fetch();	
		} catch (PDOException $e) {
			throw new Exception($e->getMessage());	
		}


	}

	
	public function getRows($query, $params = []){
		try {
			$stmt = $this->datab->prepare($query);
			$stmt->execute($params);
			return $stmt->fetchAll();	
		} catch (PDOException $e) {
			throw new Exception($e->getMessage());	
		}
	}

	
	public function insertRow($query, $params = []){
		try {
			$stmt = $this->datab->prepare($query);
			$stmt->execute($params);
			return TRUE;	
		} catch (PDOException $e) {
			throw new Exception($e->getMessage());	
		}

	}

	
	public function updateRow($query, $params = []){
		$this->insertRow($query, $params);
		return true;
	}


	public function deleteRow($query, $params = []){
		$this->insertRow($query, $params);
		return true;
	}

	
	public function lastID(){
		$lastID = $this->datab->lastInsertId(); 
		return $lastID;
	}



	public function transInsert($query, $params = [], $query2, $params2 = []){
		try {
			$this->transaction->beginTransaction();
				$stmt = $this->datab->prepare($query);
				$stmt->execute($params);

				$stmt2 = $this->datab->prepare($query2);
				$stmt2->execute($params2);

			$this->transaction->commit();
		} catch (PDOException $e) {
			$this->transaction->rollBack();
			throw new Exception($e->getMessage());	
		}
	}


	public function Begin(){
		$this->transaction->beginTransaction();
	}

	public function Commit(){
		$this->transaction->commit();
	}

	public function test()
	{
		echo 'database class test';
	}
}


 ?>
 
 
 carpeta class
 
 cart.php
 <?php
require_once('../database/Database.php');
require_once('../interface/iCart.php');
class Cart extends Database implements iCart {

	public function add_toCart($item_id, $qty, $stock_id, $user_id, $uniqid)
	{
		$sql = "INSERT INTO cart(item_id, cart_qty, cart_stock_id, user_id, cart_uniqid)
				VALUES(?,?,?,?,?)";
		return $this->insertRow($sql, [$item_id, $qty, $stock_id, $user_id, $uniqid]);
	}

	public function all_cartDatas($user_id)
	{
		$sql = "SELECT *
				FROM cart c
				INNER JOIN item i 
				ON c.item_id = i.item_id
				WHERE user_id = ? 
				ORDER BY cart_id ASC";
		return $this->getRows($sql, [$user_id]);
	}

	public function delCart($cart_id)
	{
		$sql = "DELETE FROM cart
				WHERE cart_id = ?";
		return $this->deleteRow($sql, [$cart_id]);
	}

	public function dellAllCart()
	{
		$sql = "DELETE FROM cart";
		return $this->deleteRow($sql);
	}
	public function allCart()
	{
		$sql = "SELECT *
				FROM cart c 
				INNER JOIN item i 
				ON c.item_id = i.item_id
				INNER JOIN stock s 
				ON s.item_id = i.item_id
				INNER JOIN item_type it 
				ON it.item_type_id = i.item_type_id
		";
		return $this->getRows($sql);
	}
}

$cart = new Cart();


expired.php

<?php
require_once('../database/Database.php');
require_once('../interface/iExpired.php');
class Expired extends Database implements iExpired {

	public function add_expired($name, $price, $qty, $expiredDate)
	{
		$sql = "INSERT INTO expired(exp_itemName, exp_itemPrice, exp_itemQty, exp_expiredDate)
				VALUES(?,?,?,?);";
		return $this->insertRow($sql, [$name, $price, $qty, $expiredDate]);
	}

	public function all_expired()
	{
		$sql = "SELECT *
				FROM expired";
		return $this->getRows($sql);
	}
}

$expired = new Expired();


item.php

<?php
require_once('../database/Database.php');
require_once('../interface/iItem.php');
class Item extends Database implements iItem {
	public function all_items()
	{
		$sql = "SELECT *
				FROM item i 
				INNER JOIN item_type it 
				ON i.item_type_id = it.item_type_id
				ORDER BY i.item_name ASC";
		return $this->getRows($sql);
	}
	
	public function get_item($item_id)
	{
		$sql = "SELECT *
				FROM item
				WHERE item_id = ?";
		return $this->getRow($sql, [$item_id]);
	}

	public function add_item($iName, $iPrice, $type_id, $code, $brand, $grams)
	{
		$sql = "INSERT INTO item(item_name, item_price, item_type_id, item_code, item_brand, item_grams)
				VALUES(?, ?, ?, ?, ?, ?)";
		return $this->insertRow($sql, [$iName, $iPrice, $type_id, $code, $brand, $grams]);
	}

	public function edit_item($item_id, $iName, $iPrice, $type_id, $code, $brand, $grams)
	{
		$sql = "UPDATE item 
				SET item_name = ?, item_price = ?, item_type_id = ?, item_code = ?, item_brand = ?, item_grams = ?
				WHERE item_id = ?";
		return $this->updateRow($sql, [$iName, $iPrice, $type_id, $code, $brand, $grams, $item_id]);
	}
}

$item = new Item();



 sales.php

<?php
require_once('../database/Database.php');
require_once('../interface/iSales.php');
class Sales extends Database implements iSales {
	public function new_sales($code,$generic,$brand,$gram,$type,$qty,$price)
	{
		$sql = "INSERT INTO sales(item_code,generic_name,brand,gram,type,qty,price)
				VALUES(?,?,?,?,?,?,?);";
		return $this->insertRow($sql, [$code,$generic,$brand,$gram,$type,$qty,$price]);
	}

	public function daily_sales($date)
	{
		$sql = "SELECT *
				FROM sales
				WHERE DATE(`date_sold`) = ?";
		return $this->getRows($sql, [$date]);
	}
}
$sales = new Sales();

stock.php

<?php
require_once('../database/Database.php');
require_once('../interface/iStock.php');
class Stock extends Database implements iStock {

	public function all_stockList()
	{
		
				
			$sql = "SELECT * FROM item, stock,  item_type where item_type.item_type_id=item.item_type_id and item.item_id=stock.item_id and stock.stock_qty!=?";	
		return $this->getRows($sql, [0]);
	}
	public function get_stockList($stock_id)
	{
		$sql = "SELECT *
				FROM stock s 
				INNER JOIN item i 
				ON s.item_id = i.item_id
				WHERE s.stock_id = ?";
		return $this->getRow($sql, [$stock_id]);
	}

	public function del_stockList($stock_id)
	{
		$sql = "DELETE FROM stock 
				WHERE stock_id = ?";
		return $this->deleteRow($sql, [$stock_id]);
	}

	public function add_stock($item_id, $qty, $xDate, $manu, $purc)
	{
		$sql = "INSERT INTO stock(item_id, stock_qty, stock_expiry, stock_manufactured, stock_purchased)
				VALUES(?,?,?,?,?)";
	
		return $this->insertRow($sql, [$item_id, $qty, $xDate, $manu, $purc]);
	}

	public function all_stockGroup()
	{
		$sql = "SELECT s.stock_id,i.item_id,i.item_name, i.item_price,SUM(stock_qty) as qty
				FROM stock s 
				INNER JOIN item i
				ON s.item_id = i.item_id
				GROUP BY s.item_id
				ORDER BY i.item_name ASC";
		return $this->getRows($sql);
	}

	public function update_stockQty($stock_id, $stock_qty)
	{
		$sql = "UPDATE stock
				SET stock_qty = ?
				WHERE stock_id = ?";
		return $this->updateRow($sql, [$stock_qty, $stock_id]);
	}

	public function get_stockQty($stock_id)
	{
		$sql = "SELECT *
				FROM stock 
				WHERE stock_id = ?";
		return $this->getRow($sql, [$stock_id]);
	}

	public function add_fuck($item_id, $qty, $xDate, $manu, $purc)
	{
		$sql = "INSERT INTO stock(item_id, stock_qty, stock_expiry, stock_manufactured, stock_purchased)
				VALUES(?,?,?,?,?)";
		return $this->insertRow($sql, [$item_id, $qty, $xDate, $manu, $purc]);
	}

}
$stock = new Stock();


transaction.php

<?php
require_once('../database/Database.php');
require_once('../interface/iStock.php');
class Stock extends Database implements iStock {

	public function all_stockList()
	{
		
				
			$sql = "SELECT * FROM item, stock,  item_type where item_type.item_type_id=item.item_type_id and item.item_id=stock.item_id and stock.stock_qty!=?";	
		return $this->getRows($sql, [0]);
	}
	public function get_stockList($stock_id)
	{
		$sql = "SELECT *
				FROM stock s 
				INNER JOIN item i 
				ON s.item_id = i.item_id
				WHERE s.stock_id = ?";
		return $this->getRow($sql, [$stock_id]);
	}

	public function del_stockList($stock_id)
	{
		$sql = "DELETE FROM stock 
				WHERE stock_id = ?";
		return $this->deleteRow($sql, [$stock_id]);
	}

	public function add_stock($item_id, $qty, $xDate, $manu, $purc)
	{
		$sql = "INSERT INTO stock(item_id, stock_qty, stock_expiry, stock_manufactured, stock_purchased)
				VALUES(?,?,?,?,?)";
	
		return $this->insertRow($sql, [$item_id, $qty, $xDate, $manu, $purc]);
	}

	public function all_stockGroup()
	{
		$sql = "SELECT s.stock_id,i.item_id,i.item_name, i.item_price,SUM(stock_qty) as qty
				FROM stock s 
				INNER JOIN item i
				ON s.item_id = i.item_id
				GROUP BY s.item_id
				ORDER BY i.item_name ASC";
		return $this->getRows($sql);
	}

	public function update_stockQty($stock_id, $stock_qty)
	{
		$sql = "UPDATE stock
				SET stock_qty = ?
				WHERE stock_id = ?";
		return $this->updateRow($sql, [$stock_qty, $stock_id]);
	}

	public function get_stockQty($stock_id)
	{
		$sql = "SELECT *
				FROM stock 
				WHERE stock_id = ?";
		return $this->getRow($sql, [$stock_id]);
	}

	public function add_fuck($item_id, $qty, $xDate, $manu, $purc)
	{
		$sql = "INSERT INTO stock(item_id, stock_qty, stock_expiry, stock_manufactured, stock_purchased)
				VALUES(?,?,?,?,?)";
		return $this->insertRow($sql, [$item_id, $qty, $xDate, $manu, $purc]);
	}

}
$stock = new Stock();


user.php
<?php
require_once('../database/Database.php');
require_once('../interface/iUser.php');
class User extends Database implements iUser {

	public function user_login($username, $password)
	{
		$sql = "SELECT *
				FROM user 
				WHERE user_account = ?
				AND user_pass = ?
		";
		return $this->getRow($sql, [$username, $password]);
	}
	

}

$user = new User();


carpeta data


add_cart.php

<?php 
require_once('../class/Cart.php');
require_once('../class/Stock.php');
if(isset($_POST['stock_id'])){
	$stock_id = $_POST['stock_id'];
	$item_id = $_POST['item_id'];
	$cqty = $_POST['cqty'];
	$user_id = $_SESSION['logged_id'];
	$nqty = $_POST['nqty'];
	$uniqid = $_SESSION['uniqid'];
	
	$saveToCart = $cart->add_toCart($item_id, $cqty, $stock_id, $user_id, $uniqid);

	
	$updateStockQty = $stock->update_stockQty($stock_id, $nqty);

}
$cart->Disconnect();


 
add_fuck.php

<?php 
require_once('../class/Stock.php');
if(isset($_POST['purc'])){
	$item_id = $_POST['item_id'];
	$qty = $_POST['qty'];
	$xDate = $_POST['xDate'];
	$manu = $_POST['manu'];
	$purc = $_POST['purc'];

	$saveStock = $stock->add_fuck($item_id, $qty, $xDate, $manu, $purc);
}

add_item.php
<?php 
require_once('../class/Item.php');
if(isset($_POST['iName']) && isset($_POST['iPrice'])){
	$iName = $_POST['iName'];
	$iPrice = $_POST['iPrice'];
	$iType = $_POST['iType'];
	$code = $_POST['code'];
	$brand = $_POST['brand'];
	$grams = $_POST['grams'];
	$iName = strtolower($iName);
	$iPrice = strtolower($iPrice);
	$iName = ucwords(strtolower($iName));
	$code = ucwords(strtolower($code));
	$brand = ucwords(strtolower($brand));
	$grams = ucwords(strtolower($grams));

	$saveItem = $item->add_item($iName, $iPrice, $iType, $code, $brand, $grams);
	if($saveItem){
		$return['valid'] = true;
		$return['msg'] = "Nuevo registro agregado con éxito!";
	}else{
		$return['valid'] = false;
	}
	echo json_encode($return);
}

$item->Disconnect();


add_stock.php
<?php 
require_once('../class/Stock.php');
if(isset($_POST['item_id'])){
	$item_id = $_POST['item_id'];
	$qty = $_POST['qty'];
	$xDate = $_POST['xDate'];
	$manu = $_POST['manu'];
	$purc = $_POST['purc'];
	
	$saveStock = $stock->add_fuck($item_id, $qty, $xDate, $manu, $purc);
	$return['valid'] = false;
	if($saveStock){
		$return['valid'] = true;
		$return['msg'] = "New Stock Added Successfully!";
	}
	echo json_encode($return);
	
}

$stock->Disconnect();


add_transaction.php

<?php 

if(isset($_POST['custName'])){
	$custName = $_POST['custName'];
	$tender = $_POST['tender'];
	$totalOrder = $_POST['totalOrder'];
	$change = $_POST['change'];
	
}



all.expired.php

<?php 
require_once('../class/Expired.php');
$expireds = $expired->all_expired();

 ?>
 <h2>Medicamentos vencidos</h2>
<div class="table-responsive">
        <table id="myTable-expired" class="table table-bordered table-hover table-striped">
            <thead>
                <tr>
                    <th><center>Nombre</center></th>
                    <th><center>Precio</center></th>
                    <th><center>Cant.</center></th>
                    <th><center>Fecha de vencimiento</center></th>
                </tr>
            </thead>
            <tbody>
            <?php foreach($expireds as $ex): ?>
                <tr align="center" class="text-danger">
                    <td><?= ucwords($ex['exp_itemName']); ?></td>
                    <td><?= "$ ".number_format($ex['exp_itemPrice'], 2); ?></td>
                    <td><?= $ex['exp_itemQty']; ?></td>
                    <td><?= $ex['exp_expiredDate']; ?></td>
                </tr>
            <?php endforeach; ?>
            </tbody>
        </table>
</div>


<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />


<script type="text/javascript">
    $(document).ready(function() {
        $('#myTable-expired').DataTable();
    });
</script>

<?php 
$expired->Disconnect();
 ?>
 
 all_item.php
 <?php 
    require_once('../class/Item.php');
    $items = $item->all_items();
   
 ?>
<br />
<div class="table-responsive">
        <table id="myTable-item" class="table table-bordered table-hover table-striped">
            <thead>
                <tr>
                    <th>Código</th>
                    <th>Nombre</th>
                    <th>Fabricante</th>
                    <th>Tipo</th>
                    <th><center>Gramos</center></th>
                    <th><center>Precio</center></th>
                    <th>
                        <center>Acciones</center>
                    </th>
                </tr>
            </thead>
            <tbody>
                <?php foreach($items as $it): ?>
                    <tr align="center">
                        <td align="left"><?= $it['item_code']; ?></td>
                        <td align="left"><?= ucwords($it['item_name']); ?></td>
                        <td align="left"><?= $it['item_brand']; ?></td>
                        <td align="left"><?= $it['item_type_desc']; ?></td>
                        <td><?= $it['item_grams']; ?></td>
                        <td><?= "$ ".number_format($it['item_price'], 2); ?></td>
                        <td>
                           <center>
                               <button onclick="editModal('<?= $it['item_id']; ?>');" type="button" class="btn btn-warning btn-xs">Editar
                                <span class="glyphicon glyphicon-edit" aria-hidden="true"></span>
                                </button>
                           </center>
                        </td>
                    </tr>
                <?php endforeach; ?>
            </tbody>
        </table>
</div>


<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />


<script type="text/javascript">
    $(document).ready(function() {
        $('#myTable-item').DataTable();
    });
</script>

<?php 
$item->Disconnect();
 ?>
 
 all_sales.php
 
 <?php 
require_once('../class/Sales.php');

$date = $_GET['date'];
$dailySales = $sales->daily_sales($date);


 ?>
<br />
<div class="table-responsive">
        <table id="myTable-sales" class="table table-bordered table-hover table-striped">
            <thead>
                <tr>
                    <th>Código</th>
                    <th>Nombre</th>
                    <th>Fabricante</th>
                    <th><center>Gramos</center></th>
                    <th><center>Tipo</center></th>
                    <th><center>Precio</center></th>
                    <th><center>Cant.</center></th>
                    <th><center>Sub Total</center></th>
                </tr>
            </thead>
            <tbody>
            <?php 
                $total = 0;
                foreach($dailySales as $ds):
                $subTotal = number_format($ds['price'] * $ds['qty'], 2);   
                $total += $subTotal; 
            ?>
                <tr>
                    <td><?= $ds['item_code']; ?></td>
                    <td><?= $ds['generic_name']; ?></td>
                    <td><?= $ds['brand']; ?></td>
                    <td><?= $ds['gram']; ?></td>
                    <td><?= $ds['type']; ?></td>
                    <td align="center"><?= number_format($ds['price'],2); ?></td>
                    <td align="center"><?= $ds['qty']; ?></td>
                    <td align="center"><?= $subTotal; ?></td>
                </tr>
            <?php endforeach; ?>
            </tbody>
            <tr>
                <td></td>
                <td></td>
                <td></td>
                <td></td>
                <td></td>
                <td></td>
                <td align="right"><strong>TOTAL:</strong></td>
                <td align="center">
                    <strong><?= number_format($total,2); ?></strong>
                </td>
            </tr>
        </table>
</div>


<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />


<script type="text/javascript">
    $(document).ready(function() {
        $('#myTable-sales').DataTable();
    });
</script>

<?php 
$sales->Disconnect();
 ?>
 
 all_stock.php
 
 <?php 
    require_once('../class/Stock.php');
    $stocks = $stock->all_stockGroup();

   
 ?>
<br />
<div class="table-responsive">
        <table id="myTable-stock" class="table table-bordered table-hover table-striped">
            <thead>
                <tr>
                    <th><center>Nombre</center></th>
                    <th><center>Precio</center></th>
                    <th><center>Cantidad</center></th>
                </tr>
            </thead>
            <tbody>
            <?php foreach($stocks as $s): ?>
                <tr align="center">
                    <td><?= ucwords($s['item_name']); ?></td>
                    <td><?= "$ ".number_format($s['item_price'], 2); ?></td>
                    <td><?= $s['qty']; ?></td>
                </tr>
            <?php endforeach; ?>
            </tbody>
        </table>
</div>


<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />

<!-- for the datatable of employee -->
<script type="text/javascript">
    $(document).ready(function() {
        $('#myTable-stock').DataTable();
    });
</script>

<?php 
$stock->Disconnect();
 ?>
 
 all_stocklist.php
 <?php 
require_once('../class/Stock.php');
$stockList = $stock->all_stockList();

// echo '<pre>';
//     print_r($stockList);
// echo '</pre>';
 ?>
<br />
<div class="table-responsive">
        <table id="myTable-stocklist" class="table table-bordered table-hover table-striped">
            <thead>
                <tr>
                    <th><center></center></th>
                    <th>Código</th>
                    <th>Nombre</th>
                    <th>Tipo</th>
                    <th><center>Fabricado</center></th>
                    <th><center>Comprado</center></th>
                    <th><center>Precio</center></th>
                    <th><center>Cantidad</center></th>
                    <th>Vence</th>
                </tr>
            </thead>
            <tbody>
                <?php 
                    $dateNow = date('Y-m');
                    foreach($stockList as $sl): 
                    $xDate = strtotime($sl['stock_expiry']);
                    $xDate = date('Y-m', $xDate);
                    $class = "text-success";
                    if($xDate == $dateNow){ 
                        $class = "text-warning";
                    }
                ?>
                    <tr  align="center" class="<?= $class; ?>">
                        <td><input type="checkbox" name="stock" value="<?= $sl['stock_id']; ?>"></td>
                        <td align="left"><?= $sl['item_code']; ?></td>
                        <td align="left"><?= ucwords($sl['item_name']); ?></td>
                        <td align="left"><?= $sl['item_type_desc']; ?></td>
                        <td><?= $sl['stock_manufactured']; ?></td>
                        <td><?= $sl['stock_purchased']; ?></td>
                        <td><?= "$ ".number_format($sl['item_price'],2); ?></td>
                        <td><?= $sl['stock_qty']; ?></td>
                        <td align="left" width="110px;"><?= $sl['stock_expiry']; ?>
                            <?php if($xDate <= $dateNow): ?>
                                <span class="label label-danger">!</span>
                            <?php endif; ?>
                        </td>
                    </tr>
                <?php endforeach; ?>
            </tbody>
        </table>
</div>


<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />


<script type="text/javascript">
    $(document).ready(function() {
        $('#myTable-stocklist').DataTable();
    });
</script>

<?php 
$stock->Disconnect();
 ?>
 
 confirm_order.php
 
 <?php 
require_once('../class/Cart.php');
require_once('../class/Sales.php');
if(isset($_POST['click'])){
	if($_POST['click'] == 'yes'){
		
		$cartDetails = $cart->allCart();

		foreach ($cartDetails as $cd) {
			$code = $cd['item_code'];
			$generic = $cd['item_name'];
			$brand = $cd['item_brand'];
			$gram = $cd['item_grams'];
			$type = $cd['item_type_desc'];
			$cartQty = $cd['cart_qty'];
			$price = $cd['item_price'];

			$insertSale = $sales->new_sales($code,$generic,$brand,$gram,$type,$cartQty,$price);
			
		}

		
		$delAllCart = $cart->dellAllCart();
		$return['valid'] = false;
		if($delAllCart){
			$return['valid'] = true;
			$return['msg'] = 'La transacción se agregó correctamente!';
		}
		echo json_encode($return);
	}
}


del_cart.php

<?php 
require_once('../class/Stock.php');
require_once('../class/Cart.php');
if(isset($_POST['stock_id'])){
	$stock_id = $_POST['stock_id'];
	$cart_id = $_POST['cart_id'];
	$qty = $_POST['qty'];

	
	$cqty = $stock->get_stockQty($stock_id);
	$currentQty = $cqty['stock_qty'];
	$qty += $currentQty;
	
	$stock->update_stockQty($stock_id, $qty);
	
	$deleteCart = $cart->delCart($cart_id);
}//end isset

$stock->Disconnect();

del_expired.php

<?php 

require_once('../class/Expired.php');
require_once('../class/Stock.php');
if(isset($_POST['stock_id'])){
	$stock_id = $_POST['stock_id'];

	
	$stockDetail = $stock->get_stockList($stock_id);
	$name = $stockDetail['item_name'];
	$price = $stockDetail['item_price'];
	$qty = $stockDetail['stock_qty'];
	$expiredDate = $stockDetail['stock_expiry'];

	$saveToExpired = $expired->add_expired($name, $price, $qty, $expiredDate);
	$delStock =	$stock->del_stockList($stock_id);
	$return['valid'] = false;
	if($delStock && $saveToExpired){
		$return['valid'] = true;
		$return['msg'] = "Eliminado correctamente!";
	}
	echo json_encode($return);
}

$expired->Disconnect();

edit_item.php

<?php 
require_once('../class/Item.php');
if(isset($_POST['item_id'])){
	$item_id = $_POST['item_id'];
	$iName = $_POST['iName'];
	$iPrice = $_POST['iPrice'];
	$iType = $_POST['iType'];
	$code = $_POST['code'];
	$brand = $_POST['brand'];
	$grams = $_POST['grams'];
	$saveEdit = $item->edit_item($item_id, $iName, $iPrice, $iType, $code, $brand, $grams);
	$return['valid'] = false;
	if($saveEdit){
		$return['valid'] = true;
		$return['msg'] = "Editado correctamente!";
	}
	echo json_encode($return);
}
$item->Disconnect();


get_item.php

<?php 
require_once('../class/Item.php');
if(isset($_POST['item_id'])){
	$item_id = $_POST['item_id'];
	$itemDetails = $item->get_item($item_id);
	$return['title'] = "Edit Item";
	$return['event'] = "edit";
	if($itemDetails > 0){
		$return['name'] = $itemDetails['item_name'];
		$return['price'] = $itemDetails['item_price'];
		$return['id'] = $itemDetails['item_id'];
		$return['code'] = $itemDetails['item_code'];
		$return['brand'] = $itemDetails['item_brand'];
		$return['grams'] = $itemDetails['item_grams'];
		$return['type'] = $itemDetails['item_type_id'];
	}
	echo json_encode($return);	
	
}

$item->Disconnect();


login.php

<?php 
require_once('../class/User.php');

if(isset($_POST['un'])){
	$un = $_POST['un'];
	$up = $_POST['up'];

	$up = md5($up);
	$result = $user->user_login($un, $up);
	if($result > 0){
		
		$return['logged'] = true;
		$return['url'] = "home.php";
		$_SESSION['logged_id'] = $result['user_id'];
		$_SESSION['logged_type'] = $result['user_type'];
		$_SESSION['uniqid'] = uniqid();
	}else{
		
		$return['logged'] = false;
		$return['msg'] = "Usuario o contraseña invalido!";
	}

	echo json_encode($return);

}

$user->Disconnect();

order.php

<?php 
    require_once('../class/Stock.php');
    require_once('../class/Cart.php');
    $stocks = $stock->all_stockList();
    $cartDatas = $cart->all_cartDatas($_SESSION['logged_id']);
    
 ?>

<div class="row">
    <div class="col-md-6">
        <div class="panel panel-success">
            <div class="panel-heading">
                <h3 class="panel-title">
                <span class="glyphicon glyphicon-list" aria-hidden="true"></span>
                Productos</h3>
            </div>
            <div class="panel-body">
               
               <div class="table-responsive">
                        <table id="myTable-item-order" class="table table-bordered table-hover table-striped">
                            <thead>
                                <tr>
                                    <th><center>Código</center></th>
                                    <th><center>Nombre</center></th>
                                    <th><center>Fabricante</center></th>
                                    <th><center>Precio</center></th>
                                    <th><center>Cant.</center></th>
                                    <th><center></center></th>
                                </tr>
                            </thead>
                            <tbody>
                            <?php foreach($stocks as $s): ?>
                                <tr align="center">
                                    <td><?= ucwords($s['item_code']); ?></td>
                                    <td><?= ucwords($s['item_name']); ?></td>
                                    <td><?= ucwords($s['item_brand']); ?></td>
                                    <td><?= "$ ".number_format($s['item_price'], 2); ?></td>
                                    <td><?= $s['stock_qty']; ?></td>
                                    <td>
                                        <button onclick="toCart('<?= $s['stock_id']; ?>','<?= $s['stock_qty']; ?>','<?= $s['item_id']; ?>');" type="button" class="btn btn-success btn-xs">
                                            <span class="glyphicon glyphicon-shopping-cart" aria-hidden="true"></span>
                                        </button>
                                    </td>
                                </tr>
                            <?php endforeach; ?>
                            </tbody>
                        </table>
                </div>

                <script type="text/javascript">
                    $(document).ready(function() {
                        $('#myTable-item-order').DataTable();
                    });
                </script>

               
            </div>
        </div>
    </div>
    <div class="col-md-6">
        <div class="panel panel-primary">
            <div class="panel-heading">
                <h3 class="panel-title">
                <span class="glyphicon glyphicon-shopping-cart" aria-hidden="true"></span>
                Carrito
                </h3>
            </div>
            <div class="panel-body">
              
                <div class="table-responsive">
                        <table id="myTable-cart" class="table table-bordered table-hover table-striped">
                            <thead>
                                <tr>
                                    <th><center>Nombre</center></th>
                                    <th><center>Precio</center></th>
                                    <th><center>Cant.</center></th>
                                    <th><center>Sub</center></th>
                                    <th><center></center></th>
                                </tr>
                            </thead>
                            <tbody>
                            <?php
                            $total = 0;
                             foreach($cartDatas as $c): 
                                $price = $c['item_price'];
                                $qty = $c['cart_qty'];
                                $subTotal = $price * $qty;
                                $total += $subTotal;
                            ?>
                                <tr align="center">
                                    <td><?= ucwords($c['item_name']); ?></td>
                                    <td><?= "$ ".number_format($c['item_price'], 2); ?></td>
                                    <td><?= $c['cart_qty']; ?></td>
                                    <td><?= number_format($subTotal,2); ?></td>
                                    <td>
                                    <button onclick="delCart('<?= $c['cart_stock_id']; ?>','<?= $qty; ?>','<?= $c['cart_id']; ?>');" type="button" class="btn btn-danger btn-xs">
                                        <span class="glyphicon glyphicon-trash" aria-hidden="true"></span>
                                    </button>
                                    </td>
                                </tr>
                            <?php endforeach; ?>
                            </tbody>
                                <tr>
                                    <td></td>
                                    <td></td>
                                    <td align="right"><strong>Total:</strong></td>
                                    <td align="center">
                                        <strong><?= number_format($total, 2); ?></strong>
                                    </td>
                                    <td>
                                        <?php if($total > 0): ?>
                                        <button onclick="confirm_cart()" type="button" class="btn btn-success btn-xs">
                                        Confirmar
                                        <span class="glyphicon glyphicon-shopping-cart" aria-hidden="true"></span>
                                        </button>
                                        <?php endif; ?>
                                    </td>
                                </tr>
                        </table>
                </div>

                <script type="text/javascript">
                    $(document).ready(function() {
                        $('#myTable-cart').DataTable();
                    });
                </script>

               
            </div>
        </div>
    </div>
</div>

<br /><br /><br /><br /><br /><br /><br /><br />


print-sales.php


<?php 
require_once('../class/Sales.php');

$date = $_GET['date'];
$dailySales = $sales->daily_sales($date);


 ?>
 <!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <title></title>
    <!-- Tell the browser to be responsive to screen width -->
    <meta content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no" name="viewport">
    <!-- Bootstrap 3.3.5 -->
    <link rel="stylesheet" href="../assets/css/bootstrap.min.css">
    <link rel="stylesheet" href="../assets/css/bootstrap-theme.min.css">
    <!-- Font Awesome -->
    <link href="../assets/css/dataTables.bootstrap.min.css" rel="stylesheet">
    <script type="text/javascript">
        print();
    </script>
  </head>
  <body>
    
 <center>
    <h1>Reporte diario de ventas</h1>
    <h2>de</h2>
    <h3><?= $date; ?></h3>
 </center>
<br />
<div class="table-responsive">
        <table id="myTable-sales" class="table table-bordered table-hover table-striped">
            <thead>
                <tr>
                    <th>Código</th>
                    <th>Nombre</th>
                    <th>Fabricante</th>
                    <th><center>Gramos</center></th>
                    <th><center>Tipo</center></th>
                    <th><center>Precio</center></th>
                    <th><center>Cant.</center></th>
                    <th><center>Sub Total</center></th>
                </tr>
            </thead>
            <tbody>
            <?php 
                $total = 0;
                foreach($dailySales as $ds):
                $subTotal = number_format($ds['price'] * $ds['qty'], 2);   
                $total += $subTotal; 
            ?>
                <tr>
                    <td><?= $ds['item_code']; ?></td>
                    <td><?= $ds['generic_name']; ?></td>
                    <td><?= $ds['brand']; ?></td>
                    <td><?= $ds['gram']; ?></td>
                    <td><?= $ds['type']; ?></td>
                    <td align="center"><?= number_format($ds['price'],2); ?></td>
                    <td align="center"><?= $ds['qty']; ?></td>
                    <td align="center"><?= $subTotal; ?></td>
                </tr>
            <?php endforeach; ?>
            </tbody>
            <tr>
                <td></td>
                <td></td>
                <td></td>
                <td></td>
                <td></td>
                <td></td>
                <td align="right"><strong>TOTAL:</strong></td>
                <td align="center">
                    <strong><?= number_format($total,2); ?></strong>
                </td>
            </tr>
        </table>
</div>


<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
<br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />

<!-- for the datatable of employee -->
<script type="text/javascript">
    $(document).ready(function() {
        $('#myTable-sales').DataTable();
    });
</script>

<?php 
$sales->Disconnect();
 ?>




	  
	  
	  
	  

regis.js

	  

function eMsg(params){
	alert("Error: L"+params+"+");
}

$(document).on('submit', '#form-login', function(event) {
	event.preventDefault();
	/* Act on the event */
	var un = $('#un').val();
	var up = $('#up').val();

	$.ajax({
			url: 'data/login_user.php',
			type: 'post',
			dataType: 'json',
			data: {
				un:un,
				up:up
			},
			success: function (data) {
				console.log(data);
				if(data.logged == true){
					window.location = data.url;
				}else{
					alert(data.msg);
					$('#un').focus();
				}
			},
			error: function(){
				alert('Error: L17+');
			}
		});
});


function showAllItem()
{
	$.ajax({
			url: 'data/all_item.php',
			success: function (data) {
				$('#all-item').html(data);
			},
			error: function(){
				alert('Error: L42+');
			}
		});
}//end showAllItem
showAllItem();

$('#add-new-item').click(function(event) {
	/* Act on the event */
	$('#modal-item').find('.modal-title').text('Agregar producto');
	$('#modal-item').modal('show');
	$('#submit-item').val('add');
});

$(document).on('submit', '#form-item', function(event) {
	event.preventDefault();
	/* Act on the event */
	var iName = $('#item-name').val();
	var iPrice = $('#item-price').val();
	var iType = $('#item-type').val();
	var code = $('#code').val();
	var brand = $('#brand').val();
	var grams = $('#grams').val();
    if($('#submit-item').val() == "add"){
    	// console.log('add ra');
	    $.ajax({
	    		url: 'data/add_item.php',
	    		type: 'post',
	    		dataType: 'json',
	    		data: {
	    			iName:iName,
	    			iPrice:iPrice,
	    			iType:iType,
	    			code:code,
	    			brand:brand,
	    			grams:grams
	    		},
	    		success: function (data) {
	    			console.log(data);
	    			if(data.valid == true){
	    				$('#modal-message').find('#msg-body').text(data.msg);
	    				$('#modal-item').modal('hide');
	    				showAllItem();
	    				$('#modal-message').modal('show');
	    				$('#submit-item').val('null');
	    			}
	    		},
	    		error: function(){
	    			eMsg('70');
	    		}//
	    	});
    }//end if == "add"
});


function editModal(item_id){
	// $('#submit-item').val('add');
	$.ajax({
			url: 'data/get_item.php',
			type: 'post',
			dataType: 'json',
			data: {
				item_id:item_id
			},
			success: function (data) {
				$('#submit-item').val(data.event);
				$('#item-name').val(data.name);
				$('#item-price').val(data.price);
				$('#item-id').val(data.id);
				$('#code').val(data.code);
				$('#brand').val(data.brand);
				$('#grams').val(data.grams);
				$('#item-type').val(data.type);
				$('#modal-item').find('.modal-title').text("Editar producto");
				$('#modal-item').modal('show');
			},
			error: function(){
				alert('Error: L56+');
			}
		});
}//end editModal

//save edit modal
$(document).on('submit', '#form-item', function(event) {
	event.preventDefault();
	/* Act on the event */
	var submit = $('#submit-item').val();
	var item_id = $('#item-id').val();

	var iName = $('#item-name').val();
	var iPrice = $('#item-price').val();
	var iType = $('#item-type').val();
	var code = $('#code').val();
	var brand = $('#brand').val();
	var grams = $('#grams').val();

	if(submit  == "edit"){
		$.ajax({
				url: 'data/edit_item.php',
				type: 'post',
				dataType: 'json',
				data: {
					item_id:item_id,
					iName:iName,
	    			iPrice:iPrice,
	    			iType:iType,
	    			code:code,
	    			brand:brand,
	    			grams:grams
				},
				success: function (data) {
					// console.log(data);
					if(data.valid == true){
						$('#modal-message').find('#msg-body').text(data.msg);
						$('#modal-item').modal('hide');
						showAllItem();
						$('#modal-message').modal('show');
					}
				},
				error: function(){
					eMsg('127');
				}
			});
	}//end submit
});

function showAllStockList(){
	$.ajax({
			url: 'data/all_stocklist.php',
			type: 'post',
			success: function (data) {
				$('#all-stocklist').html(data);
			},
			error: function(){
				eMsg('152');
			}
		});
}
showAllStockList();


$('#del-stock').click(function(event) {
	/* Act on the event */
	var check = 0;
	 $('input[type=checkbox]:checked').each(function(index) {
		check++;        
    });
	 if(check == 0){
	 	alert('Please Select Row!');
	 }else{
	 	$('#confirm-type').val('expired');
		$('#modal-confirmation').modal('show');
	}//end if check == 0
});

$('.del-expired').click(function(event) {
	
	if($('#confirm-type').val() == "expired"){
			var finish = false;
		$('input[type=checkbox]:checked').each(function(index) {
			// console.log($(this).val());
			finish = true;
			var stock_id = $(this).val();
			$.ajax({
					url: 'data/del_expired.php',
					type: 'post',
					dataType: 'json',
					data: {
						stock_id:stock_id
					},
					success: function (data) {
						showAllStockList();
					},
					error: function(){
						eMsg('195');
					}
				});
	    });
		if(finish == true){
			$('#modal-confirmation').modal('hide');
			$('#modal-message').find('#msg-body').text('Eliminado correctamente!')
			$('#modal-message').modal('show');
		}//end finish
		
	}//end if
});

$('#add-stock').click(function(event) {
	/* Act on the event */
	$('#modal-stock').find('.modal-title').text('Nuevo stock');
	$('#modal-stock').modal('show');
});

//form stock
var fuck = 0;
$(document).on('submit', '#form-stock', function(event) {
	event.preventDefault();
	/* Act on the event */
    var item_id = $('#item-id').val();
    var qty = $('#qty').val();
    var xDate = $('#xDate').val();
    var manu = $('#manu').val();
    var purc = $('#purc').val();
    fuck++;
    // alert(fuck);
    $.ajax({
    		url: 'data/add_fuck.php',
    		type: 'post',
    		// dataType: 'json',
    		data: {
    			item_id:item_id,
    			qty:qty,
    			xDate:xDate,
    			manu:manu,
    			purc:purc
    		},
    		success: function (data) {
    			console.log(data);
    			// console.log('stock');
    			// if(data.valid == true){
    				$('#modal-stock').modal('hide');
 		   			showAllStockList();
    				$('#modal-message').find('#msg-body').text(data.msg);
    				$('#modal-message').modal('show');
    			// }
    		},
    		error: function(){
    			eMsg('233');
    		}
    	});

});

//all expired
function showAllExpired(){
	$.ajax({
			url: 'data/all_expired.php',
			type: 'post',
			// data: {},
			success: function (data) {
				$('#all-expired').html(data);
			},
			error: function(){
				eMsg('260');
			}
		});
}//end showAllExpired
showAllExpired();

//all stock
function showAllStocks(){
	$.ajax({
			url: 'data/all_stock.php',
			type: 'post',
			success: function (data) {
				$('#all-stock').html(data);
			},
			error: function(){
				eMsg('275');
			}
		});
}//end showAllStocks
showAllStocks();

//stock report print
$('#stock-report').click(function(event) {
	
	
	window.open('data/print.php','name','width=auto,height=auto');
});

function showOrder(){
	$.ajax({
			url: 'data/order.php',
			type: 'post',
			success: function (data) {
				$('#order').html(data);
			},
			error: function(){
				eMsg('297');
			}
		});
}//end showOrder
showOrder();

//add to cart
function toCart(stock_id, qty, item_id){
	$('#stock-id').val(stock_id);
	$('#item-id').val(item_id);
	$('#item-qty').val(qty);
	$('#modal-to-cart').modal('show');
}//end toCart

$(document).on('submit', '#form-toCart', function(event) {
	event.preventDefault();
	/* Act on the event */
	var stock_id = $('#stock-id').val();
	var item_id = $('#item-id').val();
	var qty = $('#item-qty').val();
	var cartQty = $('#cart-qty').val();//add to cart
	var newStockQty = qty - cartQty;
	if(newStockQty < 0){
		alert('El artículo no es suficiente!');
	}else{
		// alert('Enough!');
		$.ajax({
				url: 'data/add_cart.php',
				type: 'post',
				data: {
					stock_id:stock_id,
					item_id:item_id,
					cqty:cartQty,
					nqty:newStockQty
				},
				success: function (data) {
					console.log(data);
					showOrder();
					$('#modal-to-cart').modal('hide');
				},
				error:function(){
					eMsg('331');
				}
			});
	}//end if !qty
});

//del from cart
function delCart(stock_id, qty, cart_id){
	$.ajax({
			url: 'data/del_cart.php',
			type: 'post',
			data: {
				stock_id:stock_id,
				cart_id:cart_id,
				qty:qty
			},
			success: function (data) {
				console.log(data);
				showOrder();
			},
			error: function(){
				eMsg('354');
			}
		});
}//end delCart

//order form
$(document).on('submit', '#form-order', function(event) {
	event.preventDefault();
	
	var custName = $('#customer-name').val();
	var tender = $('#tendered').val();
	var totalOrder = $('#totalOrder').val();
	var change = tender - totalOrder;

	if(change < 0){
		alert('Datos insuficientes!');
	}else{
		
		$.ajax({
				url: 'data/add_transaction.php',
				type: 'post',
				
				data: {
					custName:custName,
					tender:tender,
					totalOrder:totalOrder,
					change:change
				},
				success: function (data) {
					console.log(data);
				},
				error: function(){
					eMsg('385');
				}
			});
	}//end change < 0
	
});//form order


function confirm_cart(){
	$('#confirm-type').val('confirmCart');
	$('#modal-confirmation').modal('show');
}//end confirm_cart

$('#confirm-yes').click(function(event) {
	/* Act on the event */
	var choice = $('#confirm-type').val();
	if(choice == 'confirmCart'){
		$.ajax({
				url: 'data/confirm_order.php',
				type: 'post',
				dataType: 'json',
				data:{
					click:'yes'
				},
				success: function (data) {
					// console.log(data);
					if(data.valid == true){
						$('#confirm-type').val(' ');
						$('#modal-confirmation').modal('hide');
						showOrder();
						$('#modal-message').find('#msg-body').text(data.msg);
						$('#modal-message').modal('show');
					}
				},
				error: function(){
					eMsg(445);
				}
			});
	}
});


function showAllSales(){
	var date = $('#dailyDate').val();
	dailySales(date);
}//end showAllSales
showAllSales();

function dailySales(date){
	$.ajax({
			url: 'data/all_sales.php?date='+date,
			type: 'get',
			data: {
				date:date
			},
			success: function (data) {
				$('#all-sales').html(data);
			},
			error:function(){
				eMsg(474);
			}
		});	
}


$(document).on('change', '#dailyDate', function(event) {
	event.preventDefault();
	/* Act on the event */
	var date = $('#dailyDate').val();
	if(date == '' || date == null){
		$('#printBut').hide();
	}else{
		$('#printBut').show();
	}
	dailySales(date);

});

$('#printBut').click(function(event) {
	/* Act on the event */
	var date = $('#dailyDate').val();
	window.open('data/print-sales.php?date='+date,'name','width=600,height=400');	
});




 
 
 
 
 


















 
