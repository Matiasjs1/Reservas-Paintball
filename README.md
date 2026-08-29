# 🎯 Reservas de campo de Paintball

Sistema web de **reservas online de campos de paintball** en tiempo real. Los jugadores se registran, eligen campo, fecha y horario, y pagan su partida online. El sistema **previene reservas dobles** y permite ver y administrar las reservas propias.

🌐 **Probar:** [reservas-paintball.free.nf](http://reservas-paintball.free.nf/)

Proyecto real para el campo **Urban Paintball Extremo**.

---

## ✅ Funcionalidades

- **Registro e inicio de sesión** de usuarios.
- **Reserva online:** elegís campo, fecha, hora y duración de la partida.
- **Prevención de reservas dobles:** si un campo ya está reservado en ese horario, se rechaza la solapada.
- **3 campos de tiro** con tarifas por hora.
- **Ver y borrar tus reservas.**
- Sito responsivo con estilo propio.

### Campos y tarifas

| Campo | Tarifa |
|-------|--------|
| Estándar | $10.000 / hora |
| Grande | $20.000 / hora |
| Grandioso | $30.000 / hora |

---

## 🏗️ Stack

- **Backend:** PHP (con `mysqli` / PDO).
- **Base de datos:** MySQL `reservas_paintball`.
- **Frontend:** HTML, CSS y JavaScript vanilla (sin framework).
- **Servidor:** Apache + MySQL (XAMPP / hosting free).

```
pagina/
├── index.php           # Landing + precios + FAQ + ubicación
├── reserva.php         # Formulario de reserva
├── ver_reservas.php    # Listado de reservas del usuario
├── php/                # Lógica: conexión, guardar, borrar
├── imagenes/           # Fotos de campos y recursos
└── styles.css
base de datos/          # Script SQL
```

---

## 🚀 Setup local

1. Importá `base de datos/base de datos.txt` en MySQL (crea la base `reservas_paintball`).
2. Configurá la conexión en `pagina/php/conexion.php`.
3. Serví `pagina/` con Apache (XAMPP) y andá a `http://localhost/pagina`.

Datos del campo:

- **Ubicación:** Urban Paintball Extremo (Buenos Aires).
- **Horarios:** lunes a domingo, de 9:00 a 00:00.
- **Edad mínima:** 12 años (menores acompañados o con permiso escrito).
- **Incluye:** equipo de protección completo y set inicial de balas.
- **Seguridad:** instructores capacitados y normativas vigentes.

*Ofrecemos diversión y adrenalina desde 2010.*
