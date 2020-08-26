// Write a program to demonstrate the use of static member function with example.
//Example Below is the Cost of jdm vehicle (Japanese Domestic Market).
"#include <iostream>
using namespace std;
class jdm
{
    int veh,wotax,tax=1100;
    static int cost;
    public:             

        void taxprice()
        {
             cout<<"Enter The cost of Vehicle(IN $) :";
             cin>>cost;
            veh = cost + tax;
        }
        void withtax()
        {
            cout<<"With Tax The Cost of Vehicle is :"<<veh<<endl;
            cout<<"Total Vehicle Cost is :"<<veh<<endl;
        }
        void withouttax()
        {
            cout<<"Without Tax, The Cost of Vehicle is : "<<cost;
            
        }
};
int jdm::cost;              

int main()
{

    jdm j1;         
    j1.taxprice();                      //obj 1  
    j1.withtax();                       //obj 2
    j1.withouttax();                    //obj 3
    return 0;
}"
