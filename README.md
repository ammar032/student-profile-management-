//Libraries
#include<iostream>
#include<iomanip>
#include<ctime>
#include<string>
#include<stdlib.h> 
using namespace std;


//Global Variables
int a,option1, option2, option4;
char option3;
char bmenu = 'e';
string sname1, sname2, sname3, reg;
string blood, emgc, dob, room, dname3, dname2, dname1;
string course_arr[6];
void selection();


//Repeat Functions 
string addstrings(string sname1, string sname2)
{
	string sname3 = sname1 + " " + sname2;
	return sname3;
}
void backtomenu()
{
	do
	{
		cout << "Press E To Exit : ";
		cin >> bmenu;
	} while (bmenu != 'E');
	system("cls");
}
void declare()
{
	system("cls");
	cout << setw(95) << right << "Faculty Of Electrical Engineering\n" << endl;
	cout << setw(82) << right << "Section  D" << endl;
	cout << "\n";
	cout << setfill('=') << setw(155) << "" << setfill(' ') << endl;
	cout << "\n";
	cout << setw(9) << left << "NAME   : " << setw(31) << left << sname3;
	cout << setw(104) << right << "DATE : " << __DATE__ << endl;
	cout << setw(9) << left << "REG NO : " << setw(31) << left << reg;
	cout << setw(104) << right << "Time : " << __TIME__ << endl;
	cout << "\n";
	cout << setfill('=') << setw(155) << "" << setfill(' ') << endl;
	cout << "\n\n";
}


//Main Callout Functions
void registration()
{
	cout << setw(19) << "" << setw(23) << "LMS PORTAL REGISTRATION" << setw(19) << "" << endl;
	cout << setfill('=') << setw(73) << "" << setfill(' ') << endl << endl << endl;
	cout << setw(8) << "" << setw(14) << "Father's First Name : ";
	cin >> dname1;
	cout << "\n";

	cout << setw(8) << "" << setw(14) << "Father's Last Name : ";
	cin >> dname2;
	cout << "\n";

	cout << setw(8) << "" << setw(14) << "Date Of Birth      : ";
	cin >> dob;
	cout << "\n";

	cout << setw(8) << "" << setw(14) << "Blood Group e.g B+ : ";
	cin >> blood;
	cout << "\n";

	cout << setw(8) << "" << setw(14) << "Emergency Contact  : ";
	cin >> emgc;
	cout << "\n";

	cout << setw(8) << "" << setw(14) << "Hostel Room Number : ";
	cin >> room;
	cout << "\n";

	dname3 = addstrings(dname1, dname2);
	system("cls");
}
void login()
{
	cout << setw(12) << left << "" << setw(17) << "LMS PORTAL  LOGIN" << setw(12) << "" << endl;
	cout << setfill('=') << setw(40) << "" << setfill(' ') << endl << endl << endl;
	cout << setw(8) << "" << setw(14) << "First Name : ";
	cin >> setw(14) >> sname1;
	cout << "\n\n";
	cout << setw(8) << "" << setw(14) << "Last Name  : ";
	cin >> setw(14) >> sname2;
	cout << "\n\n";
	cout << setw(8) << "" << setw(14) << "Reg No#    : ";
	cin >> setw(14) >> reg;
	cout << "\n\n";
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
	cout << setfill('=') << setw(155) << "" << setfill(' ') << endl;
}
void personal_info()
{
	cout << "Personal Information : " << endl;
	cout << setw(24) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(24) << "" << setw(27) << "|Name                     |" << setw(25) << left << sname3 << "|" << endl;
	cout << setw(24) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(24) << "" << setw(27) << "|Father Name              |" << setw(25) << left << dname3 << "|" << endl;
	cout << setw(24) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(24) << "" << setw(27) << "|Room No                  |" << setw(25) << left << room << "|" << endl;
	cout << setw(24) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(24) << "" << setw(27) << "|Date Of Birth            |" << setw(25) << left << dob << "|" << endl;
	cout << setw(24) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(24) << "" << setw(27) << "|Emergency Contact        |" << setw(25) << left << emgc << "|" << endl;
	cout << setw(24) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(24) << "" << setw(27) << "|Blood Type               |" << setw(25) << left << blood << "|" << endl;
	cout << setw(24) << "" << setw(53) << right << "|-------------------------|-------------------------|\n" << endl;
	cout << setfill('=') << setw(155) << "" << setfill(' ') << endl << endl;
	backtomenu();
}


