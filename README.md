# dron-follow-a-line-in-real-time


# English Version

The black line is on the wall (vertical). The drone must fly parallel to the wall and move along the track, maintaining distance and orientation.  

Vision pipeline: capture → exposure correction → ROI clipping → adaptive or threshold binarization → morphological cleaning → contour/center and approximate straight line extraction → lateral and angle error calculation → controller.

# Versión en Español
La línea negra está en la pared (vertical). El dron debe volar paralelo a la pared y desplazarse a lo largo de la pista manteniendo distancia y orientación.

Usamos cámara monocular montada en el dron (orientada hacia la pared), un sensor de distancia (LiDAR TOF o rangefinder) para mantener distancia constante y un bucle de control PID que combine la información de visión y distancia para generar comandos (lateral / vertical / yaw / avance).

Pipeline de visión: captura → corrección de exposición → recorte de ROI → binarización adaptativa o por umbral → limpieza morfológica → extracción del contorno/centro y recta aproximada → cálculo de error lateral y angulo → controlador.
