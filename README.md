# Caso de Optimización: Modelo de programación lineal

## Contexto

Este proyecto resuelve un problema de optimización estocástica, abordado desde una perspectiva determinística, en donde una empresa de productos químicos tiene que decidir cómo distribuir su producción entre dos plantas, tres estanques de almacenamiento y satisfacer las demandas de tres clientes. Las decisiones deben tomarse en dos etapas: una primera donde se decide la cantidad a producir y almacenar en los estanques sin conocer la demanda de los clientes, y una segunda etapa donde se ajusta la distribución según las demandas reales de los clientes. El objetivo es maximizar las utilidades obtenidas por la venta de los productos.

## Código

El código completo está disponible en el archivo [**CasoDeOptimizacion.ipynb**](code/CasoDeOptimizacion.ipynb).


## Accede al repositorio de forma local

Para clonar este repositorio en tu equipo local, puedes usar el siguiente comando:

```bash
git clone https://github.com/tu_usuario/tu_repositorio.git
```

## Librerías y Requerimientos

Para ejecutar este proyecto, es necesario tener instalada la librería `pulp`, que es utilizada para resolver el modelo de programación lineal. Se puede instalar mediante el siguiente comando:

```bash
pip install pulp
```

## Análisis de Resultados

La solución óptima del modelo muestra un beneficio total de 57,990.00, con la producción concentrada únicamente en la Planta 2, la cual abastece principalmente los Estanques 2 y 3. Los flujos entre las plantas y los tanques se ajustan de acuerdo con las demandas de los clientes en cada escenario, optimizando así los recursos disponibles y maximizando las utilidades.

### Conclusiones:

- **Producción en la Planta 1:** No se produce en la Planta 1, ya que la Planta 2 resulta ser más eficiente en este escenario.
- **Flujos:** El Tanque 2 abastece principalmente al Cliente 1 y el Tanque 3 satisface las demandas del Cliente 3. El Cliente 2 es abastecido desde el Tanque 3 en todos los escenarios.
- **Estocasticidad:** El modelo refleja la incertidumbre en las demandas de los clientes mediante la asignación flexible de los flujos en función de los diferentes escenarios de demanda, lo que permite maximizar el beneficio total mientras se ajustan las distribuciones de los productos de manera eficiente.

La solución óptima asegura una asignación adecuada de los recursos, maximizando las utilidades bajo las condiciones planteadas por el problema estocástico.

