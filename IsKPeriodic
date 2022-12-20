#include <iostream>
#include  <string>
using namespace std;

bool IsKPeriodic(const string& arr, const int k)
{
	if (k <= 0) {
		cout << "Число должно быть больше 0!" << endl;
		return false;
	}
	string a(k, ' ');
	if (k <= arr.size()) {
		for (int i = 0; i < k; i++) {
			a[i] = arr[i];
		}
	}
	else { return false; }
	int j = 0;
	int g = 0;

	for (int i = 0; i < arr.size(); i = i + k) {
		j = i;
		while (j < a.size()) {
			if (arr[j] == a[j]) {
				j++;
				continue;
			}
			else { return false; }
		}
		g++;
	}
	if (arr.size() / k == g) { return true; }
	return false;
}
	int main() {
		setlocale(LC_ALL, "rus");
		string arr = "SergiySergiySergiySergiySergiySergiy";
		int k = 6;

		if (IsKPeriodic(arr, k)) {
			cout << "Строка кратна числу " << k << "!" << endl;
		}
		else {
			cout << "Строка НЕ кратна числу " << k << "!" << endl;
		}
		return 0;
	}

