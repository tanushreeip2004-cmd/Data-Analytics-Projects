create database e_commerce ;
use e_commerce;

-- Now Creating the tables to populate the database and do futher analysis--
CREATE TABLE Products (
    ProductID INT AUTO_INCREMENT PRIMARY KEY, -- Unique ID for each product
    ProductName VARCHAR(255) NOT NULL, -- Stores just the name of the product
    Description TEXT, -- Stores a description of the product
    Price DECIMAL(10, 2) NOT NULL, -- Stores a single price for the product
    StockQuantity INT NOT NULL, -- Stores the number of items in stock
    Category VARCHAR(100), -- Stores the category of the product
    DateAdded DATE NOT NULL DEFAULT (CURDATE()) -- Stores the date when the product was added
);
-- POPULATING THE PRODUCTS TABLE -- 
INSERT INTO Products (ProductName, Description, Price, StockQuantity, Category) VALUES
('Widget A', 'Basic widget for general use', 120.00, 50, 'Widgets'),
('Tool A', 'Durable hand tool', 200.00, 35, 'Tools'),
('Robot Cleaner', 'An automated vacuum for home use.', 350.00, 25, 'Robotics'),
('Smart Lock', 'Keyless entry for your home.', 180.00, 40, 'Smart Home'),
('Portable Speaker', 'High-quality sound on the go.', 85.00, 60, 'Audio'),
('Wireless Earbuds', 'Noise-canceling earbuds with long battery life.', 125.00, 75, 'Audio'),
('Desktop PC', 'Powerful computer for gaming and work.', 1200.00, 15, 'Computers'),
('Gaming Keyboard', 'Mechanical keyboard with customizable RGB lighting.', 95.00, 50, 'Computers'),
('Fitness Tracker', 'Monitors heart rate, steps, and sleep.', 70.00, 90, 'Wearables'),
('Smartwatch', 'Tracks fitness, receives notifications, and more.', 250.00, 35, 'Wearables'),
('Espresso Machine', 'Makes café-quality espresso at home.', 450.00, 20, 'Kitchen Appliances'),
('Air Fryer', 'Cooks food with little to no oil.', 110.00, 55, 'Kitchen Appliances'),
('Digital Camera', 'High-resolution camera for professional photos.', 600.00, 18, 'Photography'),
('Drone', 'Quad-copter with a 4K camera.', 800.00, 12, 'Drones'),
('E-Reader', 'Lightweight device for reading books.', 150.00, 30, 'Books & Media'),
('Graphic Tablet', 'For digital artists and designers.', 280.00, 22, 'Creative Tools'),
('3D Printer', 'Creates three-dimensional objects from a digital file.', 950.00, 10, '3D Printing'),
('Smart Thermostat', 'Controls home temperature remotely.', 140.00, 45, 'Smart Home'),
('Solar Charger', 'Portable charger powered by the sun.', 50.00, 80, 'Outdoor Gear'),
('Tent', 'A lightweight, durable tent for two people.', 130.00, 30, 'Outdoor Gear'),
('Cookware Set', 'Non-stick pans and pots set.', 180.00, 40, 'Kitchenware'),
('Blender', 'High-speed blender for smoothies and shakes.', 75.00, 65, 'Kitchen Appliances'),
('Yoga Mat', 'Non-slip mat for yoga and pilates.', 30.00, 100, 'Fitness'),
('Dumbbell Set', 'Adjustable weight dumbbell set.', 150.00, 25, 'Fitness'),
('Gardening Gloves', 'Durable gloves for all gardening tasks.', 15.00, 120, 'Gardening'),
('Smart TV', '4K Ultra HD television with smart features.', 700.00, 20, 'Televisions'),
('Projector', 'Portable projector for home cinema.', 250.00, 15, 'Televisions'),
('Microphone', 'Studio-quality USB microphone.', 90.00, 50, 'Audio'),
('Portable Monitor', 'An extra screen for your laptop on the go.', 220.00, 35, 'Computers'),
('Electric Kettle', 'Boils water quickly with auto shut-off.', 45.00, 70, 'Kitchen Appliances'),
('Misc Item B', 'General purpose item', 110.00, 55, 'Miscellaneous'),
('Machine A', 'Heavy-duty machine for production', 500.00, 15, 'Machines'),
('Instrument A', 'Measuring instrument', 300.00, 30, 'Instruments'),
('Gizmo B', 'Portable gizmo with extra features', 170.00, 65, 'Gizmos'),
('Gadget A', 'Popular everyday gadget', 210.00, 45, 'Gadgets'),
('Device A', 'Electronic device for communication', 400.00, 25, 'Devices'),
('Contraption A', 'Unique mechanical contraption', 600.00, 18, 'Contraptions'),
('Appliance A', 'Home appliance for daily use', 800.00, 20, 'Appliances'),
('Apparatus A', 'Industrial apparatus', 1000.00, 10, 'Apparatus');

