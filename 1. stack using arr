# include <iostream>
# define cap 10
using namespace std;
class stack{
	public:
		int array[cap];
		int topindex;
	stack(){
		topindex=-1;
		}
	int count(){
		return topindex+1;
	}
	bool isempty(){
		if (count()==0) return true;
		else return false;
	}
	bool isfull(){
		if (count()==cap) return true;
		else return false;
	}
	bool push(int value){
		if (isfull()) return false;
		else {
			topindex = topindex+1;
			array[topindex]=value;
			return true;
		}
	}
	int pop(){
		int deleted_value=array[topindex];
		topindex--;
		return deleted_value;
	}
	int top(){
		return array[topindex];
	}
	void print(){
		if (isempty()) cout<<"STACK IS EMPTY"<<endl;
		else {
			cout<<"STACK : "<<endl;
			for (int i=0;i<count();i++){
				cout<<array[i]<<" ";
			}
			cout<<endl;
		}
	}
};
int main(){
	stack s;
	int choice;
	while (true){
		cout<<"1. PUSH"<<endl<<"2. ISEMPTY"<<endl<<"3. ISFULL"<<endl<<"4. POP"<<endl<<"5. PRINT"<<endl<<"6. PEEK"<<endl<<"7. EXIT"<<endl<<"ENTER YOUR CHOICE : ";
		cin>>choice;
		switch(choice){
			case 1:
				int v;
				cout<<"ENTER VALUE :";
				cin>>v;
				s.push(v);
				break;
			case 2:
				if (s.isempty()) cout<<"STACK IS EMPTY"<<endl;
				else cout<<"STACK IS NOT EMPTY"<<endl;
				break;
			case 3:
				if (s.isfull()) cout<<"STACK IS FULL"<<endl;
				else cout<<"STACK IS NOT FULL"<<endl;
				break;
			case 4:
				cout<<s.pop();
				break;
			case 5:
				s.print();
				break;
			case 6:
				cout<<s.top();
				break;
			case 7:
				return 0;
		}
	}	
}