//billing history
void billingsemester()
{
	double semesterbill;// semester 
	semesterbill = 400000;

	cout << setw(31) << "" << "|------------|------------|" << endl;
	cout << setw(31) << "" << "|Reg No      | " << setw(11) << reg << "|" << endl;
	cout << setw(31) << "" << "|------------|------------|" << endl;
	cout << setw(31) << "" << "|Name        | " << setw(11) << sname3 << "|" << endl;
	cout << setw(31) << "" << "|------------|------------|" << endl;
	cout << setw(31) << "" << "|Faculty     | " << setw(11) << " BEE " << "|" << endl;
	cout << setw(31) << "" << "|------------|------------|" << endl;
	cout << setw(31) << "" << "|Grand Total | " << setw(11) << semesterbill << "|" << endl;
	cout << setw(31) << "" << "|------------|------------|" << endl;
	cout << setfill('=') << setw(155) << "" << setfill(' ') << endl << endl;
	backtomenu();
}
void billingmess()
{
	double messbill;
	double fine;
	srand(time(0));
	
	messbill = (rand() % 15000);
	fine = (rand() % 800);
	cout << setw(25) << "" << "|------------|------------|" << endl;
	cout << setw(25) << "" << "|Reg No      | " << setw(11) << reg << "|" << endl;
	cout << setw(25) << "" << "|------------|------------|" << endl;
	cout << setw(25) << "" << "|Name        | " << setw(11) << sname3 << "|" << endl;
	cout << setw(25) << "" << "|------------|------------|" << endl;
	cout << setw(25) << "" << "|Faculty     | " << setw(11) << " BEE " << "|" << endl;
	cout << setw(25) << "" << "|------------|------------|" << endl;
	cout << setw(25) << "" << "|Grand Total | " << setw(11) << messbill << "|" << endl;
	cout << setw(25) << "" << "|------------|------------|" << endl;
	cout << setw(25) << "" << "|Fine        | " << setw(11) << fine << "|" << endl;
	cout << setw(25) << "" << "|------------|------------|" << endl;
	cout << setfill('=') << setw(155) << "" << setfill(' ') << endl << endl;
	backtomenu();
}
void month()
{
	int monthmess;
	cout << "Billing History : " << endl;
	cout << setw(18) << "" << "Mess : " << endl;
	cout << setw(25) << "" << right << "|-----------|" << endl;
	cout << setw(25) << "" << right << "|1:January  |" << endl;
	cout << setw(25) << "" << right << "|-----------|" << endl;
	cout << setw(25) << "" << right << "|2:February |" << endl;
	cout << setw(25) << "" << right << "|-----------|" << endl;
	cout << setw(25) << "" << right << "|3:March    |" << endl;
	cout << setw(25) << "" << right << "|-----------|" << endl;
	cout << setw(25) << "" << right << "|4:April    |" << endl;
	cout << setw(25) << "" << right << "|-----------|" << endl;
	cout << setw(25) << "" << right << "|5:May      |" << endl;
	cout << setw(25) << "" << right << "|-----------|" << endl;
	cout << setw(25) << "" << right << "|6:June     |" << endl;
	cout << setw(25) << "" << right << "|-----------|" << endl;
	cout << setw(25) << "" << right << "|7:July     |" << endl;
	cout << setw(25) << "" << right << "|-----------|" << endl;
	cout << setw(25) << "" << right << "|8:August   |" << endl;
	cout << setw(25) << "" << right << "|-----------|" << endl;
	cout << setw(25) << "" << right << "|9:September|" << endl;
	cout << setw(25) << "" << right << "|-----------|" << endl;
	cout << setw(25) << "" << right << "|10:October |" << endl;
	cout << setw(25) << "" << right << "|-----------|" << endl;
	cout << setw(25) << "" << right << "|11:November|" << endl;
	cout << setw(25) << "" << right << "|-----------|" << endl;
	cout << setw(25) << "" << right << "|12:December|" << endl;
	cout << setw(25) << "" << right << "|-----------|" << endl;
	cout << setfill('=') << setw(155) << "" << setfill(' ') << endl;
	cout << "Select Month : ";
	cin >> monthmess;

	switch (monthmess)
	{
	case 1:
		declare();
		cout << "Billing History : " << endl;
		cout << setw(18) << "" << "Mess : " << endl;
		cout << setw(26) << "" << "January\n" << endl;
		billingmess();
		break;
	case 2:
		declare();
		cout << "Billing History : " << endl;
		cout << setw(18) << "" << "Mess : " << endl;
		cout << setw(26) << "" << "February\n" << endl;
		billingmess();
		break;
	case 3:
		declare();
		cout << "Billing History : " << endl;
		cout << setw(18) << "" << "Mess : " << endl;
		cout << setw(26) << "" << "March\n" << endl;
		billingmess();
		break;
	case 4:
		declare();
		cout << "Billing History : " << endl;
		cout << setw(18) << "" << "Mess : " << endl;
		cout << setw(26) << "" << "April\n" << endl;
		billingmess();
		break;
	case 5:
		declare();
		cout << "Billing History : " << endl;
		cout << setw(18) << "" << "Mess : " << endl;
		cout << setw(26) << "" << "May\n" << endl;
		billingmess();
		break;
	case 6:
		declare();
		cout << "Billing History : " << endl;
		cout << setw(18) << "" << "Mess : " << endl;
		cout << setw(26) << "" << "June\n" << endl;
		billingmess();
		break;
	case 7:
		declare();
		cout << "Billing History : " << endl;
		cout << setw(18) << "" << "Mess : " << endl;
		cout << setw(26) << "" << "July\n" << endl;
		billingmess();
		break;
	case 8:
		declare();
		cout << "Billing History : " << endl;
		cout << setw(18) << "" << "Mess : " << endl;
		cout << setw(26) << "" << "August\n" << endl;
		billingmess();
		break;
	case 9:
		declare();
		cout << "Billing History : " << endl;
		cout << setw(18) << "" << "Mess : " << endl;
		cout << setw(26) << "" << "September\n" << endl;
		billingmess();
		break;
	case 10:
		declare();
		cout << "Billing History : " << endl;
		cout << setw(18) << "" << "Mess : " << endl;
		cout << setw(26) << "" << "October\n" << endl;
		billingmess();
		break;
	case 11:
		declare();
		cout << "Billing History : " << endl;
		cout << setw(18) << "" << "Mess : " << endl;
		cout << setw(26) << "" << "November\n" << endl;
		billingmess();
		break;
	case 12:
		declare();
		cout << "Billing History : " << endl;
		cout << setw(18) << "" << "Mess : " << endl;
		cout << setw(26) << "" << "December\n" << endl;
		billingmess();
		break;
	}
	cout << setfill('=') << setw(155) << "" << setfill(' ') << endl << endl;
}
void semesterchoice()
{
	int semester;
	cout << "Billing History : " << endl;
	cout << setw(18) << "" << "Select Semester : " << endl;
	cout << setw(36) << "" << right << "|--------------------|" << endl;
	cout << setw(36) << "" << right << "|1. FALL SEMESTER    |" << endl;
	cout << setw(36) << "" << right << "|--------------------|" << endl;
	cout << setw(36) << "" << right << "|2. SPRING SEMESTER  |" << endl;
	cout << setw(36) << "" << right << "|--------------------|" << endl;
	cout << setfill('=') << setw(155) << "" << setfill(' ') << endl;
	cout << "Select Semester : ";
	cin >> semester;

	switch (semester)
	{
	case 1:
		declare();
		cout << "Billing History : " << endl;
		cout << setw(18) << "" << "FALL SEMESTER : " << endl;
		billingsemester();
		break;
	case 2:
		declare();
		cout << "Billing History : " << endl;
		cout << setw(18) << "" << "SPRING SEMESTER : " << endl;
		billingsemester();
		break;
	}
}
void billingcall()
{

	cout << "Billing History : " << endl;
	cout << setw(18) << "" << "|-------------|" << endl;
	cout << setw(18) << "" << "| 1.Mess      |" << endl;
	cout << setw(18) << "" << "|-------------|" << endl;
	cout << setw(18) << "" << "| 2.Semester  |" << endl;
	cout << setw(18) << "" << "|-------------|\n" << endl;
	cout << setfill('=') << setw(155) << "" << setfill(' ') << endl;
	cout << "Select Option : ";
	cin >> option4;

}


