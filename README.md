# TranspuestaDeunaMatriz
#include <iostream>
#include <string.h>
#include <stdlib.h>

using namespace std;

int main(){
	int numeros[100][100],filas,columnas;
  int matriz2[100][100],fila,columna;
  int OP;


  printf("\nA cuantas matrices desea sacarle la transpuesta a 1 o 2?");
 printf("\n\nDigite su opcion..");
 scanf("%d",&OP);

switch(OP){//Para las opciones
  case 1:

  cout<<"\n\nDigite el numero de filas: "; cin>>filas;
	cout<<"Digite el numero de columnas: "; cin>>columnas;

  cout<<"\nLlene la matriz 1:\n\n";
	for(int i=0;i<filas;i++){
		for(int j=0;j<columnas;j++){
			cout<<"Digite un numero ["<<i<<"]["<<j<<"]: ";
			cin>>numeros[i][j];
      }
    }
  cout<<"\nMostrando matriz N°1\n\n";
	
	for(int i=0;i<filas;i++){
    cout<<"[ ";
		for(int j=0;j<columnas;j++){
			cout<<numeros[i][j]<<" ";
		}
    cout<<"]";
  	cout<<"\n";
    }
  cout<<"\nTranspuesta Matriz N°1\n\n";
	for(int i=0;i<filas;i++){
    cout<<"[ ";
		for(int j=0;j<columnas;j++){
		cout<<numeros[j][i]<<" ";
		}
    cout<<"]";
		cout<<"\n";
	}
break;
  
  case 2:
  
	cout<<"\n\nDigite el numero de filas: "; cin>>filas;
	cout<<"Digite el numero de columnas: "; cin>>columnas;

  cout<<"\n\nDigite el numero de filas de la segunda matriz: "; cin>>fila;
	cout<<"Digite el numero de columnas de la segunda matriz: "; cin>>columna;
	
	//Rellenando la matriz	
  cout<<"\nLlene la matriz N°1\n\n";
	for(int i=0;i<filas;i++){
		for(int j=0;j<columnas;j++){
			cout<<"Digite un numero ["<<i<<"]["<<j<<"]: ";
			cin>>numeros[i][j];
		}
    }
   cout<<"\nLlene la matriz N°2\n\n";
    for(int i=0;i<fila;i++){
		for(int j=0;j<columna;j++){
			cout<<"Digite un numero ["<<i<<"]["<<j<<"]: ";
			cin>>matriz2[i][j];
		}
	} 
   system("clear");
  
	cout<<"\nMostrando matriz N°1\n\n";
	
	for(int i=0;i<filas;i++){
    cout<<"[ ";
		for(int j=0;j<columnas;j++){
			cout<<numeros[i][j]<<" ";
		}
    cout<<"]";
  	cout<<"\n";
    }
	
    cout<<"\nMostrando matriz N°2\n\n";
   
    for(int n=0;n<fila;n++){
      cout<<"[ ";
		for(int m=0;m<columna;m++){
			cout<<matriz2[n][m]<<" ";
      
      
		}
    cout<<"]";
		cout<<"\n";
	}
//funcion de la transpuesta 
  cout<<"\nTranspuesta Matriz N°1\n\n";
	for(int i=0;i<filas;i++){
    cout<<"[ ";
		for(int j=0;j<columnas;j++){
		cout<<numeros[j][i]<<" ";
		}
    cout<<"]";
		cout<<"\n";
	}
  cout<<"\nTranspuesta Matriz N°2\n\n";
	for(int i=0;i<fila;i++){
    cout<<"[ ";
		for(int j=0;j<columna;j++){
			cout<<matriz2[j][i]<<" ";
		}
    cout<<"]";
		cout<<"\n";
	}
	
	
	
	return 0;
break;}
  }
