# lumi-re-
lumière qui clignote 
#include <iostream>
#include <chrono> // pour la fonction sleep

int main() {
    // Boucle infinie pour faire clignoter la lumière
    while (true) {
        // Allume la lumière pendant 500 millisecondes
        std::cout << "Lumière allumée" << std::endl;
        std::this_thread::sleep_for(std::chrono::milliseconds(500)); // Pause de 500 millisecondes

        // Éteint la lumière pendant 500 millisecondes
        std::cout << "Lumière éteinte" << std::endl;
        std::this_thread::sleep_for(std::chrono::milliseconds(500)); // Pause de 500 millisecondes
    }

    return 0;
}
