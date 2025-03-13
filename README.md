# SistemasRegistrosEstudiantes
private static void buscarEstudiante() {
    System.out.print("Ingrese la matrícula a buscar: ");
    String matriculaBuscar = scanner.nextLine();
    boolean encontrado = false;

    for (int i = 0; i < numEstudiantes; i++) {
        if (estudiantes[i].getMatricula().equals(matriculaBuscar)) {
            estudiantes[i].mostrarDatos();
            encontrado = true;
            break;
        }
    }

    if (!encontrado) {
        System.out.println("Estudiante no encontrado.");
    }
}
