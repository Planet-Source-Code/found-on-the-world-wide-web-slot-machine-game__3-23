<div align="center">

## Slot machine Game


</div>

### Description

A slot machine game created by Kevin Presa. Found at: http://www.cprogramming.com/source.html
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Found on the World Wide Web](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/found-on-the-world-wide-web.md)
**Level**          |Intermediate
**User Rating**    |3.3 (10 globes from 3 users)
**Compatibility**  |C, C\+\+ \(general\)
**Category**       |[Games](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/games__3-13.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/found-on-the-world-wide-web-slot-machine-game__3-23/archive/master.zip)





### Source Code

```
//Kevin Pre$a
#include <iostream.h>
#include <conio.h>
#include <stdlib.h>
int main(void)
	{
	clrscr();
	int t=100;
	int pull=1;
	do{
		cout<<"You have "<<t<<" tokens. Pull?? (1 to pull, 2 to not pull) ";
		cin>>pull;
		if (pull==1)
			t=t-1;
		while (pull==1){
			random;
			int a=random(3)+1;
			random;
			int b=random(3)+1;
			random;
			int c=random(3)+1;
			random;
			int win=random(100)+1;
			cout<<"["<<a<<"]"<<" ["<<b<<"]"<<"]"<<" ["<<c<<"]"<<endl;
			if ((a==b) && (b==c) && (a==c))
				cout<<"You won: "<<win<<" tokens";
			else
     {
				cout<<"You lost: "<<(int)(win/10)<<" tokens";
      t=t-(int)(win/10);  //Note that the division is to prevent it
      							 //from working like a real slot machine
                 //That is, the user loses all of his or her
                 //money in a short amount of time.
     }
			if ((a==c) && (b==a) && (b==c))
				t=t+win;
			cout<<endl<<"You have "<<t<<" tokens. Pull?? (1 to pull, 2 to not pull)? ";
			cin>>pull;
			}
		}while (pull==1);
		cout<<"Thanks for playing slot machine. Press any key to quit Slot Machine";
		getch();
		return(0);
		}
```

