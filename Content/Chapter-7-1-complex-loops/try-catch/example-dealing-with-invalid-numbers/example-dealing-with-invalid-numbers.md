### Пример: справяне с грешни числа чрез try-catch

Да се напише програма, която проверява дали едно число **n** е четно и ако е, да се отпечатва на екрана. При **невалидно въведено** число да се изписва съобщение, че въведения вход не е валидно число и въвеждането да продължи отново.

Ето как можем да решим задачата:

* Създаваме безкраен **`while`** цикъл, като за условие ще зададем **`true`**.
* В тялото на цикъла:
	* Създаваме **`try-catch`** конструкция.
	* В **`try`** блока пишем програмната логика за четене на потребителския вход, парсването му до число и проверката за четност.
	* При **четно число** го отпечатваме и излизаме от цикъла (с **`break`**). Програмата си е свършила работата и приключва.
	* При **нечетно число** отпечатваме съобщение, че се изисква четно число, без да излизаме от цикъла (защото искаме той да се повтори отново).
	* Ако **хванем изключение** при изпълнението на **`try`** блока, изписваме съобщение за невалидно въведено число (и цикълът съответно се повтаря, защото не излизаме изрично от него).