//subject related
void quizmarks()
{

	double tquizscores = 10;//total marks of the quiz
	double obtquizscores;//Obtained marks of the quiz
	double average;

	srand(time(0));
	obtquizscores = (4 + rand() % 5);

	average = (rand() % 10);

	cout << setw(11) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(11) << "" << setw(27) << "|Total Marks              |" << setw(25) << left << tquizscores << "|" << endl;
	cout << setw(11) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(11) << "" << setw(27) << "|Obtained Marks           |" << setw(25) << left << obtquizscores << "|" << endl;
	cout << setw(11) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(11) << "" << setw(27) << "|Quiz Average             |" << setw(25) << left << average << "|" << endl;
	cout << setw(11) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << endl;
	cout << setfill('=') << setw(155) << "" << setfill(' ') << endl;

	if (obtquizscores >= average)
	{
		cout << "Your Score For Quiz Is Above Average " << endl;

	}
	else
	{
		cout << "Your Score For Quiz Is Below Average " << endl;
	}
	backtomenu();
	selection();
}
void quiznum()
{

	int b;//input for quiz number.

	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << setw(11) << "" << right << "|1.Quiz-1                 |" << endl;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << setw(11) << "" << right << "|2.Quiz-2                 |" << endl;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << setw(11) << "" << right << "|3.Quiz-3.                |" << endl;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << setw(11) << "" << right << "|4.Quiz-4.                |" << endl;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << setw(11) << "" << right << "|5.Quiz-5                 |" << endl;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << endl;
	cout << setfill('=') << setw(155) << "" << setfill(' ') << endl;
	cout << "Choose The Quiz : ";
	cin >> b;
	cout << endl;

	switch (b)
	{
	case 1:
		declare();
		cout << setw(12) << "" << right << "Quiz-1  \n\n";
		quizmarks();
		break;
	case 2:
		declare();
		cout << setw(12) << "" << right << "Quiz-2  \n\n";
		quizmarks();
		break;
	case 3:
		declare();
		cout << setw(12) << "" << right << "Quiz-3  \n\n";
		quizmarks();
		break;
	case 4:
		declare();
		cout << setw(12) << "" << right << "Quiz-4  \n\n";
		quizmarks();
		break;
	case 5:
		declare();
		cout << setw(12) << "" << right << "Quiz-5  \n\n";
		quizmarks();
		break;
	}

}
void mids()
{

	double totalmarks = 35;//total marks
	double marksobtained;// random num of absents generated
	double c_avearge;//class average

	srand(time(0));

	marksobtained = (10 + rand() % 35);

	c_avearge = (10 + rand() % 35);

	cout << setw(11) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(11) << "" << setw(27) << "|Total Marks              |" << setw(25) << left << totalmarks << "|" << endl;
	cout << setw(11) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(11) << "" << setw(27) << "|Obtained Marks           |" << setw(25) << left << marksobtained << "|" << endl;
	cout << setw(11) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(11) << "" << setw(27) << "|Class Average            |" << setw(25) << left << c_avearge << "|" << endl;
	cout << setw(11) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << endl;
	cout << setfill('=') << setw(155) << "" << setfill(' ') << endl;

	if (marksobtained >= c_avearge)
	{
		cout << "**You Are Free To Select The Next Course " << endl;

	}
	else
	{
		cout << "**LOL! Try Again Next Year" << endl;
	}
	backtomenu();
	selection();
}
void final()
{

	double totalmarks = 35;//total marks
	double marksobtained;// random num of absents generated
	double c_avearge;//class average

	srand(time(0));

	marksobtained = (10 + rand() % 35);

	c_avearge = (10 + rand() % 35);


	cout << setw(11) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(11) << "" << setw(27) << "|Total Marks              |" << setw(25) << left << totalmarks << "|" << endl;
	cout << setw(11) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(11) << "" << setw(27) << "|Obtained Marks           |" << setw(25) << left << marksobtained << "|" << endl;
	cout << setw(11) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(11) << "" << setw(27) << "|Class Average            |" << setw(25) << left << c_avearge << "|" << endl;
	cout << setw(11) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << endl;
	cout << setfill('=') << setw(155) << "" << setfill(' ') << endl;

	if (marksobtained >= c_avearge)
	{
		cout << "**You Are Free To Select The Next Course " << endl;

	}
	else
	{
		cout << "**LOL! Try Again Next Year" << endl;
	}
	backtomenu();
	selection();
}
void marks()
{
	int mark;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << setw(11) << "" << right << "|1.Quiz                   |" << endl;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << setw(11) << "" << right << "|2.Mids                   |" << endl;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << setw(11) << "" << right << "|3.Finals                 |" << endl;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << endl;
	cout << setfill('=') << setw(155) << "" << setfill(' ') << endl;
	cout << "Select Option : ";
	cin >> mark;
	cout << endl;

	switch (mark)
	{
	case 1:
		declare();
		cout << setw(12) << "" << right << "Quiz  \n\n";
		quiznum();
		break;
	case 2:
		declare();
		cout << setw(12) << "" << right << "Mids  \n\n";
		mids();
		break;
	case 3:
		declare();
		cout << setw(12) << "" << right << "Finals  \n\n";
		final();
		break;
	}
}
void attendance()
{
	double tclasses = 42;//total classes
	double cmissed;// random num of absents generated
	double classes_attended;
	double attendence;

	srand(time(0));

	classes_attended = 35 + (rand() % 7);

	cmissed = tclasses - classes_attended;

	attendence = ((classes_attended / tclasses) * 100);
	cout << setw(11) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(11) << "" << setw(27) << "|Total Classes            |" << setw(25) << left << tclasses << "|" << endl;
	cout << setw(11) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(11) << "" << setw(27) << "|Attended Classes         |" << setw(25) << left << classes_attended << "|" << endl;
	cout << setw(11) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(11) << "" << setw(27) << "|Missed Classes           |" << setw(25) << left << cmissed << "|" << endl;
	cout << setw(11) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(11) << "" << setw(27) << "|Attendance percentage    |" << setw(25) << left << attendence << "%" << "|" << endl;
	cout << setw(11) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << endl;
	cout << setfill('=') << setw(155) << "" << setfill(' ') << endl;


	if (attendence <= 80)
	{
		cout << "Please Try Again As Your Attendance Is Below 80% " << endl;

	}
	else
	{
		cout << "You Can Sit For The Finals :)" << endl;
	}
	backtomenu();
	selection();

}
void assignments()
{
	double tassignments = 42;//total classes
	double assignmentsmissed;// random num of absents generated
	double assignmentsgiven;
	double assignment;

	srand(time(0));

	assignmentsgiven = 35 + (rand() % 7);
	assignmentsmissed = tassignments - assignmentsgiven;
	assignment = ((assignmentsgiven / tassignments) * 100);

	cout << setw(11) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(11) << "" << setw(27) << "|Total Assignments        |" << setw(25) << left << tassignments << "|" << endl;
	cout << setw(11) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(11) << "" << setw(27) << "|Submitted Assignments    |" << setw(25) << left << assignmentsgiven << "|" << endl;
	cout << setw(11) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(11) << "" << setw(27) << "|Missed Assignments       |" << setw(25) << left << assignmentsmissed << "|" << endl;
	cout << setw(11) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(11) << "" << setw(27) << "|Assignment marks         |" << setw(5) << left << assignment << setw(18) << left << "%" << "|" << endl;
	cout << setw(11) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << endl;
	cout << setfill('=') << setw(155) << "" << setfill(' ') << endl;
	backtomenu();
	selection();
}
void sub()
{
	int marksorassignment;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << setw(11) << "" << right << "|1.Marks                  |" << endl;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << setw(11) << "" << right << "|2.Assignments            |" << endl;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << setw(11) << "" << right << "|3.Attendance             |" << endl;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << endl;
	cout << setfill('=') << setw(155) << "" << setfill(' ') << endl;
	cout << "Select Option : ";
	cin >> marksorassignment;
	cout << endl;

	switch (marksorassignment)
	{
	case 1:
		declare();
		cout << setw(11) << "" << right << "Marks  \n\n";
		marks();
		break;
	case 2:
		declare();
		cout << setw(11) << "" << right << "Assignments  \n\n";
		assignments();
		break;
	case 3:
		declare();
		cout << setw(11) << "" << right << "Attendance  \n\n";
		attendance();
		break;
	}
}
void subjectcall()
{
	int a;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << setw(11) << "" << right << "|1.PH101                  |" << endl;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << setw(11) << "" << right << "|2.PH101-LAB              |" << endl;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << setw(11) << "" << right << "|3.CH101                  |" << endl;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << setw(11) << "" << right << "|4.CH101-LAB              |" << endl;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << setw(11) << "" << right << "|5.CS101                  |" << endl;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << setw(11) << "" << right << "|6.CS101-101              |" << endl;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << setw(11) << "" << right << "|7.HM101                  |" << endl;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << setw(11) << "" << right << "|8.HM101-LAB              |" << endl;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << setw(11) << "" << right << "|9.CH161                  |" << endl;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << setw(11) << "" << right << "|10.IF101                 |" << endl;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << setw(11) << "" << right << "|11.MT101                 |" << endl;
	cout << setw(11) << "" << right << "|-------------------------|" << endl;
	cout << endl;
	cout << setfill('=') << setw(155) << "" << setfill(' ') << endl;
	cout << "Choose your subject : ";
	cin >> a;
	cout << endl;

	switch (a)
	{
	case 1:
		declare();
		cout << setw(12) << "" << right << "PH101 \n\n";
		sub();
		break;
	case 2:
		declare();
		cout << setw(12) << "" << right << "PH101-LAB \n\n";
		sub();
		break;
	case 3:
		declare();
		cout << setw(12) << "" << right << "CH101 \n\n";
		sub();
		break;
	case 4:
		declare();
		cout << setw(12) << "" << right << "CH101-LAB \n\n";
		sub();
		break;
	case 5:
		declare();
		cout << setw(12) << "" << right << "CS101 \n\n";
		sub();
		break;
	case 6:
		declare();
		cout << setw(12) << "" << right << "CS101-101 \n\n";
		sub();
		break;
	case 7:
		declare();
		cout << setw(12) << "" << right << "HM101 \n\n";
		sub();
		break;
	case 8:
		declare();
		cout << setw(12) << "" << right << "HM101-LAB \n\n";
		sub();
		break;
	case 9:
		declare();
		cout << setw(12) << "" << right << "CH161 \n\n";
		sub();
		break;
	case 10:
		declare();
		cout << setw(12) << "" << right << "IF101 \n\n";
		sub();
		break;
	case 11:
		declare();
		cout << setw(12) << "" << right << "MT101 \n\n";
		sub();
		break;
	}

}


