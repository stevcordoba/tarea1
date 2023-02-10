 public static void main(String[] args) {
       ArrayList<String> lista = new ArrayList<>();
       lista.add("Esta oración es de prueba");
 
for(int i=0; i<lista.size(); ++i) {
    lista.set(i, lista.get(i).replaceAll("(?iu)[aeiouáéíóúü]", ""));
}

for(String s : lista) {
    System.out.println(s);
}

public static int sumanat (int suma){
    int res;
       if (suma>0){
          res= suma+ sumanat(suma-1);
 }
       else {
            return 0;
        }
       return res;
    }    
 
public static void checkBinary(int num) {
    if (num == 0) {
        System.out.println("Es binario");
        return;
    }
    if (num % 10 > 1) {
        System.out.println("No es binario");
        return;
    }
    checkBinary(num / 10);
}
    public double calcExponencial (int n, int x){
        if(x==1)  
            return n;
        else if(x==0)
                return 1;
            else
                return n* calcExponencial(n,x-1);
         }
    }
    
public double factorial (int num){
 
            if(num<=1){
                return num;
            }
            return num * factorial(num - 1);
        }
