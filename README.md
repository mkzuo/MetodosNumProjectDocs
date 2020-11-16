# MetodosNumProjectDocs
Documentation for Visual C# MetodosNumProject

##Ejemplo para crear un Objeto Funcion:

```C#
// Archivo "LinealFunc.cs" -> dentro de la carpeta "FChartFuncs"

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace MetodosNumProject.FChartFunctions
{
    internal class LinealFunc : FChartFunc // Debe extender de FChartFunc
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
