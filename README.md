# -WSQ14-Estimating-e
#include iostream>
#include cmath>
using namespace std;

float fun(float b){

  float x;
  
  float R=0.0, Rf=0.0;
  
  float factorial =1;
  
  
  for (x=1; x<=b; x++)
  
  {
    factorial= factorial*x;
    
    
    R=R+1/factorial;
  }
  Rf=R+1;
  
  return Rf;
}
int main(){

  float a;
  
  cout<<"Calculating e...  "<<endl;
  
  cout<<"Give me the value "<<endl;
  
  cin>>a;
  
  float factorial= fun (a);
  
  cout<<"The constant is "<<factorial<<endl;
  
  return 0;
}
