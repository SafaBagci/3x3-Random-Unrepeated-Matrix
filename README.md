# 3x3-Random-Unrepeated-Matrix



public class rand {

	public static void main(String[] args) {
		
		int ary[][] = new int [3][3];
		int line;
		int row;
		for(int i = 1; i <= 9; i++){
			do{
				line = (int)(Math.random()*3);
				row = (int)(Math.random()*3);
			}
			while(ary[line][row] != 0);
		
			ary[line][row] = i;
		}
		show(ary);
	}
	public static void show(int a[][]){
		
		for(int i = 0; i < 3; i++){
			for(int j = 0; j < 3; j++){
				
				System.out.print(a[i][j] + "  ");
			}
			System.out.println();
		}
	}
}
