 public static void main(String[] args) {
       ArrayList<String> lista = new ArrayList<>();
       lista.add("Esta oración es de prueba");
       

for(int i=0; i<lista.size(); ++i) {
    lista.set(i, lista.get(i).replaceAll("(?iu)[aeiouáéíóúü]", ""));
}

for(String s : lista) {
    System.out.println(s);
}
    }
}  
