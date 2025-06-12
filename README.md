#include<iostream>
using namespace std;

int main(){



double temp, celsius,fahrenheit,kelvin;
char choice;

cout<<"Enter the temprature\n";
cin>>temp;

cout<<"Enter the choice of conversion (C for Celsius, F for Fahrenheit, K for Kelvin)\n: ";
cin>>choice;

if(choice =='C' || choice =='c'){
    celsius = temp;
    fahrenheit = (celsius * 9/5) + 32;
    kelvin = celsius + 273.15;
    cout<<"Celsius: "<<celsius<<endl;
    cout<<"Fahrenheit: "<<fahrenheit<<endl;
    cout<<"Kelvin: "<<kelvin<<endl;
}
else if(choice =='F' || choice =='f'){
    fahrenheit = temp;
    celsius = (fahrenheit - 32) * 5/9;
    kelvin = celsius + 273.15;
    cout<<"Celsius: "<<celsius<<endl;
    cout<<"Fahrenheit: "<<fahrenheit<<endl;
    cout<<"Kelvin: "<<kelvin<<endl;
}
else if(choice =='K' || choice =='k'){
    kelvin = temp;
    celsius = kelvin - 273.15;
    fahrenheit = (celsius * 9/5) + 32;
    cout<<"Celsius: "<<celsius<<endl;
    cout<<"Fahrenheit: "<<fahrenheit<<endl;
    cout<<"Kelvin: "<<kelvin<<endl;
}
else{
    cout<<"Invalid choice!"<<endl;
}

return 0;
}
