# Web-Scraping Using Selenium and BeautifulSoup
Recently, I've been diving deep into web scraping techniques, specifically utilizing the power of Selenium and Beautiful Soup. 
In this repository, you'll find examples of both Selenium and Beautiful Soup. Each project showcases the same use cases and demonstrates the power and flexibility of these libraries.

### Selenium
Selenium is a powerful tool that allows for browser automation. With Selenium, we can simulate user interactions, such as clicking buttons, filling out forms, and navigating through web pages. This capability is particularly useful when dealing with websites that heavily rely on JavaScript or AJAX requests. By automating the browser, we can extract data that would otherwise be inaccessible through traditional scraping methods.

### BeautifulSoup
Beautiful Soup, on the other hand, is a Python library specifically designed for parsing HTML and XML documents. It provides a convenient way to navigate and search through the document's structure, making it effortless to extract desired information. Beautiful Soup is especially handy when working with static websites or when combined with Selenium for scraping dynamically generated content.

## Project Description
This project demonstrates how to scrape data from https://books.toscrape.com using both Selenium and Beautiful Soup. It covers scenarios where Selenium interacts with elements and navigates through the website, while Beautiful Soup extracts the desired data from the HTML structure.

## Setting up Selenium
To set up Selenium, follow these steps:

**Install Python:** Selenium is a Python library, so you need to have Python installed on your system. You can download the latest version of Python from the official website at https://www.python.org/downloads/. Follow the installation instructions specific to your operating system.

**Install Selenium:** Once you have Python installed, you can install Selenium using pip, the package manager for Python. Open your command prompt or terminal and run the following command:

<pre><code>
pip install selenium
</code></pre>

This command will download and install the Selenium library along with its dependencies.

The source of downloads for Selenium WebDriver varies depending on your Operating System and preferred browser. In this example, we will focus on using Chrome. To begin, verify the installed version of Chrome by clicking the three dots at the top right of the Chrome window, selecting "About," and noting the version number displayed. This version of the information is crucial for obtaining the correct driver.

**Download WebDriver:** WebDriver is a component of Selenium that interacts with the web browser. The choice of WebDriver depends on the browser you want to automate. Here are the popular web browsers and their corresponding WebDriver:

**Chrome:** Download ChromeDriver from the official website at https://sites.google.com/a/chromium.org/chromedriver/downloads. Make sure to choose the version compatible with your Chrome browser.

**Firefox:** Download GeckoDriver from the official website at https://github.com/mozilla/geckodriver/releases. Choose the appropriate version for your Firefox browser.

**Edge:** Download Microsoft WebDriver from the official website at https://developer.microsoft.com/en-us/microsoft-edge/tools/webdriver/. Select the version that matches your Edge browser.
Ensure that the WebDriver executable is in your system's PATH environment variable. This allows Selenium to locate the WebDriver when executing your scripts.

**Verify Installation:** To verify that Selenium is properly installed, open a Python interpreter, or create a new Python script. Import the Selenium module by adding the following line at the beginning:

<pre><code>
  from selenium import webdriver
</code>
</pre>

If the import statement doesn't throw any errors, it means Selenium is installed correctly.

**Run a Test:** Now you're ready to run a simple Selenium test. Add the following code to your script:

<pre>
  <code>
    from selenium import webdriver
    # Create a WebDriver instance for Chrome
    driver = webdriver.Chrome()
    # Open a website
    driver.get('https://www.example.com')
    # Print the page title
    print(driver.title)
    # Close the browser
    driver.quit()
  </code>
</pre>

When you run this script, it will open the specified website in the browser controlled by Selenium, retrieve the page title, print it to the console, and then close the browser.

## Setting up BeautifulSoup

To set up Beautiful Soup, follow these steps:

**Install Beautiful Soup:**  Beautiful Soup is a Python library, so you need to install it. You can use pip, the package manager for Python, to install Beautiful Soup. Open your command prompt or terminal and run the following command:

<pre>
  <code>
    pip install beautifulsoup4
  </code>
</pre>

This command will download and install the Beautiful Soup library along with its dependencies.

I**mport Beautiful Soup:** Once you have Beautiful Soup installed, you can start using it in your Python scripts. Import the library by adding the following line at the beginning of your script:

<pre>
  <code>
    from bs4 import BeautifulSoup
  </code>
</pre>

This import statement will make the Beautiful Soup module available for use in your script.
