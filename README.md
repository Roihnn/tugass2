#include <iostream>
#include <conio.h>
using namespace std;

main(){
    char nama_siswa[50];
    int keaktifan, tugas, ujian, keaktifan1, tugas1, ujian1,hasil;

  cout << "|==============================================|" <<endl;
	cout << "|            Daftar Nilai Siswa                |" <<endl;
	cout << "|==============================================|" <<endl;	
	cout<<endl;

    cout << "Masukkan Nama siswa : ";
	gets (nama_siswa);
    cout <<"Masukan NIlai Keaktifan     :";
    cin >> keaktifan;
    cout << "Masukkan Nilai Tugas    : ";
	cin >> tugas;
	cout << "Masukkan Nilai Ujian      : ";
	cin >> ujian;

    //proses untuk mendapatkan nilai murni
    keaktifan1 = (keaktifan*20/100);
    tugas1 = (tugas*30/100);
    ujian1 = (ujian*50/100);

    cout<<"nilai keaktifan:"<<keaktifan1<<endl ;
    cout<<"nilai tugas    :"<<tugas1<<endl;
    cout<<"nilai ujian    :"<<ujian1<<endl;
   
    hasil = (keaktifan1+tugas1+ujian1);

    

    cout<<"Siswa yang bernama "<<nama_siswa<<endl;
    cout<<"Memperoleh nilai akhir sebesar "<<hasil;
}
