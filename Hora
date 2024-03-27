#include <stdio.h>
#include <time.h>

int main() {
    // Variáveis para armazenar informações de tempo
    time_t currentTime;
    struct tm *localTime;

    // Loop infinito para atualizar o relógio
    while (1) {
        // Obter o tempo atual
        currentTime = time(NULL);
        localTime = localtime(&currentTime);

        // Extrair informações de hora, minutos e segundos
        int hours = localTime->tm_hour;
        int minutes = localTime->tm_min;
        int seconds = localTime->tm_sec;

        // Imprimir o tempo atual no formato de relógio
        printf("\r%02d:%02d:%02d", hours, minutes, seconds);

        // Esperar 1 segundo antes de atualizar novamente
        fflush(stdout); // Limpar o buffer de saída
        sleep(1);
    }

    return 0;
}