//timetable
void timetable()
{
	cout << "Timetable : " << endl;
	cout << setw(11) << "" << " |------------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|" << endl;
	cout << setw(11) << "" << " |            |   08:00   |   09:00   |   10:00   |   10:30   |   11:30   |   12:30   |   01:30   |   02:30   |   03:30   |   04:30   |" << endl;
	cout << setw(11) << "" << " |    TIME    |     -     |     -     |     -     |     -     |     -     |     -     |     -     |     -     |     -     |     -     |" << endl;
	cout << setw(11) << "" << " |            |   08:50   |   09:50   |   10:50   |   11:20   |   12:20   |   01:20   |   02:20   |   03:20   |   04:20   |   05:20   |" << endl;
	cout << setw(11) << "" << " |------------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|" << endl;
	cout << setw(11) << "" << " |            |           |           |           |           |           |           |           |           |           |           |" << endl;
	cout << setw(11) << "" << " |   MONDAY   |           |   PH101   |           |   HM101   |           |           |   CH161   |   MT101   |   CH101   |           |" << endl;
	cout << setw(11) << "" << " |            |           |           |           |           |           |           |           |           |           |           |" << endl;
	cout << setw(11) << "" << " |------------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|" << endl;
	cout << setw(11) << "" << " |            |           |           |           |           |                       |           |                                   |" << endl;
	cout << setw(11) << "" << " |  TUESDAY   |           |           |   MT101   |           |      HM101 - LAB      |           |            PH101 - LAB            |" << endl;
	cout << setw(11) << "" << " |            |           |           |           |           |                       |           |                                   |" << endl;
	cout << setw(11) << "" << " |------------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|" << endl;
	cout << setw(11) << "" << " |            |           |           |           |           |           |           |           |                                   |" << endl;
	cout << setw(11) << "" << " |  WEDNESDAY |           |           |           |   MT101   |   CS101   |   PH101   |           |            IF101 - LAB            |" << endl;
	cout << setw(11) << "" << " |            |           |           |           |           |           |           |           |                                   |" << endl;
	cout << setw(11) << "" << " |------------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|" << endl;
	cout << setw(11) << "" << " |            |           |           |           |                                   |           |           |           |           |" << endl;
	cout << setw(11) << "" << " |  THURSDAY  |           |           |           |            CS101 - LAB            |           |   CH101   |   CS101   |   PH101   |" << endl;
	cout << setw(11) << "" << " |            |           |           |           |                                   |           |           |           |           |" << endl;
	cout << setw(11) << "" << " |------------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|" << endl;
	cout << setw(11) << "" << " |            |           |           |           |           |           |           |           |           |           |           |" << endl;
	cout << setw(11) << "" << " |   FRIDAY   |           |           |           |           |           |           |           |           |           |           |" << endl;
	cout << setw(11) << "" << " |            |           |           |           |           |           |           |           |           |           |           |" << endl;
	cout << setw(11) << "" << " |------------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|-----------|" << endl;
	cout << "\n";
	cout << setfill('=') << setw(155) << "" << setfill(' ') << endl << endl;
	backtomenu();

}


