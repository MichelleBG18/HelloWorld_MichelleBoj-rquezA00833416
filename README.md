## HelloWorld_MichelleBojorquezA00833416
## Luis Padrón A01571607
# Michelle Bojórquez Gómez
## Laboratorio para explicar branch, commits, pull-request, merge, markdown

**bold text**
**ITC**

*italicized text*
*TC1033.2*

1. GitHub
2. Tec21
3. Fin semestre

- GitHub
- Tec21
- Fin semestre

`
//Michelle Bojórquez Gómez / A00833416
#include <iostream>
#include "Reloj.h"
using namespace std;

//Funcion menu
int menu(){
	int opcion;

	cout << "    Menu" <<
	"\n1. setHora" <<
	"\n2. setMinutos" <<
	"\n3. getHora" <<
	"\n4. getMinutos" <<
	"\n5. muestra" <<
	"\n6. incrementaMinutos" <<
	"\n7. Salir" << endl;

	cout << "Ingrese el numero de la funcion que desea utilizar: ";
	cin >> opcion;

	return opcion;
}

int main() {
	//Generar objeto "hora"
	Reloj hora;

	//Declarar variables
	int _hr = 0, _minu = 0, opcion;

	//Deplegar menu
	do{
		opcion = menu();

		switch(opcion){

			case 1:
				cout << "Ingrese la hora: ";
				cin >> _hr;
				hora.setHora(_hr);
				break;

			case 2:
				cout << "Ingrese los minutos: ";
				cin >> _minu;
				hora.setMinutos(_minu);
				break;

			case 3:
				hora.getHora();
				break;

			case 4:
				hora.getMinutos();
				break;

			case 5:
				hora.muestra();
				break;

			case 6:
				hora.incrementaMinutos();
				break;

			case 7:
				cout << "Bye" << endl;
				break;

			default:
				cout << "Input no valido" << endl;
				break;

		}
	} while(opcion != 7);

	return 0;
}
`



