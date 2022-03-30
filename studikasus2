#include <iostream>
#include <conio.h>
using namespace std;

class rumahm{
	friend istream& operator>>(istream&, rumahm&);
	friend ostream& operator<<(ostream&, const rumahm&);
		private:
			int menu, jml, harga, total, jarak, akhir, diskon, o;
			string m;
		public:
			void har();
			void potongan();
			void ongkir();
};

ostream& operator<<(ostream& out, const rumahm& m){
	out<<"====== Menu Rumah Makan ======"<<endl;
	out<<"=============================="<<endl;
	out<<"1. Ayam geprek	: Rp. 21.000 "<<endl;
	out<<"2. Ayam goreng	: Rp. 17.000 "<<endl;
	out<<"3. Udang goreng	: Rp. 19.000 "<<endl;
	out<<"4. Cumi goreng	: Rp. 20.000 "<<endl;
	out<<"5. Ayam bakar   : Rp. 25.000 "<<endl;
	out<<"=============================="<<endl;
}

istream& operator>>(istream& in, rumahm& y){
	cout<<"Masukkan menu yang dipesan        : ";
	in>>y.menu;
	cout<<"Masukkan jarak antar (km)         : ";
	in>>y.jarak;
}

void rumahm::har(){
	if(menu==1){
		m = "Ayam geprek";
		cout<<"Masukkan jumlah menu yang dipesan : ";
		cin>>jml;
		harga=21000*jml;	
	}
	else if(menu==2){
		m = "Ayam goreng";
		cout<<"Masukkan jumlah menu yang dipesan : ";
		cin>>jml;
		harga=17000*jml;
	}
	else if(menu==3){
		m = "Udang goreng";
		cout<<"Masukkan jumlah menu yang dipesan : ";
		cin>>jml;
		harga=19000*jml;
	}
	else if(menu==4){
		m = "Cumi goreng";
		cout<<"Masukkan jumlah menu yang dipesan : ";
		cin>>jml;
		harga=20000*jml;
	}
	else if(menu==5){
		m = "Ayam Bakar";
		cout<<"Masukkan jumlah menu yang dipesan : ";
		cin>>jml;
		harga=25000*jml;
	}
	else{
		cout<<"Tidak terdaftar";
	}
}

void rumahm::ongkir(){
	if(jarak<=3){
		o = 15000;
		total = harga + o;
	}
	else{
		o = 25000;
		total = harga + o;
	}
}

void rumahm::potongan(){
	if(harga>25000&&harga<50000){
		diskon = 3000;
		akhir = total - diskon;
		cout<<"\n====== RUMAH MAKAN TIF ======"<<endl;
		cout<<"Makanan     : "<<m<<endl;
		cout<<"Jumlah      : "<<jml<<endl;
		cout<<"Jarak antar : "<<jarak<<"km"<<endl;
		cout<<"Harga       : Rp. "<<harga<<endl;
		cout<<"Ongkir      : Rp. "<<o<<endl;
		cout<<"Potongan    : Rp. "<<diskon<<endl;
		cout<<"Total       : Rp. "<<akhir<<endl;
		cout<<"============================="<<endl;
		cout<<"======= TERIMA KASIH ========";
	}
	else if((harga>50000)&&(harga<150000)){
		diskon = (0.15*total)+5000;
		akhir = total - diskon;
		cout<<"\n====== RUMAH MAKAN TIF ======"<<endl;
		cout<<"Makanan     : "<<m<<endl;
		cout<<"Jumlah      : "<<jml<<endl;
		cout<<"Jarak antar : "<<jarak<<"km"<<endl;
		cout<<"Harga       : Rp. "<<harga<<endl;
		cout<<"Ongkir      : Rp. "<<o<<endl;
		cout<<"Potongan    : Rp. "<<diskon<<endl;
		cout<<"Total       : Rp. "<<akhir<<endl;
		cout<<"============================="<<endl;
		cout<<"======= TERIMA KASIH ========";
	}
	else{
		diskon = (0.35*total)+8000;
		akhir = total - diskon;
		cout<<"\n====== RUMAH MAKAN TIF ======"<<endl;
		cout<<"Makanan     : "<<m<<endl;
		cout<<"Jumlah      : "<<jml<<endl;
		cout<<"Jarak antar : "<<jarak<<"km"<<endl;
		cout<<"Harga       : Rp. "<<harga<<endl;
		cout<<"Ongkir      : Rp. "<<o<<endl;
		cout<<"Potongan    : Rp. "<<diskon<<endl;
		cout<<"Total       : Rp. "<<akhir<<endl;
		cout<<"============================="<<endl;
		cout<<"======= TERIMA KASIH ========";
	}
}

int main(){
	rumahm e;
	cout<<e;
	cin>>e;
	e.har();
	e.ongkir();
	e.potongan();
	getch();
}
