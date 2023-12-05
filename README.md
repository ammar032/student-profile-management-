//Libraries
#include<iostream>
#include<iomanip>
#include<cctype>
#include<algorithm>
#include<ctime>
#include<string>
#include<stdlib.h> 
using namespace std;

//Global Variables
int option1, option2, option3;
string sname1, sname2, sname3, reg;
string blood, emgc, dob, room, dname3, dname2, dname1;
string course_arr[6];

//Repeat Functions 
string addstrings(string sname1, string sname2)
{
	string sname3 = sname1 + " " + sname2;
	return sname3;
}
void declare()
{
	system("cls");
	cout << setw(95) << right << "Faculty Of Electrical Engineering\n" << endl;
	cout << setw(82) << right << "Section  D" << endl;
	cout << "\n";
	cout << "===========================================================================================================";
	cout << "================================================" << endl;
	cout << "\n";
	cout << setw(9) << left << "NAME   : " << setw(31) << left << sname3;
	cout << setw(104) << right << "DATE : " << __DATE__ << endl;
	cout << setw(9) << left << "REG NO : " << setw(31) << left << reg;
	cout << setw(104) << right << "Time : " << __TIME__ << endl;
	cout << "\n";
	cout << "===========================================================================================================";
	cout << "================================================" << endl;
	cout << "\n\n";
}