-- Checking the products table--
select * from products;

-- Creating the users table--
CREATE TABLE Users (
    UserID INT AUTO_INCREMENT PRIMARY KEY, -- Unique ID for each user
    UserName VARCHAR(255) NOT NULL, -- Stores the user's name
    Email VARCHAR(255) NOT NULL UNIQUE, -- Stores the user's email, which must be unique
    Address VARCHAR(255) -- Stores the user's address
);

-- POPULATING THE USERS TABLE--
 INSERT INTO Users (UserName, Email, Address) VALUES
('Sanjay Sharma', 'sanjay.sharma@example.com', '101 MG Road, Bangalore'),
('Deepa Reddy', 'deepa.reddy@example.com', '20 Subhash Nagar, Chennai'),
('Aamir Khan', 'aamir.khan@example.com', '33 Lajpat Nagar, Delhi'),
('Pooja Shah', 'pooja.shah@example.com', '44 Juhu, Mumbai'),
('Rohit Verma', 'rohit.verma@example.com', '55 DLF Phase 4, Gurgaon'),
('Shweta Tiwari', 'shweta.tiwari@example.com', '66 Viman Nagar, Pune'),
('Gaurav Joshi', 'gaurav.joshi@example.com', '77 Civil Lines, Allahabad'),
('Nisha Singh', 'nisha.singh@example.com', '88 Gomti Nagar, Lucknow'),
('Vivek Agnihotri', 'vivek.agnihotri@example.com', '99 Indiranagar, Bangalore'),
('Lata Mangeshkar', 'lata.mangeshkar@example.com', '11 Linking Road, Mumbai'),
('Ravi Shankar', 'ravi.shankar@example.com', '22 Sector 10, Chandigarh'),
('Sonali Bendre', 'sonali.bendre@example.com', '31 Green Park, Delhi'),
('Praveen Kumar', 'praveen.kumar@example.com', '42 HSR Layout, Bangalore'),
('Anita Deshpande', 'anita.deshpande@example.com', '53 Karol Bagh, Delhi'),
('Bhavna Singh', 'bhavna.singh@example.com', '64 Ballygunge, Kolkata'),
('Chetan Bhagat', 'chetan.bhagat@example.com', '75 Malabar Hill, Mumbai'),
('Divya Dutta', 'divya.dutta@example.com', '86 Rajendra Nagar, Patna'),
('Esha Deol', 'esha.deol@example.com', '97 Gwalior Road, Agra'),
('Faisal Khan', 'faisal.khan@example.com', '108 Marine Drive, Mumbai'),
('Gautam Gambhir', 'gautam.gambhir@example.com', '19 Defence Colony, Delhi'),
('Harshita Jain', 'harshita.jain@example.com', '28 Panvel, Navi Mumbai'),
('Irfan Pathan', 'irfan.pathan@example.com', '37 Sardar Patel Road, Ahmedabad'),
('Jaya Bachchan', 'jaya.bachchan@example.com', '46 Juhu, Mumbai'),
('Kailash Kher', 'kailash.kher@example.com', '59 Baner, Pune'),
('Lokesh Singh', 'lokesh.singh@example.com', '68 Anna Nagar, Chennai'),
('Manish Pandey', 'manish.pandey@example.com', '79 Whitefield, Bangalore'),
('Nandita Das', 'nandita.das@example.com', '87 Tollygunge, Kolkata'),
('Om Puri', 'om.puri@example.com', '96 Andheri East, Mumbai'),
('Pranav Kumar', 'pranav.kumar@example.com', '105 Sector 5, Panchkula'),
('Qamar Zafar', 'qamar.zafar@example.com', '114 Saket, Delhi'),
('Priya Verma', 'priya.verma@example.com', '45 Sector 18, Noida'),
('Rahul Khanna', 'rahul.khanna@example.com', '78 Park Street, Kolkata'),
('Sneha Patel', 'sneha.patel@example.com', '12 Civil Lines, Lucknow'),
('Arjun Mehta', 'arjun.mehta@example.com', '56 Andheri West, Mumbai'),
('Neha Singh', 'neha.singh@example.com', '89 Connaught Place, Delhi'),
('Vikram Rao', 'vikram.rao@example.com', '34 Jubilee Hills, Hyderabad'),
('Anjali Gupta', 'anjali.gupta@example.com', '67 Koregaon Park, Pune'),
('Karan Malhotra', 'karan.malhotra@example.com', '90 Banjara Hills, Hyderabad'),
('Ritika Kapoor', 'ritika.kapoor@example.com', '23 Marine Drive, Mumbai');

