\# product\_category

Step 1: Install nodeJs package and Init application

node -v

Step 2: Create a directory and init application

npm init

Install required packages using NPM

Express,body-parser,mysql,ejs

nodemon: Optional package and Installed globally. It helps us to listen for modifications to files and automatically restart the app server.

npm intall <pakage name>

npm install --save express mysql body-parser ejs

npm install -g nodemon

-- phpMyAdmin SQL Dump

-- version 5.2.0

-- https://www.phpmyadmin.net/

\--

-- Host: 127.0.0.1:3307

-- Generation Time: May 05, 2023 at 08:27 AM

-- Server version: 10.4.27-MariaDB

-- PHP Version: 8.2.0

SET SQL\_MODE = "NO\_AUTO\_VALUE\_ON\_ZERO";

START TRANSACTION;

SET time\_zone = "+00:00";


/\*!40101 SET @OLD\_CHARACTER\_SET\_CLIENT=@@CHARACTER\_SET\_CLIENT \*/;

/\*!40101 SET @OLD\_CHARACTER\_SET\_RESULTS=@@CHARACTER\_SET\_RESULTS \*/;

/\*!40101 SET @OLD\_COLLATION\_CONNECTION=@@COLLATION\_CONNECTION \*/;

/\*!40101 SET NAMES utf8mb4 \*/;

\--

-- Database: `project\_cat`

\--

\-- --------------------------------------------------------

\--

-- Table structure for table `cat\_table`

\--

CREATE TABLE `cat\_table` (

`id` int(10) NOT NULL,

`parent\_id` int(10) NOT NULL,

`product` varchar(30) NOT NULL

) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4\_general\_ci;

\--

-- Dumping data for table `cat\_table`

\--

INSERT INTO `cat\_table` (`id`, `parent\_id`, `product`) VALUES

(2, 0, 'Vegetable'),

(5, 8, 'Apple'),

(8, 0, 'Fruits'),

(9, 2, 'potato'),

(10, 0, 'Grocery'),

(11, 0, 'Snacks'),

(12, 0, 'ColdDrinks'),

(13, 2, 'Tomato'),

(14, 2, 'Carrot'),

(15, 2, 'Onions'),

(16, 8, 'Mango'),

(17, 11, 'Lays'),

(18, 12, 'COke'),

(19, 8, 'Lichi'),

(20, 11, 'Kurkure'),

(21, 12, 'Pepsi'),

(22, 10, 'Rice'),

(23, 10, 'Aata');

\--

-- Indexes for dumped tables

\--

\--

-- Indexes for table `cat\_table`

\--

ALTER TABLE `cat\_table`

ADD PRIMARY KEY (`id`);

\--

-- AUTO\_INCREMENT for dumped tables

\--

\--

-- AUTO\_INCREMENT for table `cat\_table`

\--

ALTER TABLE `cat\_table`

MODIFY `id` int(10) NOT NULL AUTO\_INCREMENT, AUTO\_INCREMENT=24;

COMMIT;

/\*!40101 SET CHARACTER\_SET\_CLIENT=@OLD\_CHARACTER\_SET\_CLIENT \*/;

/\*!40101 SET CHARACTER\_SET\_RESULTS=@OLD\_CHARACTER\_SET\_RESULTS \*/;

/\*!40101 SET COLLATION\_CONNECTION=@OLD\_COLLATION\_CONNECTION \*/;