//Main Callout Functions
void registration()
{
	cout << "Please Enter Your Father's First Name" << endl;
	cin >> dname1;
	cout << "Please Enter Your Father's Last Name" << endl;
	cin >> dname2;
	cout << "Please Enter Your Date Of Birth e.g day/month/year (29/2/04) " << endl;
	cin >> dob;
	cout << "Please Enter Your Blood Group e.g B+" << endl;
	cin >> blood;
	cout << "Please Enter Your Emergency Contact" << endl;
	cin >> emgc;
	cout << "Please Enter You Hostel Room Number e.g hostel 11 room b-54 as (H-11/B-54)" << endl;
	cin >> room;

	dname3 = addstrings(dname1, dname2);
	system("cls");
}
void login()
{
	cout << "please enter your first name" << endl;
	cin >> sname1;
	cout << "please enter your last name" << endl;
	cin >> sname2;
	cout << "please enter your reg no" << endl;
	cin >> reg;


	sname3 = addstrings(sname1, sname2);
	system("cls");
}
void menu()
{
	cout << "1. Personal Information" << endl;
	cout << "\n";
	cout << "2. Timetable" << endl;
	cout << "\n";
	cout << "3. Courses" << endl;
	cout << "\n";
	cout << "4. Subjects" << endl;
	cout << "\n";
	cout << "5. Billing History" << endl;
	cout << "\n";
	cout << "6. Event Updates" << endl;
	cout << "\n";
	cout << "7. Annual Schedule" << endl;
	cout << "\n";
	cout << "8. Sign Out" << endl;
	cout << "\n\n";
	cout << "===========================================================================================================";
	cout << "================================================" << endl;
}
void personal_info()
{
	cout << "1. Personal Information : " << endl;
	cout << setw(27) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(27) << "" << setw(27) << "|Name                     |" << setw(25) << left << sname3 << "|" << endl;
	cout << setw(27) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(27) << "" << setw(27) << "|Father Name              |" << setw(25) << left << dname3 << "|" << endl;
	cout << setw(27) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(27) << "" << setw(27) << "|Room No                  |" << setw(25) << left << room << "|" << endl;
	cout << setw(27) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(27) << "" << setw(27) << "|Date Of Birth            |" << setw(25) << left << dob << "|" << endl;
	cout << setw(27) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(27) << "" << setw(27) << "|Emergency Contact        |" << setw(25) << left << emgc << "|" << endl;
	cout << setw(27) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(27) << "" << setw(27) << "|Blood Type               |" << setw(25) << left << blood << "|" << endl;
	cout << setw(27) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;

	cout << "2. Timetable" << endl;
	cout << "\n";
	cout << "3. Courses" << endl;
	cout << "\n";
	cout << "4. Subjects" << endl;
	cout << "\n";
	cout << "5. Billing History" << endl;
	cout << "\n";
	cout << "6. Event Updates" << endl;
	cout << "\n";
	cout << "7. Annual Schedule" << endl;
	cout << "\n";
	cout << "8. Sign Out" << endl;
	cout << "\n\n\n";
	cout << "===========================================================================================================";
	cout << "================================================" << endl;
}
void sem2_def()
{
	cout << "1. Personal Information" << endl;
	cout << "\n";
	cout << "2. Timetable" << endl;
	cout << "\n";

	cout << "3. Courses : \n";
	cout << setw(14) << "" << "Semester 1" << endl;
	cout << setw(14) << "" << "Semester 2 : " << endl;

	cout << setw(28) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(28) << "" << setw(53) << right << "|Course 1:                |N/A                      |" << endl;
	cout << setw(28) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(28) << "" << setw(53) << right << "|Course 2:                |N/A                      |" << endl;
	cout << setw(28) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(28) << "" << setw(53) << right << "|Course 3:                |N/A                      |" << endl;
	cout << setw(28) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(28) << "" << setw(53) << right << "|Course 4:                |N/A                      |" << endl;
	cout << setw(28) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(28) << "" << setw(53) << right << "|Course 5:                |N/A                      |" << endl;
	cout << setw(28) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(28) << "" << setw(53) << right << "|Course 6:                |N/A                      |" << endl;
	cout << setw(28) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << "\n\n";
	cout << "4. Subjects" << endl;
	cout << "\n";
	cout << "5. Billing History" << endl;
	cout << "\n";
	cout << "6. Event Updates" << endl;
	cout << "\n";
	cout << "7. Annual Schedule" << endl;
	cout << "\n";
	cout << "8. Sign Out" << endl;
	cout << "\n\n\n";
	cout << "===========================================================================================================";
	cout << "================================================" << endl;

}
void timetable()
{
	cout << "1. Personal Information" << endl;
	cout << "\n";
	cout << "2. Timetable : " << endl;
	cout << setw(14) << "" << " |------------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|" << endl;
	cout << setw(14) << "" << " |            |   08:00   |   09:00   |   10:00   |   10:30   |   11:30   |   12:30   |   01:30   |   02:30   |   03:30   |   04:30   |" << endl;
	cout << setw(14) << "" << " |    TIME    |     -     |     -     |     -     |     -     |     -     |     -     |     -     |     -     |     -     |     -     |" << endl;
	cout << setw(14) << "" << " |            |   08:50   |   09:50   |   10:50   |   11:20   |   12:20   |   01:20   |   02:20   |   03:20   |   04:20   |   05:20   |" << endl;
	cout << setw(14) << "" << " |------------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|" << endl;
	cout << setw(14) << "" << " |            |           |           |           |           |           |           |           |           |           |           |" << endl;
	cout << setw(14) << "" << " |   MONDAY   |           |   PH101   |           |   HM101   |           |           |   CH161   |   MT101   |   CH101   |           |" << endl;
	cout << setw(14) << "" << " |            |           |           |           |           |           |           |           |           |           |           |" << endl;
	cout << setw(14) << "" << " |------------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|" << endl;
	cout << setw(14) << "" << " |            |           |           |           |           |                       |           |                                   |" << endl;
	cout << setw(14) << "" << " |  TUESDAY   |           |           |   MT101   |           |      HM101 - LAB      |           |            PH101 - LAB            |" << endl;
	cout << setw(14) << "" << " |            |           |           |           |           |                       |           |                                   |" << endl;
	cout << setw(14) << "" << " |------------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|" << endl;
	cout << setw(14) << "" << " |            |           |           |           |           |           |           |           |                                   |" << endl;
	cout << setw(14) << "" << " |  WEDNESDAY |           |           |           |   MT101   |   CS101   |   PH101   |           |            IF101 - LAB            |" << endl;
	cout << setw(14) << "" << " |            |           |           |           |           |           |           |           |                                   |" << endl;
	cout << setw(14) << "" << " |------------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|" << endl;
	cout << setw(14) << "" << " |            |           |           |           |                                   |           |           |           |           |" << endl;
	cout << setw(14) << "" << " |  THURSDAY  |           |           |           |            CS101 - LAB            |           |   CH101   |   CS101   |   PH101   |" << endl;
	cout << setw(14) << "" << " |            |           |           |           |                                   |           |           |           |           |" << endl;
	cout << setw(14) << "" << " |------------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|" << endl;
	cout << setw(14) << "" << " |            |           |           |           |           |           |           |           |           |           |           |" << endl;
	cout << setw(14) << "" << " |   FRIDAY   |           |           |           |           |           |           |           |           |           |           |" << endl;
	cout << setw(14) << "" << " |            |           |           |           |           |           |           |           |           |           |           |" << endl;
	cout << setw(14) << "" << " |------------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|" << endl;

	cout << "\n";
	cout << "3. Courses" << endl;
	cout << "\n";
	cout << "4. Subjects" << endl;
	cout << "\n";
	cout << "5. Billing History" << endl;
	cout << "\n";
	cout << "6. Event Updates" << endl;
	cout << "\n";
	cout << "7. Annual Schedule" << endl;
	cout << "\n";
	cout << "8. Sign Out" << endl;
	cout << "\n\n";
	cout << "===========================================================================================================";
	cout << "================================================" << endl;
	
}
void sem2_edit()
{

	cout << "Enter N/A If Course Not Decided Yet." << endl;

	for (int i = 0; i < 6; i++)
	{
		cout << "Enter Course " << i + 1 << " : ";
		cin >> course_arr[i];
	}
}
void sem2_courses()
{
	cout << "1. Personal Information" << endl;
	cout << "\n";
	cout << "2. Timetable" << endl;
	cout << "\n";

	cout << "3. Courses : \n";
	cout << setw(14) << "" << "Semester 1" << endl;
	cout << setw(14) << "" << "Semester 2 : " << endl;

	cout << setw(28) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(28) << "" << setw(27) << right << "|Course 1:                |" << setw(25) << left << course_arr[0] << "|" << endl;
	cout << setw(28) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(28) << "" << setw(27) << right << "|Course 2:                |" << setw(25) << left << course_arr[1] << "|" << endl;
	cout << setw(28) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(28) << "" << setw(27) << right << "|Course 3:                |" << setw(25) << left << course_arr[2] << "|" << endl;
	cout << setw(28) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(28) << "" << setw(27) << right << "|Course 4:                |" << setw(25) << left << course_arr[3] << "|" << endl;
	cout << setw(28) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(28) << "" << setw(27) << right << "|Course 5:                |" << setw(25) << left << course_arr[4] << "|" << endl;
	cout << setw(28) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(28) << "" << setw(27) << right << "|Course 6:                |" << setw(25) << left << course_arr[5] << "|" << endl;
	cout << setw(28) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << "\n\n";

	cout << "4. Subjects" << endl;
	cout << "\n";
	cout << "5. Billing History" << endl;
	cout << "\n";
	cout << "6. Event Updates" << endl;
	cout << "\n";
	cout << "7. Annual Schedule" << endl;
	cout << "\n";
	cout << "8. Sign Out" << endl;
	cout << "\n\n\n";
	cout << "===========================================================================================================";
	cout << "================================================" << endl;
}