-- Checking the users table --
select * from users;

-- Creating the orders table--
CREATE TABLE Orders (
    OrderID INT AUTO_INCREMENT PRIMARY KEY, -- Unique ID for each order
    UserID INT, -- ID of the user who placed the order
    OrderDate DATE NOT NULL, -- Date when the order was placed
    TotalAmount DECIMAL(10, 2) NOT NULL, -- Total amount of the order
    FOREIGN KEY (UserID) REFERENCES Users(UserID) -- Link to the Users table
);

INSERT INTO Orders (UserID, OrderDate, TotalAmount) VALUES
(1, '2024-09-01', 270.00),   
(2, '2024-09-02', 450.00),   
(3, '2024-09-03', 110.00),   
(4, '2024-09-05', 1250.00),  
(5, '2024-09-06', 320.00),   
(6, '2024-09-07', 480.00),   
(7, '2024-09-08', 600.00),     
(8, '2024-09-10', 950.00),   
(9, '2024-09-12', 130.00),
(10, '2024-09-15', 750.00),
(11, '2024-09-16', 300.00),
(12, '2024-09-18', 150.00),
(13, '2024-09-19', 400.00),
(14, '2024-09-20', 650.00),
(15, '2024-09-21', 80.00),
(16, '2024-09-22', 900.00),
(17, '2024-09-24', 550.00),
(18, '2024-09-25', 1050.00),
(19, '2024-09-26', 220.00),
(20, '2024-09-28', 180.00),
(21, '2024-09-29', 1100.00),
(22, '2024-09-30', 380.00),
(23, '2024-10-01', 520.00),
(24, '2024-10-03', 700.00),
(25, '2024-10-04', 120.00),
(26, '2024-10-05', 680.00),
(27, '2024-10-06', 420.00),
(28, '2024-10-08', 290.00),
(29, '2024-10-09', 850.00),
(30, '2024-10-10', 1000.00),
(31, '2024-10-11', 250.00),
(32, '2024-10-13', 460.00),
(33, '2024-10-14', 630.00),
(34, '2024-10-15', 350.00),
(35, '2024-10-17', 590.00),
(36, '2024-10-18', 920.00),
(37, '2024-10-20', 170.00),
(38, '2024-10-21', 780.00),
(39, '2024-10-22', 140.00);

-- Checking the orders table--
select * from orders;

-- Creating the reviews table to collect customers feedback on our orders --
CREATE TABLE Reviews (
    ReviewID INT AUTO_INCREMENT PRIMARY KEY, -- Unique ID for each review
    ProductID INT, -- ID of the product being reviewed
    UserID INT, -- ID of the user who wrote the review
    Rating INT, -- Rating given by the user (1 to 5 stars)
    ReviewText TEXT, -- Text of the review
    FOREIGN KEY (ProductID) REFERENCES Products(ProductID), -- Link to the Products table
    FOREIGN KEY (UserID) REFERENCES Users(UserID), -- Link to the Users table
    CHECK (Rating >= 1 AND Rating <= 5) -- Ensure the rating is between 1 and 5
);

