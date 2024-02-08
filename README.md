//separating 0's and 1's using two pointer approach
public class Main
{
	public static void main(String[] args) {
	    //int a[]=new int[7];
	    int a[]={0,1,0,1,0,0,1,1};
	    int i=0;
	    int j=a.length-1;
	    while(i<j){
	        if(a[i]==0)
	        {
	            i++;
	        }
	        else if(a[j]==1){
	            j--;
	        }
	        else{
	            int temp;
	            temp=a[i];
	            a[i]=a[j];
	            a[j]=temp;
	        }
	    }
	    for(int k=0;k<a.length;k++){
	        System.out.println(a[k]);
	    }
		
	}
}
