# Hacker-rank-Solution-
I have written code for Viral Advertising question on hacker rank in c++
#include <bits/stdc++.h>

using namespace std;

// Complete the viralAdvertising function below.
int viralAdvertising(int n) {

double shared=5;
double liked =floor(shared/2);
double cumulative=liked;;
for(int i=1;i<n;i++)
{
    shared = liked*3;
    liked = floor(shared/2);
    cumulative +=liked;
    
}
return cumulative;
}

int main()
{
    ofstream fout(getenv("OUTPUT_PATH"));

    int n;
    cin >> n;
    cin.ignore(numeric_limits<streamsize>::max(), '\n');

    int result = viralAdvertising(n);

    fout << result << "\n";

    fout.close();

    return 0;

