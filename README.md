# Moda
public static void main(String[] args) {
    
        int numeroMax_que_se_rep = 0;
        int moda = 0;
        int numeros[] = {1, 2, 3, 5, 6, 4, 5, 2, 5, 3, 2, 5, 2, 6, 2, 4, 2, 2};
        for (int i = 0; i < numeros.length; i++) {
            int vecesRepetida = 0;
            for (int j = 0; j < numeros.length; j++) {

                if (numeros[i] == numeros[j]) {
                    vecesRepetida++;
                }
                if (vecesRepetida > numeroMax_que_se_rep) {
                    moda = numeros[i];
                    numeroMax_que_se_rep = vecesRepetida;

                }

            }

        }System.out.println("La moda es "+moda+" y se repitio "+numeroMax_que_se_rep+"  veces");

    }

}
