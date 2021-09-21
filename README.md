# EJERCICIO-1-MPOO

/*
INTEGRANTES DE EQUIPO:
Basurto Sánchez Jocelyn Judit
García Jiménez Carlos Iván
Miramontes Carsolio Carla Ivette
*/

class Vehiculo{

  int precio = 0;        //público
  String _Marca = "";    //privado
  String _Duenio = "";   //privado
  bool pago_diferido;    //público

  String get Marca{
    return _Marca;
  }
  set Marca( String marca ){
    _Marca = marca;
  }
  String get Duenio{
    return _Duenio;
  }
  set Duenio( String duenio ){
    _Duenio = duenio;
  }

  @override
  String toString(){
    print("\nINFORMACIÓN DEL VEHÍCULO:\n");
    return "MARCA: $_Marca\nPRECIO: $precio pesos mexicanos\nDUEÑO: $_Duenio\nPAGO DIFERIDO: $pago_diferido";
  }

  void frena( String stop ){
  print("\nEl carro: $stop");
  }

  void arranca( String go ){
  print("El carro: $go");
  }
}

void main() {

  final vehiculo = Vehiculo();

  vehiculo.precio = 450000;
  vehiculo.Marca = "Mazda";
  vehiculo.Duenio = "Jorge Ríos";
  vehiculo.pago_diferido = true;
   
  print(vehiculo);

  vehiculo.frena("STOOOOOP");
  vehiculo.arranca("RUN RUN RUN");
	
}
