package Ayaw;

import java.util.Scanner;

public class GradingSystem {

  public static void main(String[] args) {
  
  Scanner s = new Scanner(System.in);
  
 	System.out.print ("Enter your grade in PROGRAMMING LEC : ");
	 float proglec = s.nextFloat();
	 
	 System.out.print ("Enter your grade in PROGRAMMING LAB : ");
	 float proglab = s.nextFloat();
	 
	 System.out.print ("Enter your grade IN PANLIPUNAN      : ");
	 float panli = s.nextFloat();
	 
	 System.out.print ("Enter your grade in DISSTRU 1       : ");
	 float distru = s.nextFloat();
	 
	 System.out.print ("Enter your grade in GEPURPCOM       : ");
	 float purcom = s.nextFloat();
	 
	 System.out.print ("Enter your grade in REMMCRAT        : ");
	 float rem = s.nextFloat();
	 
	 System.out.print ("Enter your grade in GEFILDIS        : ");
	 float fildis = s.nextFloat();
	 
	 System.out.print ("Enter your grade in N.S.T.P         : ");
	 float nstp = s.nextFloat();
	 
	 System.out.print ("Enter your grade in DBMLEC          : ");
	 float dbmslec = s.nextFloat();
	 
	 System.out.print ("Enter your grade in DBMLAB          : ");
	 float dbmslab = s.nextFloat();
	 
	 System.out.print ("Enter your grade in P.E 2           : ");
	 float pe = s.nextFloat();
	 
	 float average = (proglec + proglab + 
				dbmslec + dbmslab +							purcom  + fildis  + 
				panli   + purcom  + 							nstp    + rem     + 
				pe ) / 11;

	 System.out.println ();
	 System.out.println("GENERAL AVERAGE	              	       : " + average);
	 
	 if (average > 100) System.out.println("INVALID GRADES");
	 else if (average >= 98) System.out.println("WITH HIGHEST HONORS");
	 else if (average >= 95) System.out.println("WITH HIGH HONORS");
	 else if (average >= 90) System.out.println("WITH HONORS");
	 else if (average >= 75) System.out.println("PASSED");
	 else System.out.println("FAILED");
  }

}
