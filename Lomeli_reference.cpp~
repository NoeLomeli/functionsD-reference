//Name: Noe Lomeli
//Date: October 15, 2015
//Project FunctionsD-reference

#include <iostream>
#include <string>
using namespace std;
// ********************************************************
void sort(int& numA, int& numB, int& numC);
// Summary: Sorts three numbers in increasing order
// Precondition: Three ints to be sorted are passed by value into the function; three ints are passed 
// by reference in increasing order.
// Postcondition: Three ints are sorted and stored in their new variable according to increasing order.
//
// ********************************************************
void numDigits(int valA, int& n);
// Summary: determines the number of digits in an integer.
// Precondition: one int to be passed by value into the function; one int is passed 
// by reference with the value of the number of digits.
// Postcondition: after the int is passed by value into the function,the number of digits is stored in the passed by reference integer
//
// ********************************************************
void computeSphere(double& a, double& v, double r);
// Summary: Calculates the volume and area of asphere
// Precondition: one double to be passed by value into the function; two doubles are passed 
// by reference with the value of area and volume.
// Postcondition: after the double is passed by value into the function,the values for area and volume are stored in the passed by reference doubles
//
// ********************************************************
void swap(int& A, int& B);
// Summary: Swaps int A with int B 
// Precondition: two ints have to be passed by value into the function; two ints are passed 
// by reference with the value of each other swapped
// Postcondition: after the doubles are passed by value into the function,the values for each int is swapped in the other.
//
// ********************************************************
int main()
{
    //sorting formula
    int numA =2, numB =30, numC = -50;
    cout << "result expected: Invalid input result: ";
    sort(numA, numB, numC);
    int numD =10, numE =3, numF = 50;
    cout << "result expected: 3 10 50 result: ";
    sort(numD, numE, numF);
    int numG =0, numH =100, numI = 50;
    cout << "result expected: 0 50 100 result: ";
    sort(numG, numH, numI);
    
    //number of digits
    int valA = 10000;
    int n = 0;
    cout << "result expected: 5 result: ";
    numDigits(valA, n);
    int valB = -100;
    int v = 0;
    cout << "result expected: 3 result: ";
    numDigits(valB, v);
    int valC = -10001;
    int i = 0;
    cout << "result expected: Invalid result -- result: ";
    numDigits(valC, i);
    
    //volume and area of a sphere
    double rad = 5;
    double valA1 = 0;
    double valA2 = 0;
    cout << "result expected area: 314.16 volume: 523.6 -- result: ";
    computeSphere(valA1, valA2, rad);
    double rad2 = -5;
    double valB1 = 0;
    double valB2 = 0;
    cout << "result expected: Invalid input -- result: ";
    computeSphere(valB1, valB2, rad2); 
    double rad3 = 10;
    double valC1 = 0;
    double valC2 = 0;
    cout << "result expected area: 1256.64  volume: 4188.79  -- result: ";
    computeSphere(valC1, valC2, rad3); 
    
    //swap integer places
    int A = 10;
    int B = 33;
    cout << "result expected: 33 10  -- result: ";
    swap(A, B);
    int A1 = 45;
    int B1 = 56;
    cout << "result expected: 56 45  -- result: ";
    swap(A1, B1);
    
    return 0;


}//main

void sort(int& numA, int& numB, int& numC)
{    
    if(((numA >= 0) && (numA <= 100)) && ((numB >= 0) && (numB <= 100)) && ((numC >= 0) && (numC <= 100)))//accounts for all numbers to be greater than 0 and less than 100
    {
        int temp = 0;
        if ((numB > numC) && (numB > numA))
        { 
            temp = numA;
            numA = numB;
            numB = numC;
            numC = temp;
            cout << numC << " " << numB << " " << numA << endl;
           
        }//if
       
        else if ((numA > numC) && (numC > numB))
        { 
            temp = numB;
            numB = numC;
            numC = temp;       
            cout << numC << " " << numB << " " << numA << endl;   
        }//else if
        else if ((numA > numB) && (numC > numA))
        { 
            temp = numA;
            numA = numC;
            numC = numB;
            numB = temp;       
            cout << numC << " " << numB << " " << numA << endl;   
        }//else if
        else
        {
            cout << numC << " " << numB << " " << numA << endl;     
        }//else
    }//if
    else
        cout << "Invalid input" << endl;//if input does not meet conditions
    return;
}//sort 
void numDigits(int valA, int& n)
{
    if ((valA >= -10000) && (valA <= 10000))//input cannot be less than -10000 or greater than 10000
    {
        if ((valA >= -9) && (valA <= 9))
        {
            n = 1;
            cout << n << endl;
        }
        else if ((valA >= 10) && (valA <= 99))  
        {
            n = 2;
            cout << n << endl;
        }
        else if ((valA >= -99) && (valA <= -10))
        {
            n = 2;
            cout << n << endl;
        }
        else if ((valA >= 100) && (valA <= 999))  
        {
            n = 3;
            cout << n << endl;
        }
        else if ((valA >= -999) && (valA <= -100))
        {
            n = 3;
            cout << n << endl;
        }
        else if ((valA >= 1000) && (valA <= 9999)) 
        {
            n = 4;
            cout << n << endl;
        }
        else if ((valA >= -9999) && (valA <= -1000))
        {
            n = 4;
            cout << n << endl;
        }
        else
        {
            n = 5;
            cout << n << endl;
        }    
            
    }//outter if
    
    else
        cout << "Invalid input" << endl;
        
    
    return;
}//numDigits
void computeSphere(double& a, double& v, double r)
{
     const double PI = 3.14;
     if ((r >= 0) && (r <= 10000))//radius cannot be less than 0 or greater than 10000
    {
        a = 4 * PI * r * r; //formula for area of sphere
        v = (4 * PI * r * r * r) / 3;//formula for volume
        cout << a << " " << v << endl;
    }//if
    else
    {
        cout << "Invalid input" << endl;    
    }//else
    return;   

}//calcAreaPerimeter 
void swap(int& A, int& B)
{
    int temp;
    temp = A;
    A = B;
    B = temp;
    cout << A << " " << B << endl;

}//void  
