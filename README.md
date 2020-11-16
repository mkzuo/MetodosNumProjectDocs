# MetodosNumProjectDocs
Documentation for Visual C# MetodosNumProject

## Ejemplo para crear un Objeto Funcion:

```C#
// Archivo "LinealFunc.cs" -> dentro de la carpeta "FChartFuncs"

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace MetodosNumProject.FChartFunctions
{
    public class LinealFunc : FChartFunc // Debe extender de FChartFunc
    {
        double m;
        double n;

        public LinealFunc(double _m, double _n)
        {
			// Aqui definimos como procesaremos las variables de entrada
            this.m = _m;
            this.n = _n;
        }
		
		
		// Esta funcion se debe definir con el nombre de F y debe retornar un double
        public double F(double x)
        {
			// Devuelve el valor de x evaluado en la funcion, es decir F(x)
            return x * m + n;
        }


    }
}

```

## Como Graficar una funcion

```C#

CuadraticFunc func1 = new CuadraticFunc(2,1,3);

CuadraticFunc func2 = new CuadraticFunc(-2, 1, 3);

this.MAIN_CHART.PlotFunction(func1, -5, 20, "Funcion Cuadratica", 4);

this.MAIN_CHART.PlotFunction(func2, -5, 20, "Funcion Cuadratica 2", 4);
            

this.MAIN_CHART.SetAxisXRange(-20, 20);

this.MAIN_CHART.SetAxisYRange(-50, 200);

```