-- Populating the Reviews Table--
INSERT INTO Reviews (ProductID, UserID, Rating, ReviewText) VALUES
(1, 1, 5, 'Excellent quality widget, very useful.'),
(2, 2, 4, 'Good widget but a bit expensive.'),
(3, 3, 5, 'The tool is very durable and reliable.'),
(4, 4, 3, 'Average tool, could be improved.'),
(5, 5, 4, 'Handy miscellaneous item, worth the price.'),
(6, 6, 2, 'Not very satisfied, quality could be better.'),
(7, 7, 5, 'The machine works perfectly for my needs.'),
(8, 8, 4, 'Compact machine, useful in small workshops.'),
(9, 9, 5, 'High precision instrument, highly recommended.'),
(10, 10, 4, 'Great instrument, but the price is a bit high.'),
(11, 11, 5, 'Fun and easy to use, perfect for a gift.'),
(12, 12, 3, 'The gizmo is alright, but the battery life is short.'),
(13, 13, 5, 'This gadget is a game-changer for daily tasks.'),
(14, 14, 4, 'Solid gadget, works as advertised.'),
(15, 15, 5, 'The device is excellent, fast, and reliable.'),
(16, 16, 4, 'Good device with many features.'),
(17, 17, 5, 'A truly unique and well-built contraption.'),
(18, 18, 3, 'This contraption is hard to set up.'),
(19, 19, 5, 'Amazing appliance, makes life easier.'),
(20, 20, 4, 'Smart appliance with great features, though a bit complex.'),
(21, 21, 5, 'The apparatus is robust and performs well.'),
(22, 22, 4, 'Scientific apparatus, very accurate.'),
(23, 23, 5, 'The robot cleaner is a lifesaver.'),
(24, 24, 4, 'Smart lock is great, but the app could be better.'),
(25, 25, 5, 'Awesome portable speaker, very clear sound.'),
(26, 26, 5, 'The wireless earbuds have great sound quality.'),
(27, 27, 5, 'Powerful and fast desktop computer.'),
(28, 28, 4, 'Great gaming keyboard, a bit noisy.'),
(29, 29, 5, 'The fitness tracker is very accurate.'),
(30, 30, 4, 'A nice smartwatch, but the battery drains fast.'),
(31, 31, 5, 'Makes perfect espresso every time.'),
(32, 32, 5, 'A must-have for every kitchen.'),
(33, 33, 4, 'Good camera, but the autofocus is a bit slow.'),
(34, 34, 5, 'The drone is a blast to fly.'),
(35, 35, 4, 'The e-reader is good for the price.'),
(36, 36, 5, 'A very responsive and useful graphic tablet.'),
(37, 37, 4, 'The 3D printer is good for hobbyists.'),
(38, 38, 5, 'Works perfectly, easy to install.'),
(39, 39, 4, 'A convenient solar charger for outdoor trips.');

-- Checking the Reviews Table --
select * from Reviews;

-- Adding the new ProductLaunchDate to the products table --

alter table products
add column ProductLaunchDate date;
select * from products;

-- populating the ProductLaunchDate's row --

-- Update the 'ProductLaunchDate' for each category of products
-- Here, we're setting the launch date for 'Widgets' to January 1, 2024

update products
set ProductLaunchDate = '2025-01-01'
where Category = 'widgets';

-- Set the launch date for 'Tools' to February 1, 2024
UPDATE Products 
SET ProductLaunchDate = '2024-02-01' 
WHERE Category = 'Tools';

-- Set the launch date for 'Miscellaneous' products to March 1, 2024
UPDATE Products 
SET ProductLaunchDate = '2024-03-01' 
WHERE Category = 'Miscellaneous';

-- Set the launch date for 'Machines' to April 1, 2024
UPDATE Products 
SET ProductLaunchDate = '2024-04-01' 
WHERE Category = 'Machines';

-- Set the launch date for 'Instruments' to May 1, 2024
UPDATE Products 
SET ProductLaunchDate = '2024-05-01' 
WHERE Category = 'Instruments';

-- Set the launch date for 'Gizmos' to June 1, 2024
UPDATE Products 
SET ProductLaunchDate = '2024-06-01' 
WHERE Category = 'Gizmos';

-- Set the launch date for 'Gadgets' to July 1, 2024
UPDATE Products 
SET ProductLaunchDate = '2024-07-01' 
WHERE Category = 'Gadgets';

-- Set the launch date for 'Devices' to August 1, 2024
UPDATE Products 
SET ProductLaunchDate = '2024-08-01' 
WHERE Category = 'Devices';

-- Set the launch date for 'Contraptions' to September 1, 2024
UPDATE Products 
SET ProductLaunchDate = '2024-09-01' 
WHERE Category = 'Contraptions';