//courses
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
	cout << "Courses : \n";
	cout << setw(11) << "" << "Semester 2 : " << endl;

	cout << setw(25) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(25) << "" << setw(27) << right << "|Course 1:                |" << setw(25) << left << course_arr[0] << "|" << endl;
	cout << setw(25) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(25) << "" << setw(27) << right << "|Course 2:                |" << setw(25) << left << course_arr[1] << "|" << endl;
	cout << setw(25) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(25) << "" << setw(27) << right << "|Course 3:                |" << setw(25) << left << course_arr[2] << "|" << endl;
	cout << setw(25) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(25) << "" << setw(27) << right << "|Course 4:                |" << setw(25) << left << course_arr[3] << "|" << endl;
	cout << setw(25) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(25) << "" << setw(27) << right << "|Course 5:                |" << setw(25) << left << course_arr[4] << "|" << endl;
	cout << setw(25) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(25) << "" << setw(27) << right << "|Course 6:                |" << setw(25) << left << course_arr[5] << "|" << endl;
	cout << setw(25) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << "\n";
	cout << setfill('=') << setw(155) << "" << setfill(' ') << endl << endl;
}
void sem1_courses()
{
	cout << "Courses : \n";
	cout << setw(11) << "" << "Semester 1 : " << endl;
	cout << setw(25) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(25) << "" << setw(53) << right << "|Course 1:                |HM-101                   |" << endl;
	cout << setw(25) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(25) << "" << setw(53) << right << "|Course 2:                |MT-101                   |" << endl;
	cout << setw(25) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(25) << "" << setw(53) << right << "|Course 3:                |PH-101                   |" << endl;
	cout << setw(25) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(25) << "" << setw(53) << right << "|Course 4:                |CH-161                   |" << endl;
	cout << setw(25) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(25) << "" << setw(53) << right << "|Course 5:                |CH-101                   |" << endl;
	cout << setw(25) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(25) << "" << setw(53) << right << "|Course 6:                |CS-101                   |" << endl;
	cout << setw(25) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(25) << "" << setw(53) << right << "|Course 7:                |CS-101 LAB               |" << endl;
	cout << setw(25) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(25) << "" << setw(53) << right << "|Course 8:                |PH-101 LAB               |" << endl;
	cout << setw(25) << "" << setw(53) << right << "|-------------------------|-------------------------|" << endl;
	cout << setw(25) << "" << setw(53) << right << "|Course 9:                |IF-101 LAB               |" << endl;
	cout << setw(25) << "" << setw(53) << right << "|-------------------------|-------------------------|\n" << endl;
	cout << "\n";
	cout << setfill('=') << setw(155) << "" << setfill(' ') << endl << endl;
	backtomenu();
}


