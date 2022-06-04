class Main {
    
    String dna1 = "ATGCGATACGCTTGA";
    String dna2 = "ATGCGATACGTGA";
    String dna3 = "ATTAATATGTACTGA";
    String dna = dna1;

  public void myMethod(){
    int dna1ATG = dna1.indexOf("ATG");
    int dna2ATG = dna2.indexOf("ATG");
    int dna3ATG = dna3.indexOf("ATG");
      
    int dna1TGA = dna1.indexOf("TGA");
    int dna2TGA = dna2.indexOf("TGA");
    int dna3TGA = dna3.indexOf("TGA");
    
    if (dna1ATG < 0 || dna1TGA < 0 || (dna1TGA - dna1ATG) % 3 != 0){
        System.out.println("dna1 is not a protein");
    } else {
        System.out.println("dna1 is a protein");
    }
    
        if (dna2ATG < 0 || dna2TGA < 0 || (dna2TGA - dna2ATG) % 3 != 0){
        System.out.println("dna2 is not a protein");
    } else {
        System.out.println("dna2 is a protein");
    }
    
        if (dna3ATG < 0 || dna3TGA < 0 || (dna3TGA - dna3ATG) % 3 != 0){
        System.out.println("dna3 is not a protein");
    } else {
        System.out.println("dna3 is a protein");
    }
  }
    public static void main(String[] args) {
        Main James = new Main();
        James.myMethod();
    }
    }