-- Set the launch date for 'Appliances' to October 1, 2024
UPDATE Products 
SET ProductLaunchDate = '2024-10-01' 
WHERE Category = 'Appliances';

-- Set the launch date for 'Apparatus' to November 1, 2024
UPDATE Products 
SET ProductLaunchDate = '2024-11-01' 
WHERE Category = 'Apparatus';

UPDATE Products
SET ProductLaunchDate = '2024-01-15'
WHERE Category = 'Robotics';

UPDATE Products
SET ProductLaunchDate = '2024-02-20'
WHERE Category = 'Smart Home';

UPDATE Products
SET ProductLaunchDate = '2024-03-10'
WHERE Category = 'Audio';

UPDATE Products
SET ProductLaunchDate = '2024-04-05'
WHERE Category = 'Computers';

UPDATE Products
SET ProductLaunchDate = '2024-05-12'
WHERE Category = 'Wearables';

UPDATE Products
SET ProductLaunchDate = '2024-06-01'
WHERE Category = 'Kitchen Appliances';

UPDATE Products
SET ProductLaunchDate = '2024-07-18'
WHERE Category = 'Photography';

UPDATE Products
SET ProductLaunchDate = '2024-08-05'
WHERE Category = 'Drones';

UPDATE Products
SET ProductLaunchDate = '2024-09-01'
WHERE Category = 'Books & Media';

UPDATE Products
SET ProductLaunchDate = '2024-10-10'
WHERE Category = 'Creative Tools';

UPDATE Products
SET ProductLaunchDate = '2024-11-20'
WHERE Category = '3D Printing';

UPDATE Products
SET ProductLaunchDate = '2024-12-01'
WHERE Category = 'Smart Home';

UPDATE Products
SET ProductLaunchDate = '2024-05-25'
WHERE Category = 'Outdoor Gear';

UPDATE Products
SET ProductLaunchDate = '2024-06-15'
WHERE Category = 'Kitchenware';

UPDATE Products
SET ProductLaunchDate = '2024-07-07'
WHERE Category = 'Fitness';

UPDATE Products
SET ProductLaunchDate = '2024-08-01'
WHERE Category = 'Gardening';

UPDATE Products
SET ProductLaunchDate = '2024-09-05'
WHERE Category = 'Televisions';

UPDATE Products
SET ProductLaunchDate = '2024-10-22'
WHERE Category = 'Audio';

UPDATE Products
SET ProductLaunchDate = '2024-11-15'
WHERE Category = 'Computers';

UPDATE Products
SET ProductLaunchDate = '2024-12-05'
WHERE Category = 'Kitchen Appliances';

UPDATE Products
SET ProductLaunchDate = '2024-08-20'
WHERE Category = 'Health';

UPDATE Products
SET ProductLaunchDate = '2024-09-15'
WHERE Category = 'Home Decor';

UPDATE Products
SET ProductLaunchDate = '2024-10-01'
WHERE Category = 'Home Office';

UPDATE Products
SET ProductLaunchDate = '2024-11-01'
WHERE Category = 'Bags';

UPDATE Products
SET ProductLaunchDate = '2024-12-10'
WHERE Category = 'Drinkware';

-- Final check to ensure all new categories have a launch date
SELECT DISTINCT Category, ProductLaunchDate
FROM Products
ORDER BY ProductLaunchDate;

-- DATA VALIDATION aka Validating the data --

select ProductID,ProductName,ProductLaunchDate from products;

-- ensuring there are no null values in ProductLaunchDate column--
select count(*)
from products
where ProductLaunchDate is not null;

-- Checking the count of null, just to ensure there are no null values--
select count(*)
from products
where ProductLaunchDate is null;

-- Retrieve and display product details including the newly added 'ProductLaunchDate'
-- This helps you verify the integrity of the data after adding the constraint

SELECT ProductName, Price, StockQuantity, ProductLaunchDate 
FROM Products;

-- Group the products by 'ProductLaunchDate' and count how many products were launched on each date
-- This gives you an overview of product launches 

SELECT ProductLaunchDate, COUNT(*) AS NumberOfProducts 
FROM Products 
GROUP BY ProductLaunchDate;

