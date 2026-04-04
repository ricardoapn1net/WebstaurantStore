# WebstaurantStore
WebstaurantStore - WebstaurantStore Code Screen Task

# *** WebstaurantStore Code Screen Task ***
#* This script will extract all products pages URLs from the three outlet pages.
#* It uses the regular expression extractor to extract all product links from those pages.
  - Prevents the need to of having to load them from a random ".csv" file.
  - Prevents the need to update the script anytime a product is added, changed or removed.
  - These URLs are all stored in three "product" variables. "products_page1", "products_page2" & "products_page3".
#* A product is then selected at random from one of the 3 product pages variables using the "RandomFromMultipleVars" function.
  - The product link is then stored in the "product" parameter.
#* The Product page transaction contains a total of 14 samplers plus the transaction itself.
  - Throughput is set to 75 requests/min (5 transactions/min).
  - Throughput is controlled by the "Constant Througput Timer".
#* The "clarkAssociates_Outlet_04_product_page" transaction will have the average transaction response time from all the loaded product pages.
  - If there is a need to see individual product pages response times in the resulting report, it can be accomplished by unselecting the "Generate parent sample" of the transaction controller.
#* Test will run for a duration of 15 minutes
#* Values of the User Defined Variables can be changed from the command line when running the load test from the CLI except for the hostname which is hardcoded.
