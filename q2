#include <iostream>
#include <iostream>
#include <fstream>
#include <sstream>
#include <cstdlib>
#include <string>
 using namespace std;

 int bananas(string banana){
   string str2="banana";
   ifstream myFile;
   myFile.open(banana.c_str());
   string line;
   size_t found;
    while ( getline(myFile, line) ){
     found = line.find(str2);
        if (found!=string::npos)
            cout << "first 'banana' found at: " <<found<<endl;
            found=line.find("banana",found+1);
          if (found!=string::npos)
            cout << "second 'banana' found at: " << found <<endl;

            found=line.find("banana",found+2);
          if (found!=string::npos)
            cout << "third 'banana' found at: " << found <<endl;

            found=line.find("banana",found+4);
          if (found!=string::npos)
            cout << "forth 'banana' found at: " << found <<endl;

            found=line.find("banana",found+5);
          if (found!=string::npos)
            cout << "fifth 'banana' found at: " << found <<endl;
    }

    myFile.close();

  return 0;
}
int main(){
  bananas("bananas.txt");
}
