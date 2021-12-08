berjalan dari bawa layar ke atas layar
   per karakter
   menggunakan C Compiler
   menggunakan C++ Compiler
   ----------------------------------------- */

// karena ada proses cetak ke layar dan
@@ -35,9 +35,7 @@ int main ()
{

// mendefinisikan kalimat string 60 karakter	
char kalimat[60]="halo selamat datang";

// char potongan;
char kalimat[60]="halo selamat datang - universitas lampung";

// mendefinisikan variabel baris
short int baris;
@@ -55,10 +53,10 @@ short int panjang_kalimat;
// int waktu,waktu2;

// ini kalau di OS Linux
//system("clear"); //clears the screen
system("clear"); //clears the screen

// ini kalau di Windows
system("cls"); //clears the screen
//system("cls"); //clears the screen

cout << "Masukkan suatu kalimat:";
//gets(kalimat);
@@ -81,25 +79,13 @@ for (huruf=0;huruf<panjang_kalimat;huruf++)
 {
   PosisiLayar(kolom,baris+1); //reposition cursor   
   cout << " ";
//   write(1," ",1);

//  sleep(1);

  PosisiLayar(kolom,baris); //reposition cursor   
   cout << kalimat[huruf];

//   write(1,kalimat[huruf],1);


   //  puts(kalimat);

   // untuk membuat jeda
//   for (waktu=0;waktu<=4000;waktu++)
//       for (waktu2=1;waktu2<=4000;waktu2++);

  //sleep(1);

   //delay(1000);
   PosisiLayar(1,1); //reposition cursor   
   getchar();

 }
}
return 0;
}
