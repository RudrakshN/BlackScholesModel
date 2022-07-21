#include <iostream>
#include <math.h>
#include <cmath>
#include <cstdlib>

using namespace std;

int main()
{
    //Getting the variables ready 

    long double sp ;                                           //stock price 
    long double stp ;                                          //strike price
    long double time ;                                         //time of expiry
    long double v ;                                            //Volitality or standard deviation log returns 
    long double r ;                                            //risk free interest rate 

    cout<<"Welcome to Black Scholes Option Pricing Model Calculator";

    cout<<"Please enter the value of stock price";
    cin>>sp;

    cout<<"Please enter the value of strike price";
    cin>>stp;

    cout<<"Please enter the value of time";
    cin>>time;

    cout<<"Please enter the value of volitality";
    cin>>v;

    cout<<"Please enter the value of risk free interest rate";
    cin>>r;


    //Caluclation of delta1 and delta2
     
     long double delta1,delta2 ;

     delta1 = (log(sp/stp)+(r+(((sp*sp)/2)*time)))/(sqrt(time)*v) ;

     delta2 = (log(sp/stp)+(r-(((sp*sp)/2)*time)))/(sqrt(time)*v) ;
     
     //Calculation of option price 

     cout<<"The intrinsic value of the option is" ;

     cout<<(sp*(1/sqrt(2*3.14159265))*pow(2.71828182,-(delta1*delta1)/2))-(pow(2.71828182,-r*time)*stp*(1/sqrt(2*3.14159265))*pow(2.71828182,-(delta2*delta2)/2)) ;
}
