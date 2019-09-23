# String_pallindrone

package elclipse;

public class String_palin {

	public static void main(String[] args) {
		// TODO Auto-generated method stub

		String x="too hot t hoot";    
		x=x.replace(" ","");                 //replacing character
		x=x.toUpperCase();                  ///converting to uppercase
		char y[]=x.toCharArray();
		int size=y.length;
		int a[]=new int [size];
		int i=0;
		while(i!=size) {
			a[size-1-i]=y[i];                   ///reversing the string
			i++;
		}
		i=0;
		while(i!=size) {
			if(a[i]!=y[i]) {
				System.out.print("Not pallindrone");      
				System.exit(0);
			}
			else {
				i++;
				continue;
			}
		}
		System.out.println("pallindrone");


	}

}
/////time complexity is O(n)
