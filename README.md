#include <iostream>
#include <ctime>
#include <time.h>
int main(){

    int year;
    time_t t = time(nullptr);
    tm *const pTInfo = localtime(&t);
    year=1900 + pTInfo->tm_year;
    std::cout<<year;

}
