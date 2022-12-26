# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemograman
<br> Nama		: Angga Alhusaini Youztima
<br>NIM		:	1227050021
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum

## Source Code
#include <iostream>
#include <conio.h>
using namespace std;

void garis(){
	cout<<"--------------------------------------"<<endl;
}

main(){
	int br,kl,x,y,z;
	cout<<"Inputkan berapa banyak baris yang diinginkan untuk array : ";
	cin>>br;
	cout<<"Inputkan berapa banyak kolom yang diinginkan untuk array : ";
	cin>>kl;
	garis();
	
	int array[br][kl],tukar[br][kl]; 
    cout<<"Berikan nilai pada array!"<<endl;
    garis();
    for (x=1; x<=br; x++){
    	for(y=1; y<=kl; y++){
    		cout<<"Array baris ke-"<<x<<" kolom ke-"<<y<<": \n";
    		cin>>array[x][y];
    		garis();
		}
	}
	
	cout<<"Array sebelum ditukar kolom dan barisnya : \n";
	garis();
	for(x=1;x<=br;x++){
		for(y=1;y<=kl;y++){
			cout<<"  "<<array[x][y];
		}
		cout<<endl;
	}
	garis();
	
	cout<<"Array sesudah ditukar kolom dan barisnya : \n";
	garis();
	for(x=1;x<=kl;x++){
		for(y=1;y<=br;y++){
			cout<<"  "<<array[y][x];
		}
		cout<<endl;
	}
	garis();
}

#include <iostream>

using namespace std;

void garis(){
	cout<<"---------------------"<<endl;
}

main(){
	int br,kl,x,y,z,i;
	cout<<"Inputkan berapa banyak baris yang diinginkan untuk array : ";
	baris:
	cin>>br;
	if(br>20){
		cout<<"Baris anda terlalu banyak!!"<<endl;
		goto baris;
	}
	cout<<"Inputkan berapa banyak kolom yang diinginkan untuk array : ";
	cin>>kl;
	if(kl>20){
		cout<<"Kolom anda terlalu banyak!!"<<endl;
		goto baris;
	}
	garis();
	
	int array[br][kl];
    cout<<"Berikan nilai pada array!"<<endl;
    garis();
    for (x=1; x<=br; x++){
    	for(y=1; y<=kl; y++){
    		cout<<"Array baris ke-"<<x<<" kolom ke-"<<y<<": \n";
    		cin>>array[x][y];
		}
		garis();
	}	
	
	cout<<"Array awal : \n";
	garis();
	for(x=1;x<=br;x++){
		for(y=1;y<=kl;y++){
				cout<<" "<<array[x][y];
		}
		cout<<endl;
	}
	garis();
	
	int hasil[x * y];
	int kali=0;
	for(x=1;x<=br;x++){
		for(y=1;y<=kl;y++){
			if(array[x][y]%3 != 0 && array[x][y]%5 != 0 && array[x][y]%7 != 0){
				hasil[kali]=array[x][y];
				kali++;
			}
		}
	}
	
	cout<<"\nHasilnya yang tidak bisa dibagi 3, 5, 7 adalah : ";
	for(int i = 0; i < kali; i++){
		cout<<hasil[i];
		if(i < kali -1){
			cout<<", ";
		}else{
			cout<<".";
		}
	}
}
## Output
  ![Screenshot (137)](https://user-images.githubusercontent.com/121450649/209570801-2b49d7a6-8d9b-440d-ac66-c0b36f34c475.png)
  ![Screenshot (138)](https://user-images.githubusercontent.com/121450649/209570818-5308eea9-71c9-492d-8e9c-a907b84087d5.png)

