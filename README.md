# solar-energy-calculator

# Getting started
**Step 1:**
Head to your terminal and paste the following command **'git clone https://github.com/aqeemabd/solar-energy-calculator.git'**

**Step 2:**
Once you cloned the project, open using your desire code editor ex: **Visual Studio Code**

**Step 3:**
Run **'NPM i'** to install the node modules

**Step 4:**
Copy and paste **'.env.example'** file and rename it to **'.env'**

**Step 5:**
 1. Change the variable inside the **'.env'** file based on your local database credentials setup
 2. Open your local database
 3. Run the SQL below to create 'savings' table inside your database (make sure your **'DB_NAME'** is correct)
    ~~~~sql
    CREATE TABLE IF NOT EXISTS `savings` (
    `ID` int NOT NULL AUTO_INCREMENT,
    `systemSize` float DEFAULT NULL,
    `totalSystemCost` float DEFAULT NULL,
    `targetMonthlyPayment` float DEFAULT NULL,
    `monthlyPayment` float DEFAULT NULL,
    `name` varchar(50) COLLATE utf8mb4_unicode_ci DEFAULT NULL,
    `email` varchar(50) COLLATE utf8mb4_unicode_ci DEFAULT NULL,
    `state` varchar(50) COLLATE utf8mb4_unicode_ci DEFAULT NULL,
    `created_at` timestamp NULL DEFAULT NULL,
    `updated_at` timestamp NULL DEFAULT NULL,
    PRIMARY KEY (`ID`)
    ) ENGINE=InnoDB AUTO_INCREMENT=10 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_unicode_ci;
    ~~~~

Step 6
Run **'NPM start'** to open the webpage.
