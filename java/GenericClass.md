# generic class 
 class Main <T>
{
    T i;
    public void add(T i){
      this.i=i;
    }
    public T get(){
        return i;
    }
	public static void main(String[] args) {
		Main<Integer> m1 = new Main<Integer>();
		Main<String> m2 = new Main<String>();
	//	Integer m3 = new Integer(23);
		m1.add(23);
		m2.add("sakshi");
		System.out.println("m1: " +m1.get()+ " m2: " +m2.get());
		
	}
}
