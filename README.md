# Análisis Estadístico del Rendimiento en la temporada regular 2023 de la NBA

* Oscar Miguel Ortega Lozano - 2220528
* Juan David Toloza Parada - 2221067
* Laura Camila Diaz-Delgado - 2220100

![Descripción de la imagen](https://raw.githubusercontent.com/LauraCD2/estadisticos/main/Images/istockphoto-1480105317-612x612.jpg)

El baloncesto, como uno de los deportes más dinámicos y analíticos del mundo, genera una vasta cantidad de datos que permiten evaluar el rendimiento individual y colectivo de los jugadores. En este proyecto, nos enfocamos en el análisis estadístico de las métricas clave de los jugadores de la NBA durante la temporada regular de 2023, utilizando el dataset 2023_nba_player_stats.csv, el cual, contiene estadísticas detalladas de 539 jugadores, con 30 variables que abarcan aspectos cuantitativos y cualitativos del rendimiento individual. A continuación, se describe su estructura y variables clave:

### Variables del Dataset (NBA 2023)

#### 1. Datos Demográficos
| **Variable** | **Descripción**                          | **Tipo**   |
|--------------|------------------------------------------|-------------|
| `PName`      | Nombre del jugador                       | `object`    |
| `POS`        | Posición (PG, SG, SF, PF, C)             | `object`    |
| `Team`       | Abreviatura del equipo                   | `object`    |
| `Age`        | Edad del jugador                         | `int64`     |

---

#### 2. Rendimiento General
| **Variable** | **Descripción**                          | **Tipo**   |
|--------------|------------------------------------------|-------------|
| `GP`         | Partidos jugados                         | `int64`     |
| `W`          | Partidos ganados                         | `int64`     |
| `L`          | Partidos perdidos                        | `int64`     |
| `Min`        | Minutos totales jugados                  | `float64`   |

---

#### 3. Estadísticas Ofensivas
| **Variable** | **Descripción**                          | **Tipo**   |
|--------------|------------------------------------------|-------------|
| `PTS`        | Puntos totales anotados                  | `int64`     |
| `FGM`        | Tiros de campo convertidos               | `int64`     |
| `FGA`        | Tiros de campo intentados                | `int64`     |
| `FG%`        | Porcentaje de tiros de campo             | `float64`   |
| `3PM`        | Triples convertidos                      | `int64`     |
| `3PA`        | Triples intentados                       | `int64`     |
| `3P%`        | Porcentaje de triples                    | `float64`   |
| `FTM`        | Tiros libres convertidos                 | `int64`     |
| `FTA`        | Tiros libres intentados                  | `int64`     |
| `FT%`        | Porcentaje de tiros libres               | `float64`   |

---

#### 4. Estadísticas Defensivas
| **Variable** | **Descripción**                          | **Tipo**   |
|--------------|------------------------------------------|-------------|
| `OREB`       | Rebotes ofensivos                        | `int64`     |
| `DREB`       | Rebotes defensivos                       | `int64`     |
| `REB`        | Rebotes totales                          | `int64`     |
| `STL`        | Robos de balón                           | `int64`     |
| `BLK`        | Bloqueos                                 | `int64`     |
| `PF`         | Faltas personales                        | `int64`     |
| `+/-`        | Diferencial de puntos del equipo         | `int64`     |

---

#### 5. Métricas Avanzadas
| **Variable** | **Descripción**                          | **Tipo**   |
|--------------|------------------------------------------|-------------|
| `AST`        | Asistencias totales                      | `int64`     |
| `TOV`        | Pérdidas de balón                        | `int64`     |
| `FP`         | Puntos de fantasía NBA                   | `int64`     |
| `DD2`        | Número de dobles-dobles                  | `int64`     |
| `TD3`        | Número de triples-dobles                 | `int64`     |

---

**Notas**:  
- **Dataset**: [2023 NBA Player Stats](https://www.kaggle.com/datasets/amirhosseinmirzaie/nba-players-stats2023-season)  
- **Registros**: 539 jugadores  
- **Limpieza**:  
  - Relleno de valores vacíos en `POS` con "PF"  
  - Normalización de nombres de columnas  
