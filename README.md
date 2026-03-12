# Flipkart Selenium Automation Assignment

## Project Description
This project automates a product search scenario on the Flipkart website using Java, Selenium WebDriver, and Maven.

The automation script performs the following steps:
1. Opens the Flipkart website.
2. Closes the login popup if it appears.
3. Searches for **Bluetooth Speakers**.
4. Applies filters:
   - Brand → boAt
   - Customer Ratings → 4★ & above
5. Sorts the results by Price – Low to High.
6. Opens the first product in a new tab.
7. Checks the Available offers section and prints the number of offers in the console.
8. Verifies the Add to Cart functionality.

## Test Scenarios

### Scenario 1: Product Available
If the Add to Cart button is available:
- Click Add to Cart
- Navigate to the cart page
- Capture screenshot named cart_result.png

### Scenario 2: Product Not Available
If:
- Add to Cart button is missing
- Add to Cart button is disabled
- Product shows Out of Stock

Then:
- Print the message in console:
  `Product unavailable — could not be added to cart.`
- Capture screenshot named result.png

## Technologies Used
- Java
- Selenium WebDriver
- Maven
- ChromeDriver
- Eclipse IDE

## Project Structure

src/test/java/FlipkartAutomation1
- BaseTest.java
- FlipkartHomePage.java
- SearchResultsPage.java
- ProductPage.java
- CartPage.java
- MainTest.java

screenshots
- cart_result.png
- result.png

pom.xml

## How to Run the Project

1. Clone the repository.
2. Open the project in Eclipse or IntelliJ.
3. Make sure Maven dependencies are downloaded.
4. Run the file:

`MainTest.java`

5. The automation will start executing and screenshots will be saved in the **screenshots** folder.

## Output
- Console logs showing automation steps.
- Screenshot when product added to cart.
- Screenshot when product unavailable.
