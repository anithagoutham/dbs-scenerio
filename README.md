package selenium_package;


	
	
	import org.openqa.selenium.By;
	import org.openqa.selenium.WebDriver;
	import org.openqa.selenium.WebElement;
	import org.openqa.selenium.chrome.ChromeDriver;


	public class interview {	

		

		public static void main(String[] args) throws InterruptedException {
		System.setProperty("weddriver.chrome.driver","E:\\Selenium\\New folder\\chromedriver_win32_2.zip");
				
				WebDriver driver = new ChromeDriver();
				
				driver.get("http://www.dms.com.sg");
			
				driver.findElement(By.xpath("//a[text()='Cards']")).click();
				
				driver.findElement(By.tagName("//a[text()='Credit Cards']']")).click();
				
				WebElement Alt= driver.findElement(By.className("compare-label"));
				WebElement Black = driver.findElement(By.className("compare-label"));
				
				
				
				if(Alt.equals(Black))
				{
					System.out.println("Test is passed");
				}
				else
				{
					System.out.println("Test is Failed");
				}	
			  Thread.sleep(3000);	
			}		    
				
				

			}

		
