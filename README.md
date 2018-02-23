# WriteToFile
//#include "stdafx.h"
#include <iostream>
#include <fstream>
#include <sstream>
#include <string>
using namespace std;

int main()
{

    for (int i=0;i<5;i++)
    {
        ostringstream Convert;
        Convert<<"random_circuit_"<<i<<".v";
        string filename = "/Users/Lutarez/Desktop/test/" + Convert.str();
        ofstream output(filename.c_str());
        output.close();
    }



}
