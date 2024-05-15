package login;

import org.openqa.selenium.By;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;

public class flipkartpage {

	public static void main(String[] args) {
		// TODO Auto-generated method stub

		
		
		ChromeDriver driver = new ChromeDriver();
		 
		 driver.get("https://www.flipkart.com/");
		
		WebElement searchbox = driver.findElement(By.name("q"));
		searchbox.sendKeys( new CharSequence[] {"Iphone15"});
		searchbox.submit();
		
		
     		driver.findElement(By.xpath("//*[@id=\"container\"]/div/div[3]/div[1]/div[2]/div[3]/div/div/div/a/div[2]/div[1]/div[1]")).click();
		

			// directly page path 	
//	 driver.get("https://www.flipkart.com/apple-iphone-15-black-128-gb/p/itm6ac6485515ae4?pid=MOBGTAGPTB3VS24W&lid=LSTMOBGTAGPTB3VS24WVZNSC6&marketplace=FLIPKART&q=iphone+15&store=tyy%2F4io&srno=s_1_2&otracker=AS_QueryStore_OrganicAutoSuggest_2_6_na_na_na&otracker1=AS_QueryStore_OrganicAutoSuggest_2_6_na_na_na&fm=organic&iid=c3cafb89-92a5-477b-9e32-06db5566aa42.MOBGTAGPTB3VS24W.SEARCH&ppt=None&ppn=None&ssid=z71raswv280000001712918202595&qH=2f54b45b321e3ae5");
		
		 
		
//	WebElement BuyNow = driver.findElement(By.xpath("//*[@id=\"container\"]/div/div[3]/div[1]/div[1]/div[2]/div/ul/li[2]/form/button"))

//     		  driver.findElement(By.linkText("https://www.flipkart.com/checkout/init?otracker=search")).click();

     		
     	// Or using CSS selector:
            WebElement buyNow = driver.findElement(By.xpath("//*[@id=\"container\"]/div/div[3]/div[1]/div[1]/div[2]/div/ul/li[2]/form/button"));

            // Click the "Buy Now" button
            buyNow.click();

     		
	
	
	}

}
