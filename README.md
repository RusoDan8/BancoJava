# BancoJava
Un pequeño sistema de banco en java
import java.util.Scanner;

// Press Shift twice to open the Search Everywhere dialog and type `show whitespaces`,
// then press Enter. You can now see whitespace characters in your code.
public class Main
{
    public static void main(String[] args) {

        menu();


    }

    public static void menu()
    {

        int opcion;
        System.out.println("Bienvenido a Banco Bienestar \n");
        System.out.println("Elija el numero de la opcion. \n 1- Crear Usuario \n 2- Cambiar NIP \n 3- Depositar o Retirar dinero");
        Scanner cin = new Scanner(System.in);
        opcion = cin.nextInt();

        switch (opcion)
        {
            case 1:
            {
                crearCliente();
            }

        }



    }

    public static void crearCliente()
    {
        Scanner cin_Cliente = new Scanner(System.in);
        Cliente Agregar_nuevo = new Cliente();
        System.out.println("Ingrese nombre de el cliente");
        Agregar_nuevo.Nombre = cin_Cliente.nextLine();
        System.out.println("Ingrese Apellido");
        Agregar_nuevo.Apellido = cin_Cliente.nextLine();
        System.out.println("inserte NIP");
        Agregar_nuevo.password = cin_Cliente.nextLine();

        System.out.println("Sus datos son:" +  Agregar_nuevo.Nombre + "" + Agregar_nuevo.Apellido + "" + Agregar_nuevo.password);

    }
}
class Cliente
{
    int id;
 String Nombre;
 String Apellido;

 float dinero;

 String password;


}