//event update
struct Event
{
	string name;
	string date;
	string location;
};
void displayEvents(Event events[], int size)
{
	cout << "Event Updates   : " << endl;

	cout << setw(21) << "" << left << setw(45) << "Event" << setw(30) << "Date" << setw(30) << "Location\n";
	cout << setfill('=') << setw(105) << "" << setfill(' ') << endl << endl;

	for (int i = 0; i < size; ++i) {
		Event event = events[i];
		cout << setw(21) << "" << setw(45) << event.name;
		cout << setw(30) << event.date;
		cout << setw(30) << event.location << endl;
		cout << setw(21) << "" << setfill('-') << setw(105) << "" << setfill(' ') << endl;
	}
	cout << "\n";
	cout << setfill('=') << setw(155) << "" << setfill(' ') << endl << endl;
	backtomenu();
}
void displayUniversityEvents()
{
	// Global array to store the events
	Event events[] =
	{
		{"Annual Tech Conference", "January 15-17, 2024", "Auditorium"},
		{"Alumni Reunion", "January, 2024", "Auditorium"},
		{"Inauguration of New Academic Building", "February 1, 2024", "Backside GiKafe"},
		{"Open House", "February 25-26, 2024", "Giki"}
	};

	displayEvents(events, sizeof(events) / sizeof(events[0]));
}


