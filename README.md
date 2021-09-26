 #include <iostream>
using namespace std;
int dfs(int n)
{
    if (n == 1) 
	return 1;
    if (n == 2) 
	return 2;
    return dfs(n - 1) + dfs(n - 2);
}
int main()
{
    int f, ans;
    cin >> f;
    ans = dfs(f);
    cout << ans << endl;
    return 0;
}
