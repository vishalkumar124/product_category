# product_category
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
--
-- Host: 127.0.0.1:3307
-- Generation Time: May 05, 2023 at 08:27 AM
-- Server version: 10.4.27-MariaDB
-- PHP Version: 8.2.0

SET SQL_MODE = "NO_AUTO_VALUE_ON_ZERO";
START TRANSACTION;
SET time_zone = "+00:00";


/*!40101 SET @OLD_CHARACTER_SET_CLIENT=@@CHARACTER_SET_CLIENT */;
/*!40101 SET @OLD_CHARACTER_SET_RESULTS=@@CHARACTER_SET_RESULTS */;
/*!40101 SET @OLD_COLLATION_CONNECTION=@@COLLATION_CONNECTION */;
/*!40101 SET NAMES utf8mb4 */;

--
-- Database: `project_cat`
--

-- --------------------------------------------------------

--
-- Table structure for table `cat_table`
--

CREATE TABLE `cat_table` (
  `id` int(10) NOT NULL,
  `parent_id` int(10) NOT NULL,
  `product` varchar(30) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
-- Dumping data for table `cat_table`
--

INSERT INTO `cat_table` (`id`, `parent_id`, `product`) VALUES
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

--
-- Indexes for dumped tables
--

--
-- Indexes for table `cat_table`
--
ALTER TABLE `cat_table`
  ADD PRIMARY KEY (`id`);

--
-- AUTO_INCREMENT for dumped tables
--

--
-- AUTO_INCREMENT for table `cat_table`
--
ALTER TABLE `cat_table`
  MODIFY `id` int(10) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=24;
COMMIT;

/*!40101 SET CHARACTER_SET_CLIENT=@OLD_CHARACTER_SET_CLIENT */;
/*!40101 SET CHARACTER_SET_RESULTS=@OLD_CHARACTER_SET_RESULTS */;
/*!40101 SET COLLATION_CONNECTION=@OLD_COLLATION_CONNECTION */;