-- Now, Tracking that which products were bought in which order--
-- we will be creating a orderdetails table --
-- creating OrderDetails table--
CREATE TABLE OrderDetails (
    OrderDetailID INT AUTO_INCREMENT PRIMARY KEY,
    OrderID INT,
    ProductID INT,
    Quantity INT NOT NULL,
    Price DECIMAL(10,2) NOT NULL,
    FOREIGN KEY (OrderID) REFERENCES Orders(OrderID),
    FOREIGN KEY (ProductID) REFERENCES Products(ProductID)
);
select * from orderdetails;
-- populating the orders table-- 
-- Populating the OrderDetails table --

INSERT INTO OrderDetails (OrderID, ProductID, Quantity, Price) VALUES
(1, 1, 1, 120.00),   
(1, 2, 1, 150.00),   
(2, 9, 1, 300.00),  
(2, 10, 1, 150.00),  
(3, 6, 1, 110.00),   
(4, 7, 1, 500.00),   
(4, 8, 1, 750.00),   
(5, 12, 1, 170.00),  
(5, 11, 1, 130.00),  
(6, 16, 1, 480.00),  
(7, 17, 1, 600.00),  
(8, 20, 1, 950.00),  
(9, 11, 1, 130.00),  
(10, 8, 1, 750.00),  
(11, 9, 1, 300.00),  
(12, 5, 1, 90.00),   
(12, 6, 1, 60.00),   
(13, 15, 1, 400.00), 
(14, 18, 1, 650.00), 
(15, 5, 1, 90.00),   
(16, 19, 1, 800.00), 
(17, 21, 1, 1000.00),
(17, 22, 1, 1200.00),
(18, 13, 1, 210.00), 
(19, 14, 1, 310.00), 
(20, 11, 1, 130.00),
(21, 22, 1, 1200.00),
(22, 16, 1, 480.00), 
(23, 15, 1, 400.00), 
(24, 7, 1, 500.00),  
(25, 6, 1, 110.00),  
(26, 19, 1, 800.00), 
(27, 2, 1, 150.00),  
(28, 1, 1, 120.00),  
(29, 9, 1, 300.00), 
(30, 1, 1, 120.00),  
(31, 12, 1, 170.00), 
(32, 16, 1, 480.00), 
(33, 20, 1, 950.00), 
(34, 1, 1, 120.00),  
(35, 17, 1, 600.00), 
(36, 18, 1, 700.00), 
(37, 5, 1, 90.00),   
(38, 15, 1, 400.00),
(39, 1, 1, 120.00);  
commit;

-- checking order Details table --
Select* from OrderDetails;

-- CONDUCTING SOME BUISNESS INSIGHTS --

-- 1.) Calculating the total sales per order-- 
SELECT p.ProductName, SUM(od.Quantity * od.Price) AS TotalSales
FROM OrderDetails od
JOIN Products p ON od.ProductID = p.ProductID
GROUP BY p.ProductName
ORDER BY TotalSales DESC;

-- 2.) TOP 5 Best-selling Products--
SELECT p.ProductName, SUM(od.Quantity) AS TotalUnitsSold, SUM(od.Quantity * od.Price) AS TotalRevenue
FROM OrderDetails od
JOIN Products p ON od.ProductID = p.ProductID
GROUP BY p.ProductName
ORDER BY TotalRevenue DESC
LIMIT 5;

-- 3.) Top 5 Customers by Spending-- 
SELECT u.UserName, u.Email, SUM(o.TotalAmount) AS TotalSpent
FROM Users u
JOIN Orders o ON u.UserID = o.UserID
GROUP BY u.UserID, u.UserName, u.Email
ORDER BY TotalSpent DESC
LIMIT 5;

-- 4.) Average Rating per Product --
SELECT p.ProductName, AVG(r.Rating) AS AvgRating, COUNT(r.ReviewID) AS ReviewCount
FROM Products p
LEFT JOIN Reviews r ON p.ProductID = r.ProductID
GROUP BY p.ProductName
ORDER BY AvgRating DESC;

-- 5.) Monthly Sales Trend-- 
SELECT DATE_FORMAT(OrderDate, '%Y-%m') AS Month, SUM(TotalAmount) AS MonthlyRevenue
FROM Orders
GROUP BY Month
ORDER BY Month;

-- 6.) Category-wise Sales --
SELECT p.Category, SUM(od.Quantity * od.Price) AS TotalRevenue
FROM OrderDetails od
JOIN Products p ON od.ProductID = p.ProductID
GROUP BY p.Category
ORDER BY TotalRevenue DESC;


