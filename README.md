include <iostream>

using namespace std;

class Marks
{
    float Score;
    string Grade;
    public:
        Marks(){}
        Marks(float s , string g);
        Marks(float s, string g);
        void display(void);
};
Marks::Marks(float s, string g)
{
    Score=s;
    Grade=g;
}
void Marks::display(void)
{
    cout<<"\n"<<"Score = "<<Score<<"\n"
    <<"Grade = "<<Grade<<"\n";
}
int main()
{
    Marks s1,s2,s3;              
    string g;
    float s;
    cout<<"Enter Score (in percent)"<<"\n";
    cin>>s>>g;
    s1=Marks(s,g);
    
    cout<<"Enter Score (in decimal)"<<"\n";
    cin>>s>>g;
    s2=Marks(s,g);
    
    cout<<"Enet Score and period "<<"\n";
    cin>>s>>g;
    s3=Marks(s,g);
    
    cout<<"\nDeposit 1";
    s1.display();
    
     cout<<"\nDeposit 1";
    s2.display();
    
     cout<<"\nDeposit 1";
    s3.display();
    
    return 0;
}