//annual schedule
struct Event2
{
	string name;
	string date;
	string duration;
};
void displaySchedule(Event2 events2[], int size)
{
	cout << "Annual Schedule : " << endl;

	cout << setw(18) << "" << left << setw(45) << "Event" << setw(45) << "Date" << setw(15) << "Duration\n";
	cout << setw(12) << "" << setfill('=') << setw(105) << "" << setfill(' ') << endl << endl;

	for (int i = 0; i < size; ++i) {
		Event2 event2 = events2[i];
		cout << setw(18) << "" << setw(45) << event2.name;
		cout << setw(45) << event2.date;
		cout << setw(15) << event2.duration << endl;
		cout << setw(18) << "" << setfill('-') << setw(105) << "" << setfill(' ') << endl;
	}
	cout << endl;
	cout << "\n";
	cout << setfill('=') << setw(155) << "" << setfill(' ') << endl << endl;
	backtomenu();
}
void displayUniversitySchedule()
{
	Event2 events2[] = {

		{"Fresh Person Orientation", "September 02 - 03, 2023", "2 days"},
		{"Fall Semester starts", "September 04, 2023"},
		{"Classes" , "September 04,2023 - October 27 2023", "8 weeks"},
		{"Mid-Term Examination" , "October 30, 2023 - November 3, 2023", "1 week"},
		{"Mid-Term Examination" , "October 30, 2023 - November 3, 2023", "1 week"},
		{"Classes" , "November 13, 2023 - December 29, 2023", "7 weeks"},
		{"Final Examination" , "January 01, 2024 - January 07, 2024", "1 week"},
		{"End of Semester Break" , "January 08, 2024 - January 19, 2024", "2 weeks"},
		{"Spring Semester Begins" , "January 22, 2024"},
		{"Classes" , "January 22, 2024 - March 15, 2024", "8 weeks"},
		{"Mid-Term Examinations" , "March 18, 2024 - March 22, 2024", "1 week"},
		{"Classes" , "March 25, 2024 - April 05, 2024", "2 weeks"},
		{"Eid-ul-Fitr Break" , "April 08, 2024 - April 12, 2024", "1 week"},
		{"Classes" , "April 15, 2024 - May 10, 2024", "5 weeks"},
		{"Final Examinations" , "May 20, 2024 - May 26, 2024", "1 week"},
		{"End of Semester Break" , "May 27, 2024 - June 07, 2024", "2 weeks"},
		{"Summer School Begins" , "June 10, 2024"},
		{"Classes" , "June 10, 2024 - June 14, 2024", "1 week"},
		{"Eid-ul-Adha Break" , "June 15, 2024 - June 21, 2024", "1 week"},
		{"Classes" , "June 24, 2024 - August 09, 2024", "7 weeks"},
		{"Final Examination" , "August 12, 2024 - August 17, 2024", "1 week"},
		{"End of Summer Break" , "August 19, 2024 - August 30, 2024", "2 weeks"},
		{"End of Semester Break" , "January 08, 2024 - January 19, 2024", "2 weeks"},
		{"Orientation of Freshmen" , "September 01, 2024 - September 01, 2024", "1 day"},
		{"Fall Semester Starts" , "September 02, 2024"},
	};

	displaySchedule(events2, sizeof(events2) / sizeof(events2[0]));
}


