# wsdl_sunat
wsdl para envío a sunat

Para evitar el error SoapFault Exception :[WSDL] 
SOAP-ERROR Parsing WSDL: BillServicesPortBinding already defined in...

debe guardar los archivos en una carpeta
y en el código donde apunta al WS de SUNAT
direccionarlo al archivo donde lo tiene alojado
ejemplo:

//Reemplazar esto
$wsdl='https://e-factura.sunat.gob.pe/ol-ti-itcpfegem/billService?wsdl';

//Por esto
$wsdl='c:xampp/htdocs/miproyecto/wsdl/billService.wsdl';
...resto del código
