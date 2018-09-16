# 9.16.1
范围for循环&amp;Vector
// 9.15.2新版本实验.cpp : 定义控制台应用程序的入口点。
//

#include "stdafx.h"
#include<iostream>
#include<vector> //容器，表示对象的集合

using namespace std;
int main()
{
	vector<int> c = { 1,2,3,4 };
	//范围变量必须是引用类型，这样才能对元素执行写操作
	for (auto &r : c) { //对于C中的每一个元素
		r=r * 2 ;
	}
	for (int i = 0; i < 4; i++) {
		cout << c[i] << " ";
	}
    return 0;
}
