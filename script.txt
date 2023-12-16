#include <iostream>
#include <thread>
#include <chrono>

int main()
{
    srand(time(0));
    for (int i = 0; i < 45; i++)
    {
        for (int j = 0; j < 888; j++)
        {
            std::cout << static_cast<char>(33 + rand() % (127 - 33 + 1)) << " * ";
        }
        std::cout << std::endl;
    }

    for (int i = 0; i < 110; i++)
    {
        std::this_thread::sleep_for(std::chrono::milliseconds(10));
        std::cout << "#";
        std::this_thread::sleep_for(std::chrono::milliseconds(15));
    }
    std::this_thread::sleep_for(std::chrono::milliseconds(15));
    std::cout << std::endl;

    std::this_thread::sleep_for(std::chrono::milliseconds(50));
    std::cout << "            Успешно 100%" << std::endl;
    std::this_thread::sleep_for(std::chrono::milliseconds(390));
    std::cout << "            Все ваши данные были выгружены!!!" << std::endl;
    std::this_thread::sleep_for(std::chrono::milliseconds(1200));
    std::cout << " " << std::endl;
    std::cout << " " << std::endl;
    std::cout << " " << std::endl;
    std::cout << " " << std::endl;
    std::cout << "  Ваш компьютер заражен неизвестным вирусом" << std::endl;
    std::this_thread::sleep_for(std::chrono::milliseconds(900));
    std::cout << " " << std::endl;
    std::this_thread::sleep_for(std::chrono::milliseconds(700));
    std::cout << "  обратитесь к администратору" << std::endl;
    std::cout << " " << std::endl;
    std::this_thread::sleep_for(std::chrono::milliseconds(600));
    std::cout << "          !!!!!" << std::endl;
    std::cout << " " << std::endl;
    std::this_thread::sleep_for(std::chrono::milliseconds(400));
    std::cout << "     !!!" << std::endl;
    std::cout << " " << std::endl;
    std::this_thread::sleep_for(std::chrono::milliseconds(200));
    std::cout << "!!!" << std::endl;
    return 0;
}