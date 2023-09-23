using namespace std;

int main() {
	
	int T;
	cin >>T;
	while(T--)
	{
	    int N;
	    string d;
	    cin>>N;
	   cin>>d;
	    for(int i=0; i<N;i++)
	    {
	        if(d[i]=='5' or d[i]=='0')
	            {
	                cout<<"yes"<<endl;
	                break;}
	                 }
	           } cout<<"no"<<endl;
	return 0;
}