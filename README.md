# dartLab2

class Alumno{
  String? nombre;
  String? apellido;
  double? nota1;
  double? nota2;
  double? nota3;
  
  Alumno(this.nombre, this.apellido);
  Alumno.notas(this.nota1, this.nota2, this.nota3);
  
  @override
  String toString(){
    return 'Nombre completo:  $nombre, apellido: $apellido ';
  }
}

void main() {
  final arturo= Alumno('Arturo','Bullon');
  arturo.nota1=20;
  arturo.nota2=17;
  arturo.nota3=13;
  final alexnotas= Alumno.notas(12,20,10);
  alexnotas.nombre='Alex';
  alexnotas.apellido='Huancahuari';
  
  
  print(arturo.nombre);
  print(arturo.apellido);
  print(arturo.nota1); 
  print(arturo.nota2); 
  print(arturo.nota3);
  
  print(arturo.toString());
  
  print(alexnotas.nombre);
  print(alexnotas.apellido);
  print(alexnotas.nota1);
  print(alexnotas.nota2);
  print(alexnotas.nota3);
  
}
