-- phpMyAdmin SQL Dump
-- version 4.8.3
-- https://www.phpmyadmin.net/
--
-- Servidor: 127.0.0.1
-- Tiempo de generaciÃ³n: 28-05-2020 a las 13:01:41
-- VersiÃ³n del servidor: 10.1.35-MariaDB
-- VersiÃ³n de PHP: 7.2.9

SET SQL_MODE = "NO_AUTO_VALUE_ON_ZERO";
SET AUTOCOMMIT = 0;
START TRANSACTION;
SET time_zone = "+00:00";


/*!40101 SET @OLD_CHARACTER_SET_CLIENT=@@CHARACTER_SET_CLIENT */;
/*!40101 SET @OLD_CHARACTER_SET_RESULTS=@@CHARACTER_SET_RESULTS */;
/*!40101 SET @OLD_COLLATION_CONNECTION=@@COLLATION_CONNECTION */;
/*!40101 SET NAMES utf8mb4 */;

--
-- Base de datos: `bd_blog`
--

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `blog`
--

CREATE TABLE `blog` (
  `id` int(10) NOT NULL,
  `fecha` timestamp NOT NULL DEFAULT CURRENT_TIMESTAMP,
  `titulo` varchar(600) NOT NULL,
  `contenido` varchar(6000) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;

--
-- Volcado de datos para la tabla `blog`
--

INSERT INTO `blog` (`id`, `fecha`, `titulo`, `contenido`) VALUES
(1, '2020-05-25 22:15:27', 'MODELO COMPUTACIONAL QUE PUSO AL MUNDO EN CUARENTENA', 'Esta reflexiÃ³n solo deja en claro un hecho que parece inevitable: hasta que no se produzca una vacuna o por lo menos un tratamiento efectivo al covid 19, es altamente probable que la economÃ­a global '),
(6, '2020-05-28 10:40:30', '632 casos positivos de covid-19 en un dia, Bolivia alcanza nuevo record inesperado', 'Nuevo record de contagios en Bolivia. Este miercoles 27 de mayo, se registraron 632 nuevos casos de covid-19 en seis departamentos, con Santa Cruz al frente. La cifra total de infectados llega a 7.768.    El Ministerio de Salud informe que en Santa Cruz hay 478 nuevos pacientes de coronavirus, seguido de Beni, con 113; Cochabamba, con 31, y La Paz, con 5. Se confirmaron los tres nuevos positivos en Chuquisaca, y Oruro tambien sumÃƒÂ³ 2.  ');

-- --------------------------------------------------------

--
-- Estructura de tabla para la tabla `login`
--

CREATE TABLE `login` (
  `id` int(11) UNSIGNED NOT NULL,
  `usuario` varchar(50) NOT NULL,
  `pass` varchar(100) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;

--
-- Volcado de datos para la tabla `login`
--

INSERT INTO `login` (`id`, `usuario`, `pass`) VALUES
(1, 'rodrigo', '6777980'),
(2, 'admin', 'admin');

--
-- Ãndices para tablas volcadas
--

--
-- Indices de la tabla `blog`
--
ALTER TABLE `blog`
  ADD PRIMARY KEY (`id`);

--
-- Indices de la tabla `login`
--
ALTER TABLE `login`
  ADD PRIMARY KEY (`id`);

--
-- AUTO_INCREMENT de las tablas volcadas
--

--
-- AUTO_INCREMENT de la tabla `blog`
--
ALTER TABLE `blog`
  MODIFY `id` int(10) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=7;

--
-- AUTO_INCREMENT de la tabla `login`
--
ALTER TABLE `login`
  MODIFY `id` int(11) UNSIGNED NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=3;
COMMIT;

/*!40101 SET CHARACTER_SET_CLIENT=@OLD_CHARACTER_SET_CLIENT */;
/*!40101 SET CHARACTER_SET_RESULTS=@OLD_CHARACTER_SET_RESULTS */;
/*!40101 SET COLLATION_CONNECTION=@OLD_COLLATION_CONNECTION */;

![login](https://user-images.githubusercontent.com/66080714/83179842-dbfd6c00-a122-11ea-85de-eaaf59e0f417.png)


![Captura de pantalla (7)](https://user-images.githubusercontent.com/66080714/83189586-7cf32380-a131-11ea-9181-4fc008ecd47a.png)



![Captura de pantalla (8)](https://user-images.githubusercontent.com/66080714/83189760-baf04780-a131-11ea-8cea-915a1a65410a.png)