void selection()
{
	cout << "Please Select An Option : ";
	cin >> option1;
	cout << "\n\n";

	//main switch
	switch (option1)
	{
	case 1:
		declare();
		personal_info();
		break;
	case 2:
		declare();
		timetable();
		break;
	case 3:
		declare();
		cout << "1. Personal Information" << endl;
		cout << "\n";
		cout << "2. Timetable" << endl;
		cout << "\n";
		cout << "3. Courses : " << endl;
		cout << setw(14) << "" << "Semester 1" << endl;
		cout << setw(14) << "" << "Semester 2" << endl;
		cout << "\n\n";
		cout << "4. Subjects" << endl;
		cout << "\n";
		cout << "5. Billing History" << endl;
		cout << "\n";
		cout << "6. Event Updates" << endl;
		cout << "\n";
		cout << "7. Annual Schedule" << endl;
		cout << "\n";
		cout << "8. Sign Out" << endl;
		cout << "\n\n";
		cout << "===========================================================================================================";
		cout << "================================================" << endl;
		cout << "Please Select Semester Number : ";
		cin >> option2;
		cout << "\n\n";
		//switch for semester
		switch (option2)
		{
		case 1:
			break;
		case 2:
			declare();
			sem2_def();
			cout << "Press 0 To Edit Registered Courses : ";
			cin >> option3;
			cout << "\n\n";
			if (option3 == 0)
			{
				sem2_edit();
			}
			declare();
			sem2_courses();
			break;
		}
		break;
	case 4:
		break;
	case 5:
		break;
	case 6:
		break;
	case 7:
		break;
	case 8:
		break;
	}
}

//Main Function
int main()
{
	/*registration();*/

	login();

	declare();

	menu();

	selection();
}




