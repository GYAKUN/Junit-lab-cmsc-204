import static org.junit.Assert.assertEquals;

import static org.junit.Assert.assertTrue;

import org.junit.After;

import org.junit.Before;

import org.junit.Test;

public class GradeBookTest {

	private GradeBook g1, g2;

  @Before
  public void setUp() throws Exception {
  
	  g1 = new GradeBook(5);
    
	  g1.addScore(10);
    
	  g1.addScore(20);
    
	  g1.addScore(30);
    
	  g1.addScore(40);
    
	  g2 = new GradeBook(5);
    
	  g2.addScore(0);
    
	  g2.addScore(25);
    
	  g2.addScore(50);
    
	  g2.addScore(75);
  }

  @After
  
  public void tearDown() throws Exception {
  
	  g1 = g2 = null;
  }

  @Test
  
  public void testAddScore() {
  
	  assertTrue(g1.toString().equals("10.0 20.0 30.0 40.0 "));
    
	  assertEquals(4, g1.getScoresSize());
    
    
	  assertTrue(g2.toString().equals("0.0 25.0 50.0 75.0 "));
    
	  assertEquals(4, g2.getScoresSize());
  }

  @Test
  
  public void testSum() {
  
	  assertEquals(100, g1.sum(), 0.001);
    
	  assertEquals(150, g2.sum(), 0.001);
  
  }

  @Test
  
  public void testMinimum() {
  
	  assertEquals(10, g1.minimum(), 0.001);
    
	  assertEquals(0, g2.minimum(), 0.001);
  
  }

  @Test
  
  public void testFinalScore() {
  
	  assertEquals(90, g1.finalScore(), 0.001);
    
	  assertEquals(150, g2.finalScore(), 0.001);
 
  }

}
