#include <iostream>
#include <sstream>
#include <vector>
#include <string>

using namespace std;

// This is the function required by HackerRank to be completed
vector<int> parseInts(string str) {
    stringstream ss(str); 
    vector<int> parsed_ints;
    char ch;   
    int temp;  

    // Optimal logic: reads integer (temp), then consumes delimiter (ch)
    while (ss >> temp) { 
        parsed_ints.push_back(temp); 
        ss >> ch; // Attempts to consume the delimiter (the comma)
    }
    
    return parsed_ints;
}

// This is the main driver code (handles I/O)
int main() {
    string str;
    cin >> str; 

    vector<int> integers = parseInts(str);

    for (size_t i = 0; i < integers.size(); i++) {
        cout << integers[i] << "\n";
    }

    return 0;
}