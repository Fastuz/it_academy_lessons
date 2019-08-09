/* Создайте функцию которая просит у пользователя следующую информацию:
- Имя
- Фамилия
- Пол
- Возраст
После получения всей информации функция должна вывести в alert следующий результат:
Полное имя: Иван Иванов
Пол: М
На пенсии: Да
Учтите, что пенсионный возраст зависит от пола.
Для некоторых этапов ввода информации должна быть проверка на валидность.
Возраст может быть только положительным числом отличным от нуля,
пол может быть только М или Ж (возможен ввод строчными буквами). Имя и фамилия могут быть любыми кроме null и пустой строки.*/
function userQuestions() {
  let lastName = prompt('Введите ваше имя');
  while (lastName <= null) {
    if (lastName <= null)
      lastName = prompt('Это поле нельзя оставить пустым, введите имя');
    else
      break
  }
  let firstName = prompt('Введите вашу фамилию');
  while (firstName <= null) {
    if (firstName <= null)
      firstName = prompt('Это поле нельзя оставить пустым, введите фамилию');
    else
      break
  }
  let gender = prompt('Ваш пол М или Ж?');
  if ((gender === 'М') || (gender === 'м')) gender = 'М';
    else
    if ((gender === 'Ж') || (gender === 'ж')) gender = 'Ж';
  let userInput,
      age;
  while(!Number.isFinite(age)){
    let userInput = prompt("Сколько Вам лет?");
    age = userInput && Number(userInput);
  }
  while (age <= -1) {
    if (age <= -1)
      age = prompt('Возраст не может быть отридцательным, попробуйте еще раз');
    else
      break
  }
  let end;
  if (gender === 'М') {
    if (age >= 60) end = 'да';
    else end = "нет";
    if (gender === 'Ж') {
      if (age >= 55) end = 'да';
      else end = 'нет';
    }
    alert('Полное имя:  ' + lastName + ' ' + firstName + " \nВаш пол:  " + gender + "\nВы на пенсии:  " + end);
    //да это не удобно, делать такую длинную запись, но разок можно
  }
}
userQuestions();
