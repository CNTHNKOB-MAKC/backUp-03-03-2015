package core.TestRunner1;
    

 
import java.util.concurrent.TimeUnit;

import org.openqa.selenium.WebDriver;
import org.openqa.selenium.firefox.FirefoxDriver;

 

 


public class TestRunnerSingleTitleValidation {
	public static void main(String[] argsPHAKIN) {
		 
		WebDriver driver = new FirefoxDriver();    // Version 1.1 :: Firefox
 
		String text_case_id = "TC-001.01Selenium";
	  String url = "http://www.newsli.ru/";
	 String titleExpected = "Newsli - новости из первых уст";
		

		
	/* String[] param = argsPHAKIN[0].split("\\|");//to use command line argument [single]
	 	String url = param [0];
 	String titleExpected = param[1];
		*/
 		
		
		driver.get(url);
		driver.manage().timeouts().implicitlyWait(30, TimeUnit.SECONDS);
		String title_actual = driver.getTitle();
 
		if (titleExpected.equals(title_actual)) {
			System.out.println("Test Case ID: \t\t" + text_case_id);
			System.out.println("URL: \t\t\t" + url);
			System.out.println("Title Expected: \t" + titleExpected);
			System.out.println("Title Actual: \t\t" + title_actual);
			System.out.println("Test Case Result: \t" + "PASSED");
		} else {
			System.out.println("Test Case ID: \t\t" + text_case_id);
			System.out.println("URL: \t\t\t" + url);
			System.out.println("Title Expected: \t" + titleExpected);
			System.out.println("Title Actual: \t\t" + title_actual);
			System.out.println("Test Case Result: \t" + "FAILED");
		}
		driver.quit();
	}
}