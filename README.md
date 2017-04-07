en este archivo va el pdf y el link del archivo fuente en overleaf.

\documentclass[12pt]{article}
\usepackage[english]{babel}
\usepackage[utf8x]{inputenc}
\usepackage{amsmath}
\usepackage{graphicx}
\usepackage[colorinlistoftodos]{todonotes}

\begin{document}

\begin{titlepage}

\newcommand{\HRule}{\rule{\linewidth}{0.5mm}}

\center 

\textsc{\LARGE Universidad Diego Portales}\\[1cm]
\textsc{\Large Ingeniería civil informática y telecomunicaciones}\\[0.5cm]

\HRule \\[0.4cm]
{ \huge \bfseries Laboratorio Nº1}\\[0.4cm]
{ \huge \bfseries Redes de Datos}\\[0.4cm]
\HRule \\[1cm]
 

\begin{minipage}{0.4\textwidth}
\begin{flushleft} \large
\emph{Author:}\\
Sebastian \textsc{Diaz}\\
\textsc{Daniel Utreras}
\end{flushleft}
\end{minipage}
~
\begin{minipage}{0.4\textwidth}
\begin{flushright} \large
\emph{Ayudante:} \\
Alexis \textsc{Inzunza} 
\emph{Profesor:} \\
José \textsc{Pérez}
\end{flushright}
\end{minipage}\\[1cm]

\includegraphics{seminarios-de-fisica-de-la-universidad-diego-portales.jpg}\\[1cm] 
{\large \today}\\[2cm]
 

\vfill

\end{titlepage}
\section{ÍNDICE}

2\ ACTIVIDAD:IDENTIFICACIÓN DE ELEMENTO DE RED ----- PÁG 2\\
2.1 EQUIPOS CONECTADOS A LA RED -------------------------------- PÁG 2\\
2.2 IDENTIFICAR SWITCH O SWITCHERS --------------------------- PÁG 2\\
2.3 HARDWARE DE RED ----------------------------------------------------- PÁG 3\\
2.4 TIPO DE CABLEADO ----------------------------------------------------- PÁG 3\\
2.5 IDENTIFICAR PATCH PANEL ----------------------------------------- PÁG 3\\
3 ACTIVIDAD:IDENTIFICACIÓN DE DISPOSITIVOS -------------- PÁG 4\\
4 ACTIVIDAD:DIAGRAMA DE RED -------------------------------------- PÁG 5\\
5 CONCLUSIÓN ------------------------------------------------------------------ PÁG 6\\
6 BIBLIOGRAFÍA ---------------------------------------------------------------- PÁG 6\\[3CM]
IMAGEN 1: PATCH PANEL Y SWITCHER ----------------------------- PÁG 2\\
IMAGEN 2: SWITCH ----------------------------------------------------------- PÁG 2\\
IMAGEN 3: CABLE UTP CAT 5 -------------------------------------------- PÁG 3\\
IMAGEN 4: PATCH PANEL -------------------------------------------------- PÁG 3\\
IMAGEN 5: TERMINAL PC -------------------------------------------------- PÁG 4\\
IMAGEN 6: DIAGRAMA DE RED ------------------------------------------ PÁG 5\\[5CM]



\section{ACTIVIDAD: IDENTIFICACIÓN DE ELEMENTOS DE RED}
\subsection{Equipos conectados a la red}
Dentro de la red se pueden identificar:

19 Computadores de escritorio 

Un Switch

Un Patch Panel

\includegraphics{Telroom.jpg}\\
(Imagen 1: Patch panel y switcher)
\subsection{Identificar switch o switchers}
La red posee un switch \\

\includegraphics{Switch.jpg}\\
(Imagen 2: Switch, dispositivo de abajo)\\[1cm]


\subsection{Hardware de red}

Switch /WS – CATALYST 2960 – 24 TT – L\\
Patch Panel Siemon 5e HD Series 24 entrada\\

\subsection{Tipo de cableado}

Cable UTP categoría 5\\

\includegraphics{UTP5ca.jpg}\\
(Imagen 3: Cable UTP Categoría 5)


\subsection{Identificar patch panel}

La red posee un patch panel\\

\includegraphics{Pathpanel.jpg}\\
(Imagen 4: Patch panel, dispositivo de arriba)

\section{ACTIVIDAD: IDENTIFICACIÓN DE DISPOSITIVOS}


\includegraphics{IN1.png}

(Imagen 5: Terminal PC)\\

IP:172.16.32.109

Mask: 255.255.255.0

\section{ACTIVIDAD: DIAGRAMA DE RED}


\includegraphics{diagrama4.png}\\
(Imagen 6:diagrama de red hecho en DRAW.IO)\\[5cm]
\section{CONCLUSIÓN}

\ En nuestro caso particular como los integrantes de este grupo (Sebastián y Daniel)  previo al ramo “redes de datos” poseíamos un nulo conocimiento de redes y cableado estructurado, considerando este trabajo como una oportunidad para introducirse en el mundo de redes de una forma más visual. El observar y analizar el laboratorio de informática de la universidad nos ayudo a percibir de mejor manera las divisiones y equipos que componen el hardware de red, y además la creación del diagrama fue una manera más didáctica de entender la lógica del cableado, encontrando la aplicación draw.io (junto a las demás aplicaciones de dibujo computacional)  una buena herramienta para el mejor entendimiento de la materia.\\
\section{BIBLIOGRAFÍA}

-www.draw.io/  pagina para crear diagramas.\\
-Wikipedia: rj45.\\           
-Wikipedia: cableado estructurado.\\           
-Wikipedia:caja de conexión.\\
-portal.udp.cl/irj/portal material de redes de datos.\\ 
-Google imagenes: foto de cable utp cat5\\
\end{document}
