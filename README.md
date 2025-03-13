# SistemasRegistrosEstudiantes
private static void eliminarEstudiante() {
    System.out.print("Ingrese la matrícula del estudiante a eliminar: ");
    String matriculaEliminar = scanner.nextLine();
    boolean eliminado = false;

    for (int i = 0; i < numEstudiantes; i++) {
        if (estudiantes[i].getMatricula().equals(matriculaEliminar)) {
            for (int j = i; j < numEstudiantes - 1; j++) {
                estudiantes[j] = estudiantes[j + 1];
            }
            numEstudiantes--;
            eliminado = true;
            System.out.println("Estudiante eliminado con éxito.");
            break;
        }
    }

    if (!eliminado) {
        System.out.println("Estudiante no encontrado.");
    }
}
