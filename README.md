#include <iostream>
#include <algorithm>

using namespace std;

int main()
{
    int colors[4];
    for (int i = 0; i < 4; ++i)
    {
        cin >> colors[i];
    }

    sort(colors, colors + 4);

    int b = 0;
    for (int i = 1; i < 4; ++i)
    {
        if (colors[i] == colors[i - 1])
        {
            b++;
        }
    }

    cout << b << endl;

    return 0;
}


