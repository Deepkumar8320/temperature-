#include<iostream>
using namespace std;

 int orlando[7];
 int austin[7];
 int temperature[7][7];
 
int main()
{
    
    
    cout<<"======Input 7 day's Temperature of Orlando========"<<endl;
    // asking user to enter the Temperature for Orlando
     cout<<"Cityname Day:"<<"#"<<" "<< "Temperature:"<<" "<<endl;
    for (int i=0; i<7; i++)
    {
        cout<<"Orlando Day:"<<i+1<<" "<< "Temperature:"<<" ";
        cin>>orlando[i];
        cout<<endl;
    }
    
    cout<<"======Input 7 day's Temperature of Austin========"<<endl;
    // asking user to enter the Temperature
    cout<<"Cityname Day:"<<"#"<<" "<< "Temperature:"<<" "<<endl;
    for (int i=0; i<7; i++)
    {
        cout<<"Austin Day:"<<i+1<<" "<<"Temperature:"<<" ";
        cin>>austin[i];
        cout<<endl;
    }
    // 
    for (int i=0;i<2;i++)
   {
        for (int j=0;j<7;j++)
        {
             if (i==0)
            {
                temperature[i][j] = orlando[j];
            }
             else if (i==1)
            {
                 temperature[i][j] = austin[j];
            }
        }
    }
    
      //print the temperature array
        cout<<"=======Expanded program output======="<<endl;
      for (int i=0;i<2;i++)
      {
            for(int j=0;j<7;j++)
             {
               if (i==0)
               {
                cout<<"Oralando City Day "<< j+1<< " = "<< temperature[i][j]<<endl; 
               }
               else if (i==1)
               {
                cout<<"Austin City Day "<< j+1<< " = "<< temperature[i][j]<<endl; 
               }
              }     
       }
    
    
    
    return 0;
    
}
