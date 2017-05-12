LAB 3
LINK: https://www.overleaf.com/8947188gzyhjdrbsykb#/32053152/
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
{ \huge \bfseries Laboratorio Nº3}\\[0.4cm]
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

2\ ACTIVIDAD ----------------------------------------------------------------- PÁG 2-13\\
2.1 DIRECCIÓN MAC DESTINO FF:FF:FF:FF:FF:FF  ------------- PÁG 2-7\\
2.2 DIRECCIÓN MAC DESTINO OTRO EQUIPO ---------------- PÁG 8-12\\
2.3 DIRECCIÓN MAC DESTINO EQUIPO FUERA DE RED ----- PÁG 13\\
3\ CUESTIONARIO -------------------------------------------------------------- PÁG 14\\
3.1 DIRECCIÓN MAC DESTINO FF:FF:FF:FF:FF:FF --------------- PÁG 14\\
3.2 DIRECCIÓN MAC DESTINO OTRO EQUIPO -------------------- PÁG 14\\
3.3 DIRECCIÓN MAC DESTINO EQUIPO FUERA DE RED ----- PÁG 14\\
4\ CONCLUSIÓN ----------------------------------------------------------------- PÁG 15\\
5\ BIBLIOGRAFÍA --------------------------------------------------------------- PÁG 15\\[2CM]
IMAGEN 1: Wireshark del PC fuente: Mensaje enviado "Hola" ----- PÁG 2\\
IMAGEN 2: Wireshark del PC fuente; Frame ----------------------------- PÁG 3\\
IMAGEN 3: Wireshark del PC fuente; Ethernet II ---------------------- PÁG 4\\
IMAGEN 4: Wireshark del PC fuente; Internet Protocol --------------- PÁG 5\\
IMAGEN 5: Wireshark del PC fuente; Internet Control ---------------- PÁG 6\\
IMAGEN 6: Wireshark del PC receptor ------------------------------------ PÁG 7\\
IMAGEN 7: Wireshark del PC destino: Mensaje recibido "Hola" --- PÁG 8\\
IMAGEN 8: Wireshark del PC destino; Frame ---------------------------- PÁG 9\\
IMAGEN 9: Wireshark del PC destino; Linux cooked capture ------- PÁG 10\\
IMAGEN 10: Wireshark del PC destino; Internet Protocol ----------- PÁG 11\\
IMAGEN 11: Wireshark del PC destino; Internet Control ------------ PÁG 12\\
IMAGEN 12: Wireshark del PC fuente ------------------------------------- PÁG 13\\



\section{ACTIVIDAD}

\subsection{Dirección MAC de destino FF:FF:FF:FF:FF:FF}

\includegraphics{ff.png}
(Imagen 1: Wireshark del PC fuente: Mensaje enviado "Hola")\\
\includegraphics{fff.png}
(Imagen 2: Wireshark del PC fuente; Frame)\\[1cm]
\includegraphics{ffff.png}
(Imagen 3: Wireshark del PC fuente; Ethernet II)\\[1cm]
\includegraphics{fffff.png}
(Imagen 4: Wireshark del PC fuente; Internet Protocol)\\[1cm]
\includegraphics{ffffff.png}
(Imagen 5: Wireshark del PC fuente; Internet Control Message Protocol)\\[1cm]
\includegraphics{fr.png}
(Imagen 6: Wireshark del PC receptor: al enviar al broadcast el mensaje lo reciben todos los PC de la red)\\[1cm]

\subsection{Dirección MAC de destino otro equipo}

\includegraphics{g.png}
(Imagen 7: Wireshark del PC destino: Mensaje recibido "Hola")\\[1cm]
\includegraphics{gg.png}
(Imagen 8: Wireshark del PC destino; Frame)\\[1cm]
\includegraphics{ggg.png}
(Imagen 9: Wireshark del PC destino; Linux cooked capture)\\[1cm]
\includegraphics{gggg.png}
(Imagen 10: Wireshark del PC destino; Internet Protocol)\\[1cm]
\includegraphics{ggggg.png}
(Imagen 11: Wireshark del PC destino; Internet Control Message Protocol y Monitoring Ethernet Trailer)\\[1cm]

\subsection{Dirección MAC de destino otro equipo fuera de la red}

\includegraphics{h.png}\\
(Imagen 12: Wireshark del PC fuente)\\[9cm]

\section{CUESTIONARIO}

\subsection{¿Qué sucede cuando se envía un paquete a la dirección FF:FF:FF:FF:FF:FF? ¿Quiénes lo reciben? ¿Porqué?}
  Al ser FF:FF:FF:FF:FF:FF la MAC broadcast el mensaje llega a cada computador de la red,ya que el switch busca la dirección en todos los PC conectados a la red, es la dirección de difusión de la red.  
\subsection{¿Qué pasa cuando se envía un paquete a la MAC de otro equipo? ¿Quiénes lo pueden recibir? ¿Porqué?}
   
  Cuando se envía un paquete a una MAC, el computador que posee aquella MAC , podrá acceder a los datos del paquete. Para esto el PC envía el paquete al switch, este verifica entre los computadores de la red la MAC de destino, luego la envía a este.

\subsection{¿Qué sucede si se envía un paquete a una MAC que no corresponda a ningún equipo de la red? ¿Quiénes lo pueden recepcionar? ¿Por qué?}

  Cuando se envía un paquete a una MAC de un PC no conectado a la red, no es recibido por ninguno, ya que el PC emisor envía el paquete al switch y este al no reconocer la MAC anula la operación.\\[9cm]

\section{CONCLUSIÓN}
Este laboratorio nos ayudó a comprender la utilización del software Scapy, el cual utilizamos para crear paquetes dentro de la red, y conocimos sus diferentes efectos dependiendo de la MAC de destino, esto nos sirvió para lograr comunicar computadores dentro de una misma red, enviando mensajes y comprender la utilidad de los protocolos del proceso, ademas logramos entender el software Wireshark, el cual nos ayudo a visualizar en pantalla la información enviada y recibida, con información detallada de esta.


\section{BIBLIOGRAFÍA}
Python\\
Wireshark\\
Scapy\\
          

\end{document}
