importjava.lang.*; importjava.io.*; importjava.util.Scanner;
publicclasssa
{
publicstaticintshowresult(intaa)throwsArithmeticException
{
intresult=12/aa;
returnresult;
}
publicstaticvoidsetdata(Stringinput)
{
intvalue=0;
try
{
value=Integer.parseInt(input);
}
catch(NumberFormatExceptionaaaaaa)
{
System.out.println("BadInputData!!");
return;
}
try
{
System.out.println("Resultis:"+showresult(value));
}
catch(ArithmeticExceptionaaaaaa)
{
System.out.println("Divisionbyzero!!");
}
}
publicstaticvoidmain(String[]a)
{
Scannerscan=newScanner(System.in); StringinData;
System.out.print("Enterthedivisor:"); inData=scan.next();
setdata(inData);
}
}
