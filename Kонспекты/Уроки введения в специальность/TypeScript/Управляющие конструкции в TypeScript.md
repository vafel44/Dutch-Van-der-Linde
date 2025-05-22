#TypeScript #УсловныеКонструкции #ifElse #switch #Циклы #for #while #doWhile #УсловныеОператоры #тернарныйОператор #break #continue
## 1. Условные конструкции

### if...else

```typescript
let number: number = 10;

if (number > 0) {
    console.log("Число положительное");
} else if (number < 0) {
    console.log("Число отрицательное");
} else {
    console.log("Число равно нулю");
}
```

### switch

```typescript
let fruit: string = "apple";

switch (fruit) {
    case "banana":
        console.log("Это банан");
        break;
    case "apple":
        console.log("Это яблоко");
        break;
    default:
        console.log("Неизвестный фрукт");
}
```

## 2. Циклы

### for

```typescript
for (let i = 0; i < 5; i++) {
    console.log(i);
}
```

### while

```typescript
let i: number = 0;

while (i < 5) {
    console.log(i);
    i++;
}
```

### do...while

```typescript
let j: number = 0;

do {
    console.log(j);
    j++;
} while (j < 5);
```

## 3. Условные операторы

### тернарный оператор

```typescript
let age: number = 18;
let canVote: string = age >= 18 ? "Может голосовать" : "Не может голосовать";
console.log(canVote);
```

## 4. Прерывание циклов

### break

```typescript
for (let i = 0; i < 10; i++) {
    if (i === 5) {
        break; // Прерывает цикл, когда i равно 5
    }
    console.log(i);
}
```

### continue

```typescript
for (let i = 0; i < 10; i++) {
    if (i % 2 === 0) {
        continue; // Пропускает четные числа
    }
    console.log(i);
}
```