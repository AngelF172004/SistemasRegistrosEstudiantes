# SistemasRegistrosEstudiantes
private static void registrarEstudiante() {
    System.out.print("Nombre: ");
    String nombre = scanner.nextLine();
    System.out.print("Edad: ");
    int edad = scanner.nextInt();
    scanner.nextLine(); // Consumir la nueva línea pendiente
    System.out.print("Matrícula: ");
    String matricula = scanner.nextLine();
    System.out.print("Carrera: ");
    String carrera = scanner.nextLine();

    estudiantes[numEstudiantes] = new Estudiante(nombre, edad, matricula, carrera);
    numEstudiantes++;
    System.out.println("Estudiante registrado con éxito.");
}
