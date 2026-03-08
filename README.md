# tugas1
Tugas1 dari mata kuliah struktur data yang mengerjakan tentang selection sort
```
package slectionsort;

public class slectionsort{
    public static void main(String[] args){
        int[] x = {20, 15, 90, 13, 26};
        int n = x.length;
        
        System.out.print("Awal: [");
        for (int i = 0; i < n; i++) {
            System.out.print(x[i]);
            if (i < n - 1) System.out.print(", ");
        }
        System.out.println("]");
        
        for (int i = 0; i < n - 1; i++) {
            int min = i;
            for (int j = i + 1; j < n; j++) {
                if (x[j] < x[min]) {
                    min = j;
                }
            }
            if (min != i) {
                int temp = x[i];
                x[i] = x[min];
                x[min] = temp;
            }
            System.out.print("Iterasi " + (i + 1) + ": [");
            for (int o = 0; o < n; o++) {
                System.out.print(x[o]);
                if (o < n - 1) System.out.print(", ");
            }
            System.out.println("]");
            
         
        }
    }
}
```
hasil atau output dari codingan diatas


<img width="356" height="181" alt="Cuplikan layar 2026-03-08 202746" src="https://github.com/user-attachments/assets/4332054a-333f-4243-9aa9-162af5ada293" />

