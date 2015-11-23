public class deberes {
	
static Scanner dato=new Scanner(System.in);

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		promedio();
		alumno();
		tienda();

	}

	public static void promedio(){
		int x=1, acum=0,acum1=0;
		System.out.println("☺☺☺☺☺Bienbenidos al sistema☺☺☺☺☺");
		System.out.println("Ingrese el numero de alumnos por favor");
		int v=dato.nextInt();
		while (x<=v){
			System.out.println("ingrse la nota:"+x);
			double n1=dato.nextDouble();
			x=x+1;
			acum=(int)(acum+n1);
			acum1=acum+v/2;
			
		}
		System.out.println("Las notas ingresadas:"+v);
		System.out.println("Suma de las notas:"+acum);
		System.out.println("Promedio general:"+acum1);
		
		
	}
	public static void alumno(){
		int acum=0;
		for(int i=1;i<=50;i++){
			System.out.println("Ingrese el numero de alumnos:"+i);
			int v=dato.nextInt ();
			acum=acum+v;

			
			
			int f=(acum/2);
			System.out.println("Su promedio es :"+f);
		}
		if ((acum<0)&(acum>=70)){
			System.out.println("Usted aprobo ☺☺ ");
		}else if(acum>71){
			System.out.println("Usted reprobo ☻☻");
			
			
		}
	}
	public static void  tienda(){
		double iva;
		double acum=0,acum1=0,acum2=0;
		System.out.println("◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘");
		System.out.println("◘◘◘◘◘◘◘◘◘◘Desea ingresar al sistema◘◘◘◘◘◘◘◘◘◘");
		System.out.println("◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘");
		String re=dato.next();
		while(re.equals("si")){
		System.out.println ("Ingrese el monto de su conmpra, por favor");
		double mo=dato.nextDouble();
		System.out.println ("Escoja la bolita a elección");
		System.out.println ("1. roja");
		System.out.println ("2. amarilla");
		System.out.println ("3. blanca ");
		System.out.println("Seleccione una opcion");
		int bo=dato.nextInt(); 
		switch (bo){
		case 1:
		    iva = ((mo)+mo*0.12);
			System.out.println(" Total a pagar incluido el iva y descuento es :"+((iva)-iva*0.40));
			 acum=acum+((iva)-iva*0.40);
			break;
		case 2:
			 iva = ((mo)+mo*0.12);
			System.out.println("Su total a pagar incluido el iva y descuento es :"+((iva)-iva*0.25));
			acum1=acum1+((iva)-iva*0.25);
			break;
		case 3:
			iva = ((mo)+mo*0.12);
			System.out.println("Su total a pagar incluido el iva es :"+iva);
			acum2=acum2+iva;
			break;
			
			default:
				System.out.println("Opción no valida");
				}System.out.println("Desea seguir ingresando datos al sistema");
		re=dato.next();
}System.out.println("El total de ventas del dia es "+(acum+acum1+acum2));
    System.out.println("◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘");
	System.out.println("◘◘◘◘◘◘◘Gracias por utilizar el sistema◘◘◘◘◘◘◘");
	System.out.println("◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘◘");
	System.exit(0);
	}
