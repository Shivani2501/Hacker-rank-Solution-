# Hacker-rank-Solution-
I have written this code of day of a programmer on hackerrank in problem solving in C++
string dayOfProgrammer(int year) {
    
 string yr;   
if(year==1918)
{
    yr="26.09.1918";
}
else if(((year <=1917) && (year % 4==0)) || ((year>1918) &&((year%400==0)||((year%4==0)&&(year%100!=0)))))
  {
      yr="12.09."+to_string(year);
  }
 else {
     yr="13.09."+to_string(year);
 } 
return yr;

}
