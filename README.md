public class GuGuDan {

    public static void main(String[] args) {
        int i =1;
        int dan =1;

        System.out.printf("%2s%n","[구구단 출력]");
        //단 표시
        for (dan = 1; dan < 10; dan++) {
            System.out.print( String.format("%2s","[")+
                              String.format("%2d",dan)+
                              String.format("%2s","단 ]")+
                              String.format("%2s","\t") );
        }
        System.out.println();
        // n x n 만들기
        for (dan = 1; dan <10; dan++) {
            for ( i = 1; i < 10; i++) {
                int result = i * dan;

                System.out.print( String.format("%d",i)
                                + String.format("%2s","x")
                                + String.format("%2d",dan)
                                + String.format("%2s","=")
                                + String.format("%2d",result)
                                + String.format("%2s","\t"));
            }
            System.out.println();
        }
    }
}
