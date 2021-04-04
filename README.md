# Hacker-rank-Solution-
I have written code for Mark and Toys question on hacker rank in c++
int maximumToys(vector<int> prices, int k) {
int n=prices.size();
int sum=0;
int count=0;
sort(prices.begin(),prices.end());
for(int i=0;i<n;i++)
{
    if(sum<=k)
    {sum+=prices[i];
    count++;
    }
}
return count-1;
}
