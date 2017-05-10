# Student-manual-information-inquiry-system
学生手册信息查询系统
//#include<iostream>
#include<fstream>

using namespace std;

class SYSTEM
{
private:
	ofstream fout;
public:
	SYSTEM();
	~SYSTEM();
	void writein();
};

SYSTEM::SYSTEM()
{
	fout.open("学生手册信息");
}

SYSTEM::~SYSTEM()
{
	fout.close();
}

void SYSTEM::writein()
{
	fout<<"我的信息";
}

int main()
{
	SYSTEM system;
	system.writein();
	return 0;
}
