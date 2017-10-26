# hw
/**
 * Auto Generated Java Class.
 */
public class APLine {
  
  public APLine(int x, int y, int z) 
  { 
    /* YOUR CONSTRUCTOR CODE HERE*/
    int a = x;
    int b = y;
    int c = z;
  }
  public double getSlope()
  {
    double slope = (-b/a);
    return slope;
  }
  public boolean isOnLine(int x, int y)
  {
    return (a*x + b*y + c) == 0;
  }
  
}
  
  public static void main(String[] args) { 
    
  
  APLine line1 = new APLine(5,4,-17);
  double slope1 = line1.getSlope();
  /* ADD YOUR CODE HERE */
  
}