//menu selection
void selection()
{
	declare();
	menu();
	cout << "Please Select An Option : ";
	cin >> option1;
	cout << "\n\n";

	//main switch
	switch (option1)
	{
	case 1:
		declare();
		personal_info();
		selection();
		break;
	case 2:
		declare();
		timetable();
		selection();
		break;
	case 3:
		declare();
		cout << "1. Personal Information" << endl;
		cout << "\n";
		cout << "2. Timetable" << endl;
		cout << "\n";
		cout << "3. Courses : \n" << endl;
		cout << setw(13) << "" << "|-------------------------|" << endl;
		cout << setw(13) << "" << "|     1. Semester_1       |" << endl;
		cout << setw(13) << "" << "|-------------------------|" << endl;
		cout << setw(13) << "" << "|     2. Semester_2       |" << endl;
		cout << setw(13) << "" << "|-------------------------|" << endl;
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
		cout << setfill('=') << setw(155) << "" << setfill(' ') << endl;
		cout << "Please Select Semester Number : ";
		cin >> option2;
		cout << "\n\n";
		//switch for semester
		switch (option2)
		{
		case 1:
			declare();
			sem1_courses();
			selection();
			break;
		case 2:
			declare();
			sem2_courses();
			cout << "Press Q To Edit All Registered Courses Or E To Exit : ";
			cin >> option3;
			cout << "\n\n";
				if (option3 == 'Q')
				{
					sem2_edit();
					declare();
					sem2_courses();
					backtomenu();
					selection();
				}
				if (option3 == 'E')
				{
					selection();
				}
			break;
		}
		break;

	case 4:
		declare();
		cout << "Subjects : \n" << endl;
		subjectcall();
		break;
	case 5:
		declare();
		billingcall();
		switch (option4)
		{
		case 1:
			declare();
			month();
			system("cls");
			break;
		case 2:
			declare();
			semesterchoice();
			system("cls");
			break;
		}
		declare();
		menu();
		selection();
		break;
	case 6:
		declare();
		displayUniversityEvents();
		selection();
		break;
	case 7:
		declare();
		displayUniversitySchedule();
		selection();
		break;
	case 8:
		cout << "\n\n";
		system("cls");
		cout << setw(56) << "" << "You Have Successfully Signed Out Of The Program!\n\n\n" << endl;
		break;
	}
}

//Main Function
int main()
{
	registration();

	login();

	selection();

}

