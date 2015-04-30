#include <iostream>
#include <fstream>
#include <sstream>
#include <cstdlib>
#include <string>
#include <vector>
#include <cmath>
using namespace std;

void ReadNumbersFromFiles (string filename){

  int number_of_lines = 0;
  int sum = 0;
  int x;
  float deb;
  int mean;
  float sdev;
  float var;
  vector <int> numbers;
  ifstream myFile;
  myFile.open(filename.c_str());
  string line;
  int numLines = 0;

while ( getline(myFile, line) )
{
  ++numLines;
  x = atoi(line.c_str());
  sum = sum + x;
  numbers.push_back(x);
}

      mean= sum/ numLines;
      for(int i = 1; i <= numLines; i++){
              deb = (x - mean)*(x - mean);
              sdev = sdev + deb;
          }
      var = sdev / (numLines - 1);
      deb= sqrt(var);
      cout << "Number of lines in text file: " << numLines<<endl;
      myFile.close();
      cout<<"the sum of the numbers: "<< sum<<endl;
      cout<<"mean: "<<mean<<endl;
      cout<<"The standard deviation: "<<endl;
    }

int main()
{
  ReadNumbersFromFiles("random_numbers.txt");
}
