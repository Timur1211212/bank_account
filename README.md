#include <iostream>
using namespace std;

struct bank_account {
    int account_number;
    std::string owners_name;
    int balance;
    int new_balance;
};

int main()
{
    setlocale(LC_ALL, "rus");
    bank_account instance_fields;

    cout << "Введите номер счёта: ";
    cin >> instance_fields.account_number;
    cout << "Введите имя владельца: ";
    cin >> instance_fields.owners_name;
    cout << "Введите баланс: ";
    cin >> instance_fields.balance;
    cout << "Введите новый баланс: ";
    cin >> instance_fields.new_balance;

    cout << "Ваш счёт: " << instance_fields.owners_name << ", " << instance_fields.account_number << ", " << instance_fields.new_balance;
    return 0;
}
