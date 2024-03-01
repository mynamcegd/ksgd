# ksgd#include <conio.h>
#include <iostream.h>

class hanghoa
{
	public:
		char mahang[2];
	char tenhang[20];
	char donvitinh[10];
	float dongia, soluong, thanhtien;
	void nhap()#include <conio.h>
#include <iostream.h>

class hanghoa
{
	public:
		char mahang[2];
	char tenhang[20];
	char donvitinh[10];
	float dongia, soluong, thanhtien;
	void nhap()
	{
		cout << "Nhap ma hang : ";
		cin >> mahang;
		cout << "Nhap ten hang : ";
		cin >> tenhang;
		cout << "Nhap don vi tinh : ";
		cin >> donvitinh;
		cout << "Nhap don gia : ";
		cin >> dongia;
		cout << "Nhap so luong : ";
		cin >> soluong;
	}

	void tinhthanhtien()
	{
		thanhtien = dongia * soluong;
	}
};

class hanghoamoi: public hanghoa
{
	public: float dongiavanchuyen, congvanchuyen;
	void nhap()
	{
		hanghoa::nhap();
		cout << "Nhap don gia van chuyen : ";
		cin >> dongiavanchuyen;
	}

	void tinhcongvanchuyen()
	{
		congvanchuyen = soluong * dongiavanchuyen;
	}

	void tinhthanhtien()
	{
		thanhtien = dongia *soluong + congvanchuyen;
	}
};

void main()
{
	hanghoamoi x;
	clrscr();
	x.nhap();
	x.tinhcongvanchuyen();
	x.tinhthanhtien();
	cout << "Thanh tien : " << x.thanhtien;
	getch();
}
	x.tinhcongvanchuyen();
	x.tinhthanhtien();
	cout << "Thanh tien : " << x.thanhtien;
	getch();
}
